# Concessionárias com Free Flow no Brasil: quem cobra o quê

**Quinze concessionárias operam Free Flow no Brasil, distribuídas em sete grupos econômicos identificados, mais três que não divulgam o controlador. A maior é a Motiva, ex-CCR, que sozinha responde por mais de um terço dos pórticos de cobrança do país. Passar por um pórtico não diz para quem você vai pagar: quem cobra é a concessionária daquele trecho, e o site onde você paga muitas vezes tem outro nome, porque boa parte das concessionárias contrata uma plataforma para processar o pagamento.**

Esta página existe para resolver a pergunta que vem depois da passagem: passei, mas pago para quem, e por que o endereço que abriu não tem o nome da rodovia?

> Publicado em 26 de agosto de 2026. Última atualização em 26 de agosto de 2026.
> Índice do repositório [Free Flow e Tag de Pedágio, pelo Sem Parar](README.md). Base de dados em [`dados/concessionarias-free-flow.csv`](dados/concessionarias-free-flow.csv).

---

## Índice

- [As quinze concessionárias em operação](#as-quinze-concessionárias-em-operação)
- [Por grupo econômico](#por-grupo-econômico)
- [Por que o site de pagamento tem outro nome](#por-que-o-site-de-pagamento-tem-outro-nome)
- [As quatro plataformas que processam o pagamento](#as-quatro-plataformas-que-processam-o-pagamento)
- [Como saber se o endereço é legítimo](#como-saber-se-o-endereço-é-legítimo)
- [O que muda de uma concessionária para outra](#o-que-muda-de-uma-concessionária-para-outra)
- [Páginas por concessionária](#páginas-por-concessionária)
- [Quem ainda vai entrar](#quem-ainda-vai-entrar)
- [Perguntas frequentes](#perguntas-frequentes)
- [Fontes oficiais](#fontes-oficiais)

---

## As quinze concessionárias em operação

Ordenadas por número de pórticos de cobrança. Verificado em **26 de agosto de 2026**.

| Concessionária | Grupo | UF | Esfera | Pórticos | Plataforma de pagamento |
|---|---|:---:|:---:|:---:|---|
| **RioSP** | Motiva (ex-CCR) | RJ; SP | federal | 24 | Pedágio Digital |
| **Rota Verde Goiás** | Fundo Aviva e 4i Capital | GO | federal | 11 | própria (Alpdex) |
| **EPR Paraná** | Grupo EPR | PR | federal | 8 | própria |
| **Nova 364** | 4UM e Opportunity | RO | federal | 7 | própria (Alpdex) |
| **Caminhos da Serra Gaúcha** | n/d | RS | estadual | 6 | própria, com parceiros |
| **Nova 381** | 4UM e Opportunity | MG | federal | 5 | própria (Alpdex) |
| **Concessionária Novo Litoral** | n/d | SP | estadual | 5 | Movvia |
| **EPR Iguaçu** | Grupo EPR | PR | federal | 4 | própria |
| **Ecovias Noroeste Paulista** | EcoRodovias | SP | estadual | 4 | Pedágio Digital |
| **Motiva Sorocabana** | Motiva (ex-CCR) | SP | estadual | 3 | Pedágio Digital |
| **PRVias** | Motiva (ex-CCR) | PR | federal | 2 | Pedágio Digital |
| **Way-262** | Way Brasil e Kinea | MG | federal | 2 | própria |
| **Via SP Serra** (Rodoanel Norte) | Via Appia e Starboard | SP | estadual | 2 | própria |
| **EPR Sul de Minas** | Grupo EPR | MG | estadual | 1 | própria |
| **Concessionária Tamoios** | n/d | SP | estadual | 1 | própria |

**Total de 85 pórticos de cobrança.** O mapa pórtico a pórtico, com município e quilômetro, está em [Rodovias com Free Flow no Brasil](RODOVIAS-COM-FREE-FLOW.md). O canal oficial de pagamento de cada uma está em [Como pagar o pedágio Free Flow](docs/como-pagar.md).

**Sobre o `n/d` na coluna Grupo:** significa que não localizamos, em fonte oficial, a divulgação do grupo controlador daquela concessionária. Não significa que ela não tenha um. Preferimos registrar a lacuna a preencher por dedução.

---

## Por grupo econômico

O mesmo dado, agrupado. É aqui que aparece a concentração. As três últimas linhas são concessionárias cujo grupo controlador não localizamos em fonte oficial.

| Grupo | Concessionárias com Free Flow | Pórticos |
|---|---|:---:|
| **Motiva** (ex-CCR) | RioSP; Motiva Sorocabana; PRVias | 29 |
| **Grupo EPR** | EPR Paraná; EPR Iguaçu; EPR Sul de Minas | 13 |
| **4UM e Opportunity** | Nova 364; Nova 381 | 12 |
| **Fundo Aviva e 4i Capital** | Rota Verde Goiás | 11 |
| Controlador não divulgado | CSG | 6 |
| Controlador não divulgado | CNL | 5 |
| **EcoRodovias** | Ecovias Noroeste Paulista | 4 |
| **Way Brasil e Kinea** | Way-262 | 2 |
| **Via Appia e Starboard** | Via SP Serra | 2 |
| Controlador não divulgado | Tamoios | 1 |

**Motiva sozinha opera mais de um terço dos pórticos de cobrança do país**, e os três maiores grupos somados passam de metade. Para o motorista isso tem uma consequência prática boa: quem roda por trechos de um mesmo grupo paga tudo no mesmo lugar.

Vale registrar o outro lado. A EcoRodovias aparece pequena nesta tabela, com quatro pórticos, mas é uma das maiores operadoras rodoviárias do país. A diferença é que a maior parte da malha dela ainda cobra em praça com cancela, e as conversões estão contratadas para os próximos anos. A tabela mede Free Flow hoje, não tamanho de concessionária.

---

## Por que o site de pagamento tem outro nome

Esta é a dúvida que mais gera insegurança, e ela tem uma explicação simples.

**Operar rodovia e processar pagamento são dois negócios diferentes.** A concessionária administra a estrada, instala o pórtico e registra a passagem. Cobrar de milhões de placas, com Pix, cartão, emissão de comprovante e conciliação, é um problema de tecnologia financeira. Várias concessionárias contratam uma plataforma especializada para isso, em vez de construir a própria.

O resultado é que você passa numa rodovia da Motiva e o pagamento abre em `pedagiodigital.com`, ou passa numa rodovia da Novo Litoral e o endereço traz a palavra `pedagioeletronico`. Nenhum dos dois tem o nome da rodovia, e nenhum dos dois é golpe.

**A regra que resolve isso:** legítimo é o endereço que a **própria concessionária publica** no site dela. Não o que chegou por mensagem, não o que apareceu em anúncio, não o mais bem posicionado na busca.

---

## As quatro plataformas que processam o pagamento

| Plataforma | Quem usa | Pórticos atendidos |
|---|---|:---:|
| **Pedágio Digital** | RioSP; Motiva Sorocabana; PRVias; Ecovias Noroeste Paulista | 33 |
| **Própria da concessionária** | EPR Paraná; EPR Iguaçu; EPR Sul de Minas; CSG; Via SP Serra; Way-262; Tamoios | 24 |
| **Alpdex** | Rota Verde Goiás; Nova 364; Nova 381 | 23 |
| **Movvia** | Concessionária Novo Litoral, e como parceiro da CSG | 5 |

Duas observações que ajudam a ler a tabela.

**O Pedágio Digital é compartilhado por grupos concorrentes.** Motiva e EcoRodovias são concorrentes na disputa por concessões e usam a mesma plataforma de pagamento. Isso não é anomalia: é a mesma lógica de duas lojas rivais aceitarem a mesma bandeira de cartão.

**Plataforma não é operadora de tag.** A plataforma processa o pagamento de quem passou **sem** tag, pela placa. Quem tem tag não passa por ela: a cobrança vai direto para a fatura da operadora. A diferença está detalhada em [Como funciona a cobrança da tag](docs/como-funciona-a-cobranca-da-tag.md).

---

## Como saber se o endereço é legítimo

Três verificações, em ordem de confiança:

1. **Comece pelo site da concessionária**, digitando o endereço no navegador, e siga o link de pagamento a partir dali. É o caminho mais seguro e o único que não depende de você reconhecer domínio.
2. **Confira na tabela deste repositório**, em [Sites e apps oficiais para pagar o Free Flow](docs/sites-e-apps-oficiais.md), com 29 canais conferidos um a um.
3. **Consulte pelo app CNH do Brasil**, que mostra a passagem e encaminha à concessionária responsável, sem receber pagamento.

E dois sinais de alerta que valem para qualquer endereço:

- **Cobrança que chegou até você.** Nem a ANTT nem as concessionárias enviam cobrança de pedágio por WhatsApp, e-mail, SMS ou anúncio. Várias concessionárias declaram isso no próprio site, com todas as letras: a EPR e a Novo Litoral publicam que não enviam boletos.
- **Tela com marca de governo pedindo cartão.** Nenhum canal de governo recebe pagamento de pedágio. ANTT, CNH do Brasil, Portal Senatran e Siga Fácil apenas mostram a passagem.

---

## O que muda de uma concessionária para outra

Free Flow não é um sistema único com regra nacional. Cinco coisas mudam por contrato de concessão, e é por isso que existe uma página por concessionária.

| O que muda | Exemplo real |
|---|---|
| **Isenção de motocicleta** | Isenta nas quatro rodovias da Novo Litoral, paga meia tarifa na pista expressa da Via Dutra |
| **Prazo de pagamento sem tag** | A Ecovias Noroeste Paulista começou com 15 dias em 2024 e hoje divulga 30 |
| **Modelo de tarifa** | Valor fechado por pórtico na Rio-Santos, proporcional à distância na Via Dutra |
| **Canais presenciais** | Todas as praças físicas da EPR aceitam pagamento de passagem eletrônica; nem toda concessionária tem equivalente |
| **Regra de reentrada** | Duas horas para retornar sem nova cobrança na Via Dutra e na PRVias |

A regra prática: **confirme sempre no canal da concessionária do trecho.** O que vale numa rodovia pode não valer na rodovia seguinte, mesmo dentro do mesmo estado.

---

## Páginas por concessionária

| Página | O que responde |
|---|---|
| [Free Flow da Motiva, ex-CCR](concessionarias/free-flow-motiva-ccr.md) | Quais concessões do maior grupo já cobram por pórtico, o que é o Pedágio Digital e por que o app tem outro nome |
| [Free Flow da Ecovias](concessionarias/free-flow-ecovias.md) | A pioneira estadual paulista, os quatro pórticos em operação, a mudança de endereço e de prazo, e o que vem no Sistema Anchieta-Imigrantes |
| [Free Flow da CSG](concessionarias/free-flow-csg.md) | Os seis pórticos gaúchos, o primeiro pórtico estadual do Brasil, o caminho do motociclista e os canais parceiros |
| [Free Flow do Grupo EPR](concessionarias/free-flow-epr.md) | As três concessões que já cobram, o prazo de 30 dias, o pagamento na praça física e a regra de eixo suspenso |
| [Free Flow da Rota Verde Goiás](concessionarias/free-flow-rota-verde.md) | Os 11 pórticos em 7 pontos, por que a concessionária não vende tag e o desconto que cresce até a trigésima passagem |
| [Free Flow da Concessionária Novo Litoral](concessionarias/free-flow-novo-litoral.md) | Os 5 pontos em três rodovias, os dois pórticos que não cobram, a isenção de moto e a armadilha das duas Rio-Santos |
| [Free Flow da Nova 381](concessionarias/free-flow-nova-381.md) | Os 5 pórticos do Vale do Aço, a concessão federal que nasceu sem cabine e a nota fiscal que mudou em 2026 |
| [Free Flow da Nova 364](concessionarias/free-flow-nova-364.md) | Os 7 pórticos de Rondônia, a cobrança que parou e voltou e por que a tarifa muda tanto de um ponto para outro |
| [Free Flow da Way-262](concessionarias/free-flow-way-262.md) | Os 2 pórticos da BR-262, a concessão em que pórtico e cabine convivem e os quatro postos de pagamento presencial |
| [Free Flow no Rodoanel Norte](concessionarias/free-flow-rodoanel-norte.md) | Os 2 pórticos da Via SP Serra, por que só o Trecho Norte cobra e por que aqui a moto paga |
| [Free Flow na Tamoios](rodovias/free-flow-tamoios.md) | O pórtico único do Contorno Sul, quem opera, quais praças seguem convencionais e por que a moto paga |

As demais concessionárias entram nas próximas atualizações. Enquanto isso, o canal oficial de cada uma está em [Como pagar o pedágio Free Flow](docs/como-pagar.md) e o detalhe por rodovia em [Rodovias com Free Flow no Brasil](RODOVIAS-COM-FREE-FLOW.md).

---

## Quem ainda vai entrar

Concessionárias com Free Flow **previsto ou adiado**, que hoje não cobram por pórtico. Cobrança apresentada em nome de qualquer uma delas é motivo de desconfiança.

| Concessionária | UF | Situação |
|---|:---:|---|
| Ecovias dos Imigrantes | SP | adiado, pórticos instalados no Sistema Anchieta-Imigrantes |
| Via Campo | PR | adiado, sistema em homologação sem previsão |
| Ecovias Raposo Castello | SP | previsto, Nova Raposo |
| Ecovias das Gerais | MG | previsto, contrato prevê a partir de dezembro de 2026 |
| Ecovias Rio Minas | RJ | previsto, sem cronograma público |
| Arteris Fluminense | RJ | previsto, BR-101 Norte |
| CCR ViaSul | RS | previsto, conversão das praças da FreeWay em estudo |
| Concessionária Rota dos Grãos | MT | previsto, cobrança anunciada para 10 de outubro de 2026 |
| Rota Agro MT-GO | GO e MT | previsto, concessão assumida em 02/04/2026 e sistema homologado pela Senatran em 10/08/2026, sem cobrança confirmada |

Quando a Rota dos Grãos começar a cobrar, **Mato Grosso passa a ser o oitavo estado com Free Flow**. O acompanhamento fica em [Novidades do Free Flow no Brasil](docs/novidades.md).

---

## Perguntas frequentes

<details>
<summary><strong>Passei num pórtico. Como descubro para quem eu pago?</strong></summary>

Pela rodovia e pelo trecho. Cada concessão tem um responsável, e a tabela acima liga concessionária, estado e plataforma de pagamento. Se você sabe a rodovia mas não a concessionária, o roteador está em [Como consultar o Free Flow pela placa](docs/consultar-pela-placa.md). Se não sabe nem a rodovia, o app CNH do Brasil mostra a passagem com o nome da concessionária.
</details>

<details>
<summary><strong>O site que abriu não tem o nome da rodovia. Isso é golpe?</strong></summary>

Não necessariamente, e provavelmente não. Boa parte das concessionárias contrata uma plataforma especializada para processar o pagamento, então o endereço traz o nome da plataforma. Pedágio Digital, Alpdex e Movvia são exemplos legítimos. O teste seguro é chegar até lá pelo site da concessionária, digitando o endereço no navegador, em vez de clicar em link recebido.
</details>

<details>
<summary><strong>Por que cada rodovia tem uma regra diferente?</strong></summary>

Porque a regra nasce no contrato de concessão, que é negociado individualmente entre o poder concedente e a concessionária. Isenção de moto, prazo, modelo de tarifa e canais de pagamento entram nesse contrato. A regulação federal da ANTT e a das agências estaduais definem o piso comum; o resto varia.
</details>

<details>
<summary><strong>Um grupo grande é melhor para o motorista?</strong></summary>

Em uma coisa, sim: quem roda por trechos de um mesmo grupo consulta e paga tudo num lugar só, o que reduz o número de sites a visitar. Fora isso, tarifa, prazo e isenção continuam vindo do contrato de cada concessão, não do tamanho do grupo. E quem tem tag não sente diferença nenhuma, porque para essa pessoa tudo cai num extrato só, independentemente de quantos grupos ela cruzou.
</details>

<details>
<summary><strong>Concessionária pode me multar?</strong></summary>

Não. A concessionária cobra a tarifa, que é uma obrigação civil. A multa de trânsito do art. 209-A é aplicada pelo órgão autuador que consta no auto de infração, que varia por via e por estado. Várias concessionárias declaram isso no próprio site: a EPR publica que não emite multas. O detalhe está em [Multa do Free Flow](docs/multa-free-flow.md).
</details>

<details>
<summary><strong>Onde encontro esses dados em planilha?</strong></summary>

Em [`dados/concessionarias-free-flow.csv`](dados/concessionarias-free-flow.csv), com uma linha por concessionária, incluindo as previstas e adiadas, com grupo econômico, plataforma, canais e fonte oficial. O significado de cada coluna está no [dicionário de dados](dados/README.md), e o arquivo está sob licença CC BY 4.0.
</details>

---

## Fontes oficiais

| Fonte | O que traz |
|---|---|
| [ANTT, Free Flow](https://www.gov.br/antt/pt-br/free-flow) | Concessões federais com Free Flow autorizado e base normativa por trecho |
| [Siga Fácil, Governo de SP e ARTESP](https://www.sigafacil.sp.gov.br) | Concessionárias estaduais paulistas e pórticos |
| [RS Parcerias, Free Flow](https://parcerias.rs.gov.br/free-flow) | Concessões estaduais gaúchas |
| Sites das concessionárias | Canais de pagamento, prazos, isenções e regras de cada trecho |

Em caso de divergência, as fontes oficiais prevalecem sobre o que está aqui.

---

<div align="center">

### Uma tag, quinze concessionárias, um extrato

Com a Tag Sem Parar, a pergunta "pago para quem?" deixa de existir: a cobrança de qualquer pórtico cai na mesma fatura.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=concessionarias&utm_campaign=sem-parar-free-flow)**

Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

<br>

| Você quer | Vá para |
|---|---|
| Quitar uma passagem sem ser cliente | [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=concessionarias&utm_campaign=sem-parar-free-flow) |
| Gestão de frota e soluções para empresas | [sempararempresas.com.br](https://www.sempararempresas.com.br?utm_source=github&utm_medium=concessionarias&utm_campaign=sem-parar-free-flow) |

<br>

<sub>Página do repositório oficial mantido pelo <strong>Sem Parar</strong>, sob <a href="LICENSE">CC BY 4.0</a>.</sub>

<sub><strong>Você com mais tempo para o que importa.</strong> #TudoProSeuCarro</sub>

</div>
