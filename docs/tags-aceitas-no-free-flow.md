# Quais tags funcionam no Free Flow: a lista por concessionária

**Todas as 15 concessionárias com Free Flow ativo no Brasil aceitam tag. Nas rodovias federais concedidas a aceitação é obrigatória por lei: qualquer tag autorizada pela ANTT é lida por qualquer pórtico federal, por força da interoperabilidade prevista na Lei nº 14.157/2021. Nas rodovias estaduais vale a lista da agência reguladora do estado, e em São Paulo as concessionárias publicam cinco operadoras autorizadas pela ARTESP: ConectCar, Move Mais, Sem Parar, Taggy e Veloe.**

Em resumo: não existe hoje pórtico de Free Flow em operação no país que recuse tag. O que muda de um trecho para outro é a lista de operadoras aceitas e as regras de desconto.

> Publicado em 26 de agosto de 2026. Última atualização em 26 de agosto de 2026.
> Parte do repositório [Free Flow e Tag de Pedágio, pelo Sem Parar](../README.md). Base de dados em [`dados/tags-aceitas-free-flow.csv`](../dados/tags-aceitas-free-flow.csv).

---

## Índice

- [A regra muda conforme quem regula a rodovia](#a-regra-muda-conforme-quem-regula-a-rodovia)
- [Tabela de aceitação por concessionária](#tabela-de-aceitação-por-concessionária)
- [As cinco operadoras autorizadas pela ARTESP](#as-cinco-operadoras-autorizadas-pela-artesp)
- [Uma divergência que vale registrar](#uma-divergência-que-vale-registrar)
- [Onde a tag não entra](#onde-a-tag-não-entra)
- [Como saber se a sua tag foi lida](#como-saber-se-a-sua-tag-foi-lida)
- [Perguntas frequentes](#perguntas-frequentes)
- [Fontes oficiais](#fontes-oficiais)

---

## A regra muda conforme quem regula a rodovia

Existem dois regimes, e eles respondem a perguntas diferentes.

**Rodovia federal concedida, regulada pela ANTT.** A interoperabilidade é obrigatória. As operadoras de tag são autorizadas pela própria ANTT, sob a sigla **AMAP**, Administradora de Meios de Pagamento para Arrecadação de Pedágio, criada pela Resolução ANTT nº 4.281/2014. Autorizada a operadora, todas as concessionárias federais precisam ler a tag dela. Por isso a maioria das concessionárias federais não publica lista própria: não faz sentido publicar uma lista que a norma já define.

**Rodovia estadual, regulada pela agência do estado.** A autorização é estadual, e a lista pode ser menor. Em São Paulo é a ARTESP; no Rio Grande do Sul, a AGERGS; em Minas Gerais, o DER-MG.

Uma consequência prática, e pouco óbvia: **a mesma tag pode ser aceita numa rodovia federal e não constar na lista de um estado.** Na prática isso hoje não gera problema para as cinco maiores operadoras, mas é o motivo pelo qual esta página existe trecho a trecho, e não como uma frase única.

A Resolução ANTT nº 6.079/2026, no art. 63-D, foi além e deixou explícito que o usuário pode optar entre os sistemas de pagamento das empresas autorizadas pela ANTT, os sistemas próprios das concessionárias e os sistemas interoperáveis entre concessionárias. Ou seja: a tag é um caminho, não o único.

---

## Tabela de aceitação por concessionária

Todas as concessionárias com Free Flow **em operação**, ordenadas por esfera. Gerada a partir de [`dados/tags-aceitas-free-flow.csv`](../dados/tags-aceitas-free-flow.csv), verificada em **26 de agosto de 2026**.

| Concessionária | UF | Regulador | Aceita tag | Operadoras publicadas | Descontos por tag |
|---|:---:|:---:|:---:|---|:---:|
| **RioSP** (Via Dutra e Rio-Santos) | RJ; SP | ANTT | sim | interoperabilidade federal | DBT; DUF |
| **Nova 381** (BR-381) | MG | ANTT | sim | interoperabilidade federal | DBT; DUF |
| **Way-262** (BR-262) | MG | ANTT | sim | interoperabilidade federal | n/d |
| **Nova 364** (BR-364) | RO | ANTT | sim | interoperabilidade federal | DBT; DUF |
| **EPR Iguaçu** (BR-163, PR-182, PR-280) | PR | ANTT | sim | interoperabilidade federal | DBT; DUF |
| **EPR Paraná** (BR-369, BR-376) | PR | ANTT | sim | interoperabilidade federal | DBT; DUF |
| **PRVias** (BR-376, PR-445) | PR | ANTT | sim | interoperabilidade federal | DBT; DUF |
| **Rota Verde Goiás** (BR-060, BR-452) | GO | ANTT | sim | interoperabilidade federal | DBT; DUF |
| **Concessionária Novo Litoral** (SP-055, SP-088, SP-098) | SP | ARTESP | sim | ConectCar; Move Mais; Sem Parar; Taggy; Veloe | DBT; DUF |
| **Concessionária Tamoios** (SP-099) | SP | ARTESP | sim | ConectCar; Move Mais; Sem Parar; Taggy; Veloe | n/d |
| **Ecovias Noroeste Paulista** (SP-326, SP-333) | SP | ARTESP | sim | lista da ARTESP | DBT; DUF |
| **Motiva Sorocabana** (SP-270) | SP | ARTESP | sim | lista da ARTESP | n/d |
| **Via SP Serra** (Rodoanel Norte, SP-021) | SP | ARTESP | sim | lista da ARTESP | n/d |
| **Caminhos da Serra Gaúcha** (ERS-122, ERS-240, ERS-446) | RS | AGERGS | sim | lista da AGERGS | DBT; DUF |
| **EPR Sul de Minas** (MG-459) | MG | DER-MG | sim | lista do DER-MG | DBT; DUF |

**Como ler a coluna "Operadoras publicadas".** "Interoperabilidade federal" significa que a aceitação decorre da norma da ANTT e a concessionária não publica lista própria. "Lista da ARTESP", "lista da AGERGS" e "lista do DER-MG" significam que vale a lista da agência reguladora e a concessionária não a reproduz no próprio site. Nomes de operadora só aparecem quando a **própria concessionária** os publica.

**Sobre `n/d` na coluna de descontos:** significa que a concessionária não publica de forma explícita quais descontos aplica ao usuário de tag, e não que não haja desconto. Nenhum percentual foi registrado aqui: eles mudam por contrato e ficam na tabela tarifária oficial de cada concessionária, linkada em [`dados/rodovias-free-flow.csv`](../dados/rodovias-free-flow.csv).

---

## As cinco operadoras autorizadas pela ARTESP

Duas concessionárias paulistas publicam a lista completa no próprio site, e elas coincidem:

| Operadora | Site oficial |
|---|---|
| ConectCar | [conectcar.com](https://www.conectcar.com) |
| Move Mais | [movemais.com](https://www.movemais.com) |
| Sem Parar | [semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=tags-aceitas&utm_campaign=sem-parar-free-flow) |
| Taggy | [taggy.com.br](https://www.taggy.com.br) |
| Veloe | [veloe.com.br](https://www.veloe.com.br) |

Publicar a lista de concorrentes aqui é deliberado. Este repositório serve à pergunta do motorista, não ao catálogo de um fornecedor, e a resposta correta para "minha tag funciona nesse pórtico?" precisa incluir todas as tags.

---

## Uma divergência que vale registrar

Nem todas as fontes publicam a mesma lista de cinco.

- As concessionárias **Novo Litoral** e **Tamoios** publicam, cada uma no próprio site: ConectCar, Move Mais, Sem Parar, Taggy e Veloe.
- Parte da cobertura de imprensa e alguns materiais de terceiros citam **GreenPass** no lugar de Taggy.

Adotamos a lista publicada pelas próprias concessionárias, que são a fonte de maior hierarquia sobre o que os pórticos delas leem, e registramos a divergência em vez de escondê-la. Se você usa uma operadora que não aparece na lista do trecho, o caminho seguro é confirmar com a sua operadora antes da viagem, e não presumir.

---

## Onde a tag não entra

Três situações em que a tag simplesmente não é o caminho, mesmo em rodovia que a aceita:

**Motocicleta.** Nenhuma tag no Brasil é homologada para moto. Onde o trecho cobra de moto, como na pista expressa da Via Dutra, no Rodoanel Norte e no Contorno Sul da Tamoios, o pagamento é sempre pela placa. A Via Dutra é explícita: proibido o uso de qualquer tag de pagamento automático em motocicleta. Nas quatro rodovias da Concessionária Novo Litoral a questão não se coloca, porque motos são isentas. O assunto completo está em [Tag em moto, carro alugado e segundo veículo](tag-em-moto-e-outros-veiculos.md).

**Tag inativa ou sem saldo.** Se a leitura falhar por irregularidade cadastral ou falta de saldo, o pórtico recorre à placa e a tarifa volta a ser paga por você, no canal da concessionária, dentro do prazo. A Tamoios descreve exatamente esse fluxo no próprio site.

**Passagem anterior à tag.** Débito registrado antes da ativação continua vinculado à placa. A tag não retroage. O caminho está em [Não paguei o Free Flow](nao-paguei-e-agora.md).

---

## Como saber se a sua tag foi lida

Três lugares, nesta ordem:

1. **Extrato da sua operadora**, no app ou no site. É onde a passagem por tag aparece, com data, rodovia e valor.
2. **App CNH do Brasil**, em Veículos, depois Pedágio eletrônico. Ele mostra a situação da passagem, que pode aparecer como paga quando a tag capturou. O passo a passo está em [Como consultar o Free Flow no app CNH do Brasil](consulta-app-cnh-do-brasil.md).
3. **Portal da concessionária**, pela placa. Aqui vale lembrar: passagem capturada por tag em regra **não** aparece, porque esse portal lista o que está em aberto.

Se a passagem não aparecer em nenhum dos três depois de alguns dias, é caso de contestação. O caminho está em [Como funciona a cobrança da tag](como-funciona-a-cobranca-da-tag.md).

---

## Perguntas frequentes

<details>
<summary><strong>Minha tag funciona em todos os pórticos de Free Flow do Brasil?</strong></summary>

Nas rodovias federais concedidas, sim, desde que a operadora seja autorizada pela ANTT: a interoperabilidade é obrigatória e o padrão técnico é o mesmo em toda a malha federal. Nas estaduais, a aceitação depende da lista da agência reguladora do estado. Hoje, as cinco operadoras autorizadas pela ARTESP cobrem todos os pórticos estaduais paulistas em operação. A Tag Sem Parar é aceita em 100% das rodovias pedagiadas do país.
</details>

<details>
<summary><strong>Preciso avisar a concessionária que tenho tag?</strong></summary>

Não. O cadastro fica com a sua operadora de tag, e é ela que se comunica com o sistema de arrecadação da concessionária. Você não precisa cadastrar placa em site de rodovia. Cadastro no site da concessionária é o caminho de quem paga **sem** tag, e em alguns casos, como na CSG, também o caminho de quem quer desconto sem poder usar tag.
</details>

<details>
<summary><strong>Existe alguma rodovia com Free Flow que só aceita placa?</strong></summary>

Hoje, não. As 15 concessionárias com Free Flow em operação aceitam tag. Vale a ressalva de que a lista muda rápido: pórtico novo entra e concessionária nova assume trecho. Este repositório é atualizado em até 72 horas depois de cada mudança confirmada.
</details>

<details>
<summary><strong>A tag me dá desconto em qualquer trecho?</strong></summary>

Nas concessões federais, DBT e DUF são previstos no regulamento da ANTT e dependem de identificação eletrônica do veículo. Nas estaduais, o desconto por tag existe onde o contrato de concessão prevê, e varia. A coluna de descontos da tabela acima registra o que cada concessionária publica. Percentuais não ficam aqui de propósito: eles mudam, e o número correto está sempre na tabela tarifária oficial.
</details>

<details>
<summary><strong>Uso vale-pedágio. Ele vale no Free Flow?</strong></summary>

Depende do formato. A CSG, no Rio Grande do Sul, declara aceitar vale-pedágio apenas no formato tag. Desde 2025, aliás, o Vale-Pedágio Obrigatório só existe em meio eletrônico: cartões, cupons e outros meios físicos foram descontinuados pela regulamentação da ANTT. Se você é transportador ou embarcador, o caminho é [sempararempresas.com.br](https://www.sempararempresas.com.br?utm_source=github&utm_medium=tags-aceitas&utm_campaign=sem-parar-free-flow).
</details>

<details>
<summary><strong>Onde encontro esses dados em planilha?</strong></summary>

Em [`dados/tags-aceitas-free-flow.csv`](../dados/tags-aceitas-free-flow.csv), com uma linha por concessionária e fonte oficial em cada uma. O significado de cada coluna está no [dicionário de dados](../dados/README.md). O arquivo está sob licença CC BY 4.0: use, adapte e redistribua, inclusive comercialmente, citando a fonte.
</details>

---

## Fontes oficiais

| Fonte | O que traz |
|---|---|
| [ANTT, Free Flow](https://www.gov.br/antt/pt-br/free-flow) | Interoperabilidade nas federais e autorização das AMAPs |
| [Resolução ANTT nº 4.281/2014](https://anttlegis.antt.gov.br/) | Define a AMAP e padroniza a arrecadação eletrônica |
| [Resolução ANTT nº 6.079/2026](https://anttlegis.antt.gov.br/) | Art. 63-D, opções de meio de pagamento no sistema de livre passagem |
| [Siga Fácil, Governo de SP e ARTESP](https://www.sigafacil.sp.gov.br) | Free Flow nas estaduais paulistas |
| [Free Flow Tamoios](https://freeflowtamoios.com.br) | Lista de operadoras autorizadas pela ARTESP |
| [Concessionária Novo Litoral](https://novolitoral.com.br/pedagio-eletronico) | Lista de operadoras aceitas e regras de desconto |
| [CSG, dúvidas sobre o Free Flow](https://www.csg.com.br/noticias/csg-esclarece-principais-duvidas-sobre-o-free-flow) | Tag, cadastro sem tag e vale-pedágio no Bloco 3 gaúcho |
| [RioSP, dúvidas frequentes](https://rodovias.motiva.com.br/riosp/central-de-ajuda/duvidas-frequentes) | Pagamento com e sem tag na Via Dutra e na Rio-Santos |

Em caso de divergência, as fontes oficiais prevalecem sobre o que está aqui.

---

<div align="center">

### Uma tag aceita em 100% das rodovias pedagiadas

Com a Tag Sem Parar, a pergunta "minha tag funciona nesse pórtico?" deixa de existir, nas praças com cancela e nos pórticos de Free Flow.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=tags-aceitas&utm_campaign=sem-parar-free-flow)**

Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

<br>

| Você quer | Vá para |
|---|---|
| Quitar uma passagem sem ser cliente | [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=tags-aceitas&utm_campaign=sem-parar-free-flow) |
| Gestão de frota e soluções para empresas | [sempararempresas.com.br](https://www.sempararempresas.com.br?utm_source=github&utm_medium=tags-aceitas&utm_campaign=sem-parar-free-flow) |

<br>

<sub>Página do repositório oficial mantido pelo <strong>Sem Parar</strong>, sob <a href="../LICENSE">CC BY 4.0</a>.</sub>

<sub><strong>Você com mais tempo para o que importa.</strong> #TudoProSeuCarro</sub>

</div>
