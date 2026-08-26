# Metodologia e fontes: como esta base de dados é feita

**Os dados deste repositório saem de fonte oficial, sempre: o cadastro de pórticos da ANTT para as rodovias federais concedidas, os portais das agências estaduais para as estaduais, e o canal da própria concessionária para prazo, endereço de pagamento e regra de isenção. Nada é inferido, deduzido ou preenchido por analogia. O que não foi confirmado aparece como `n/d`, e quando duas fontes oficiais discordam a divergência é registrada em vez de escondida.**

Esta página existe para que qualquer pessoa possa auditar o que está publicado aqui: de onde veio cada número, o que conta como um pórtico, o que fazemos diante de fontes conflitantes e com que frequência tudo isso é revisto.

> Publicado em 26 de agosto de 2026. Última atualização em 26 de agosto de 2026.
> Parte do repositório [Free Flow e Tag de Pedágio, pelo Sem Parar](../README.md). O significado de cada coluna das bases está no [dicionário de dados](../dados/README.md).

---

## Índice

- [De onde vem cada dado](#de-onde-vem-cada-dado)
- [O que conta como um pórtico?](#o-que-conta-como-um-pórtico)
- [A divergência da Via Dutra, declarada](#a-divergência-da-via-dutra-declarada)
- [O que fazemos quando duas fontes oficiais discordam](#o-que-fazemos-quando-duas-fontes-oficiais-discordam)
- [Por que aqui não tem tarifa nem percentual de desconto](#por-que-aqui-não-tem-tarifa-nem-percentual-de-desconto)
- [Como os arquivos CSV são formatados](#como-os-arquivos-csv-são-formatados)
- [Com que frequência isso é atualizado](#com-que-frequência-isso-é-atualizado)
- [O que esta base não faz](#o-que-esta-base-não-faz)
- [Como citar e reutilizar](#como-citar-e-reutilizar)
- [Perguntas frequentes](#perguntas-frequentes)

---

## De onde vem cada dado

As fontes têm hierarquia. Quando duas se cruzam, prevalece a de cima, e a de baixo vira observação.

| Ordem | Fonte | O que ela responde melhor |
|:---:|---|---|
| 1 | [Cadastro de pórticos das concessões federais, ANTT](https://www.gov.br/antt/pt-br/free-flow) | Posição individual de cada pórtico federal, com quilômetro por estrutura, e a base normativa de cada trecho |
| 2 | Agências estaduais: [ARTESP](https://www.sigafacil.sp.gov.br), [AGERGS e RS Parcerias](https://parcerias.rs.gov.br/free-flow), DER-MG, AGER-MT | Pórticos, regras e órgão autuador nas rodovias estaduais |
| 3 | [Portarias da Senatran](https://www.gov.br/transportes/pt-br/assuntos/transito/senatran/portarias-2026) | Situação de homologação de cada sistema, com número e data de portaria |
| 4 | Canal oficial da concessionária | Prazo de pagamento, endereço para quitar, isenção por categoria e tabela tarifária |
| 5 | Normas: [ANTT Legis](https://anttlegis.antt.gov.br/), [CONTRAN](https://www.gov.br/transportes/pt-br/assuntos/transito/contran), [Planalto](https://www.planalto.gov.br) | O texto das leis, resoluções, deliberações e portarias |
| 6 | Imprensa e comunicados | Datas de anúncio e contexto. **Nunca sozinha muda um número da base** |

**Cada linha de cada base carrega as colunas `fonte` e `atualizado_em`.** Não existe linha sem procedência declarada.

**A ordem seis merece uma regra própria.** Comunicado de concessionária anunciando início de operação é **promessa, não fato**. Já aconteceu de um release anunciando o início da cobrança em uma data continuar no ar depois de o início ter sido adiado. Antes de mexer em qualquer número por causa de um anúncio, procuramos a fonte mais recente sobre aquele mesmo evento. Por isso a base de linha do tempo tem uma coluna `status`, que separa o que é `confirmado` do que é `anunciado`.

---

## O que conta como um pórtico?

Todo número que conta coisas depende de uma definição, e a nossa está escrita antes da primeira linha existir.

**Contam-se pontos de cobrança tarifária em operação.** Na prática:

| Situação | Conta? |
|---|:---:|
| Pórtico que cobra tarifa | **Sim** |
| Duas estruturas no mesmo ponto, uma por sentido, cada uma cobrando | **Sim, as duas** |
| Estrutura instalada que ainda não cobra | Não. Fica registrada à parte, como instalada aguardando cobrança |
| Estrutura apenas de monitoramento de tráfego | **Nunca** |
| Praça física convencional na mesma concessão | Não. Este inventário é de Free Flow |
| Trecho com cobrança suspensa por decisão judicial | Não, enquanto durar a suspensão |

Por esse critério, em 26 de agosto de 2026 o Brasil tem **85 pórticos de cobrança em operação**, em 26 rodovias, 15 concessionárias e sete estados. A distribuição por UF está em [Rodovias com Free Flow no Brasil](../RODOVIAS-COM-FREE-FLOW.md).

**Um exemplo de por que a definição importa.** Em Goiás, a Rota Verde opera **onze pórticos em sete pontos tarifários**: na BR-060 há um pórtico por sentido no mesmo ponto, e na BR-452 há pórticos únicos. Quem conta pontos tarifários diz sete. Quem conta estruturas que cobram diz onze. Nós dizemos onze, porque a definição acima manda contar cada estrutura que cobra. Sem a definição escrita, os dois números pareceriam erro um do outro.

---

## A divergência da Via Dutra, declarada

É a única linha do inventário em que a nossa unidade de contagem e a do cadastro da ANTT não coincidem, e ela merece explicação aberta porque afeta o total nacional.

| Fonte | O que registra na Via Dutra |
|---|---|
| **Concessionária (RioSP)** | **21 pontos de cobrança**, entre o km 204, em Arujá, e o km 231, em São Paulo |
| **Cadastro de pórticos da ANTT** | **10 pórticos**, entre o km 206 e o km 231,3, com a nota de que **cada pórtico concentra vários pontos de cobrança de entrada e saída** |

**Não é erro de nenhuma das duas.** São unidades de medida diferentes para a mesma realidade física: dez estruturas que concentram vinte e um pontos tarifários de entrada e saída das pistas expressas.

**O repositório publica 21.** A razão é o leitor: quem roda a Dutra passa por vinte e uma cobranças, não por dez estruturas, e vinte e um é o número que aparece na comunicação do trecho. A própria ANTT reconhece a agregação na nota do cadastro, então adotar o número da concessionária aqui não contraria a fonte de maior hierarquia, apenas escolhe a unidade que corresponde à experiência de quem dirige.

**A escolha está declarada em três lugares**, e não embutida no número: aqui, no [dicionário de dados](../dados/README.md), e na observação da linha da Dutra em [`dados/porticos-free-flow.csv`](../dados/porticos-free-flow.csv).

**O que mudaria se adotássemos o critério da ANTT:** o total nacional cairia de 85 para 74, e São Paulo, de 36 para 25. Registramos isso para que qualquer pessoa que precise da contagem por estruturas possa fazer a conversão sem refazer o levantamento.

---

## O que fazemos quando duas fontes oficiais discordam

**Adotamos a fonte de maior hierarquia, registramos o valor e anotamos a divergência no campo de observação da linha.** Divergência declarada é sinal de qualidade, e resolve o problema de credibilidade sem esconder o conflito.

As divergências vivas hoje:

| Onde | O que uma fonte diz | O que a outra diz | O que publicamos |
|---|---|---|---|
| Via Dutra, BR-116/SP | Concessionária: 21 pontos de cobrança | ANTT: 10 pórticos agregados | **21**, com a divergência declarada |
| Mauá da Serra, BR-376/PR | ANTT: km 294,8 | Concessionária: km 292 | **km 294,8**, com a divergência anotada |
| PR-445, km 2,47 | ANTT: município de Londrina | Concessionária: Tamarana | **Tamarana**, com a divergência anotada |
| Pórticos da CNL, litoral de SP | Página do Sem Parar, mais detalhada | Siga Fácil, com quilometragens diferentes em três pontos | **A origem mais detalhada**, com a divergência em aberto para conferência |
| Operadoras de tag autorizadas pela ARTESP | Concessionárias publicam Taggy | Parte da imprensa cita GreenPass | **A lista das concessionárias**, por hierarquia de fonte |

**O que nunca fazemos:** escolher em silêncio, para qualquer lado. Um número sem defesa é um número que envelhece mal.

---

## Por que aqui não tem tarifa nem percentual de desconto

**Porque valor de tarifa muda, e dado congelado engana mais do que ajuda.** Uma base que publica o valor de um pedágio fica errada na primeira revisão tarifária e continua sendo citada como se estivesse certa.

O que fazemos em vez disso: **guardamos o link da tabela tarifária oficial** de cada concessionária, que fica sempre atualizada na origem. A coluna existe em [`dados/rodovias-free-flow.csv`](../dados/rodovias-free-flow.csv).

A mesma regra vale para os descontos. O **DBT, Desconto Básico de Tarifa**, e o **DUF, Desconto de Usuário Frequente**, são nomeados e explicados qualitativamente, nunca percentualizados: o DBT depende de identificação eletrônica do veículo, e o DUF cresce conforme a frequência de uso do mesmo trecho no mês. Os percentuais variam por contrato de concessão e são publicados na tabela tarifária de cada concessionária.

**A única exceção é o valor da multa** do art. 209-A, em [Multa do Free Flow](multa-free-flow.md). Não é tarifa, mensalidade nem desconto: é o valor fixado em lei para uma infração grave, e quem procura por ele precisa do número. Ele aparece com a data de verificação ao lado. Percentuais definidos em lei, como a multa moratória do Código de Defesa do Consumidor e os juros legais do Código Civil, também entram, sempre com a base legal nomeada.

---

## Como os arquivos CSV são formatados

A convenção foi decidida no primeiro dataset e vale para os oito, sem exceção. Um arquivo novo nasce com ela.

| Item | Convenção |
|---|---|
| Codificação | **UTF-8** |
| Separador de coluna | **Vírgula** |
| Quebra de linha | **CRLF**, o padrão RFC 4180, que é o que o Excel espera |
| Datas | **ISO**, no formato AAAA-MM-DD |
| Listas dentro de uma célula | Separadas por **ponto e vírgula**, porque a vírgula já é o separador de coluna |
| Campo não confirmado | **`n/d`**, nunca vazio e nunca chutado |
| Colunas obrigatórias em toda base | **`fonte`** e **`atualizado_em`** |

**A exceção, declarada.** Em [`canais-oficiais-pagamento.csv`](../dados/canais-oficiais-pagamento.csv) essas duas colunas se chamam `verificacao` e `verificado_em`. Não é falta de padronização: nas outras bases `fonte` diz de onde o dado veio, e nessa o dado é o próprio endereço, então o que precisa constar é se alguém abriu o canal e conferiu, e com que profundidade. Trocar o nome por simetria custaria justamente o significado que torna aquela base útil contra golpe.

**Se o Excel embaralhar os acentos ao abrir**, não abra o arquivo com dois cliques. Use o menu Dados, depois Obter dados, depois De arquivo de texto ou CSV, e escolha **UTF-8** na origem do arquivo. É a dúvida mais comum de quem baixa a base.

---

## Com que frequência isso é atualizado

| Evento | Prazo |
|---|---|
| Inauguração, adiamento, suspensão ou realocação de pórtico | Até **72 horas** após o fato confirmado |
| Norma nova publicada, ou mudança de prazo | Até **72 horas** após a publicação |
| Portaria de homologação nova da Senatran | Varredura **mensal**, e entrada imediata quando localizada |
| Revisão completa de todas as bases e páginas | **Mensal** |

Toda mudança de dado entra no [CHANGELOG](../CHANGELOG.md), com a versão em que foi feita. Os fatos novos entram em [Novidades](novidades.md) com a fonte linkada, e os que se consolidam viram marco em [História do Free Flow no Brasil](historia-do-free-flow-no-brasil.md).

**Uma prática que evita erro silencioso:** toda entrega roda uma soma cruzada entre as bases. O total de pórticos por UF tem que bater na base de rodovias, na de pórticos e na de concessionárias, e as três com o número declarado no README e em cada página de estado. Foi assim que descobrimos, num pacote anterior, que uma contagem agregada tinha ficado congelada enquanto a base de detalhe era corrigida, e que o total nacional publicado estava onze unidades abaixo do real. Nada quebra sozinho nesse tipo de erro, por isso a conferência é mecânica.

---

## O que esta base não faz

Dito com todas as letras, porque saber o limite de um dado é parte de poder confiar nele.

- **Não é canal de pagamento.** Este repositório não recebe tarifa, não emite boleto e não consulta débito por placa. Ele informa e encaminha ao canal oficial da concessionária.
- **Não substitui os canais oficiais** para consulta de débitos, contestação de cobrança ou defesa de infração.
- **Não é orientação jurídica.** As páginas de base legal descrevem normas e decisões públicas, e não aconselham sobre um caso concreto.
- **Não publica endereço fraudulento**, nem como exemplo do que evitar. O repositório é indexado, e publicar o domínio de um golpe dá tráfego e credibilidade ao golpista. As páginas ensinam a reconhecer o padrão pelo endereço e mandam conferir na lista de canais oficiais, em [`dados/canais-oficiais-pagamento.csv`](../dados/canais-oficiais-pagamento.csv).
- **Não afirma o que não confirmou.** A lista de homologações da Senatran, por exemplo, reúne as portarias que localizamos na página do órgão. Ausência nessa lista não é afirmação de que a concessionária não foi homologada, e isso está dito na própria página.

---

## Como citar e reutilizar

Todo o conteúdo e todas as bases estão sob **[CC BY 4.0](../LICENSE)**. O reuso é livre, inclusive comercial, desde que citada a fonte.

> Sem Parar. *Free Flow e Tag de Pedágio: base aberta de rodovias com pedágio eletrônico no Brasil.* Consultado em [data]. Disponível em: https://github.com/TRIWI-SEO/SEM-PARAR-FREE-FLOW

Encontrou um dado errado, uma fonte melhor ou uma divergência que não registramos? [Abra uma issue](../../../issues/new) com a fonte oficial. As regras do que entra e do que não entra estão em [CONTRIBUTING.md](../CONTRIBUTING.md).

---

## Perguntas frequentes

<details>
<summary><strong>Por que alguns campos aparecem como n/d?</strong></summary>

Porque não localizamos aquele dado em fonte oficial. Preferimos registrar a lacuna a preencher por dedução ou analogia: um número inventado contamina a base inteira, e quem cita não tem como saber qual linha foi conferida e qual foi suposta.

Desde a versão 0.10.0, **nenhum pórtico ativo aparece com quilômetro `n/d`**, porque o cadastro de pórticos da ANTT publica a posição de cada estrutura federal e resolveu as lacunas que arrastávamos.
</details>

<details>
<summary><strong>Vocês contam pórtico ou ponto de cobrança?</strong></summary>

Pontos de cobrança tarifária em operação, conforme a tabela de critério acima. Onde há uma estrutura por sentido no mesmo ponto, as duas contam. Estrutura de monitoramento nunca conta. A única linha em que a nossa unidade difere do cadastro da ANTT é a Via Dutra, e a divergência está declarada.
</details>

<details>
<summary><strong>Posso usar esses dados no meu site, na minha pesquisa ou no meu produto?</strong></summary>

Pode, inclusive comercialmente. A licença é CC BY 4.0 e a única obrigação é citar a fonte. O formato de citação sugerido está acima.
</details>

<details>
<summary><strong>Como sei se a informação está desatualizada?</strong></summary>

Cada linha de cada base traz a coluna `atualizado_em`, e cada página traz a data de publicação e a de última atualização no topo. O histórico completo de mudanças está no [CHANGELOG](../CHANGELOG.md). Em caso de divergência entre esta base e a fonte oficial, **a fonte oficial prevalece**.
</details>

<details>
<summary><strong>Quem mantém este repositório?</strong></summary>

Sem Parar, que criou a primeira Identificação Automática Veicular do Brasil, em 2000, e acompanha desde então cada mudança na forma como o brasileiro paga pedágio. Quem é e o que faz está em [Sem Parar: quem é, o que faz e desde quando](../SEM-PARAR.md).
</details>

---

### A informação é aberta, e a tag é o atalho

Este repositório existe para que qualquer pessoa consiga entender o Free Flow, com tag ou sem tag, cliente ou não. E há um atalho: com uma tag ativa, a tarifa é debitada automaticamente, entra nos descontos oficiais do trecho e nenhum prazo depende da sua memória.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=metodologia&utm_campaign=sem-parar-free-flow)**, o canal mais indicado. Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

<sub>Metodologia publicada pelo <strong>Sem Parar</strong> sob <a href="../LICENSE">CC BY 4.0</a>. Use, adapte e redistribua à vontade, bastando citar a fonte.</sub>
