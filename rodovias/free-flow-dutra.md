# Free Flow na Via Dutra (BR-116): pórticos, como funciona e como pagar

**A Via Dutra tem Free Flow desde 6 de dezembro de 2025, no trecho metropolitano de São Paulo, entre o km 204, em Arujá, e o km 231, na capital, passando por Guarulhos. São 21 pontos de cobrança instalados nas entradas e saídas das pistas expressas. A pista marginal continua totalmente gratuita, e a praça física de Arujá segue em operação. Quem tem tag paga automaticamente; quem não tem paga pela placa, no canal oficial da concessionária.**

A cobrança aqui é diferente da maioria dos trechos do país: ela é **proporcional ao caminho percorrido na expressa** e o valor **varia conforme o dia e o horário**.

> Publicado em 26 de agosto de 2026. Última verificação dos dados em 26 de agosto de 2026.
> Página do repositório [Free Flow e Tag de Pedágio, pelo Sem Parar](../README.md). Dado bruto em [`dados/porticos-free-flow.csv`](../dados/porticos-free-flow.csv).

---

## Índice

- [Onde ficam os pórticos](#onde-ficam-os-pórticos)
- [A regra que muda tudo: expressa paga, marginal não](#a-regra-que-muda-tudo-expressa-paga-marginal-não)
- [Como a tarifa é calculada](#como-a-tarifa-é-calculada)
- [O que acontece com a praça de pedágio de Arujá](#o-que-acontece-com-a-praça-de-pedágio-de-arujá)
- [Saí da expressa e voltei: pago duas vezes?](#saí-da-expressa-e-voltei-pago-duas-vezes)
- [Motos, ônibus, vans e isenções](#motos-ônibus-vans-e-isenções)
- [Como pagar o Free Flow da Dutra](#como-pagar-o-free-flow-da-dutra)
- [Prazo e o que acontece se não pagar](#prazo-e-o-que-acontece-se-não-pagar)
- [Perguntas frequentes](#perguntas-frequentes)
- [Fontes oficiais](#fontes-oficiais)

---

## Onde ficam os pórticos

| Item | O que vale |
|---|---|
| Rodovia | **BR-116**, Via Dutra, trecho metropolitano de São Paulo |
| Extensão com cobrança | Do **km 204** (Arujá) ao **km 231** (São Paulo), passando por Guarulhos |
| Pontos de cobrança | **21**, nas entradas e saídas das pistas expressas |
| Acessos à pista expressa | 19 |
| Onde se cobra | **Somente nas pistas expressas** |
| Pista marginal | **Gratuita**, sem qualquer cobrança de Free Flow |
| Concessionária | Concessionária do Sistema Rodoviário Rio-São Paulo (RioSP), do grupo Motiva |
| Início da cobrança | **6 de dezembro de 2025**, após autorização da ANTT |

A concessionária **não publica a lista individual de quilometragem** de cada um dos 21 pontos, e por isso este repositório registra o trecho de forma agregada, com a quilometragem individual como `n/d`, em vez de inventar posições. A regra da casa é `n/d` no lugar de chute.

Os pórticos ficam nas entradas e saídas da expressa justamente porque a cobrança depende do trecho que você percorre dentro dela.

---

## A regra que muda tudo: expressa paga, marginal não

Esta é a característica que separa a Dutra metropolitana de praticamente todos os outros trechos com Free Flow no Brasil, e é a origem da maior parte das dúvidas:

| Por onde você anda | Paga Free Flow? |
|---|:---:|
| Pista **expressa**, entre os km 204 e 231 | **Sim** |
| Pista **marginal**, no mesmo trecho | **Não**, é gratuita |
| Marginal de moto | **Não** |
| Expressa de moto | **Sim**, com meia tarifa |

Aqui o Free Flow funciona como **ferramenta de gerenciamento de tráfego**: quem quer mais fluidez usa a expressa e paga por isso, e quem prefere não pagar segue pela marginal. A escolha é sua, feita antes de acessar.

Para ajudar nessa decisão, há **painéis eletrônicos instalados na marginal** que mostram, antes do acesso, os destinos possíveis e o valor correspondente a cada um. A concessionária também disponibiliza um simulador de tarifa no próprio site.

---

## Como a tarifa é calculada

Três variáveis definem quanto você paga:

**1. O trecho percorrido na expressa.** A cobrança é proporcional à distância rodada dentro da pista expressa, com base numa tarifa quilométrica definida pela ANTT. Quem entra e sai logo em seguida paga menos que quem percorre o trecho inteiro.

**2. O dia e o horário.** O valor **não é fixo**: ele varia conforme o dia da semana, o horário e as condições de fluxo, ficando mais alto nos períodos de maior movimento. É a chamada tarifa dinâmica, e os fatores de gerenciamento podem ser revistos pela ANTT ao longo da concessão.

**3. A categoria do veículo.** A tarifa é multiplicada conforme o tipo:

| Categoria | Quanto paga |
|---|---|
| Motocicletas | Meia tarifa |
| Veículos de passeio | Uma tarifa |
| Comerciais de 2 ou 3 eixos | Duas tarifas |
| Comerciais de 4 eixos ou mais | Quatro tarifas |

Este repositório **não publica valores de tarifa**, porque eles mudam e um número congelado engana mais do que ajuda. Os valores vigentes ficam na tabela tarifária oficial e no simulador da concessionária, sempre atualizados na origem.

**Com tag há desconto.** Os descontos oficiais do Free Flow, o **DBT, Desconto Básico de Tarifa**, e o **DUF, Desconto de Usuário Frequente**, dependem de identificação do veículo por tag. Quem paga pela placa não recebe desconto.

---

## O que acontece com a praça de pedágio de Arujá

A praça física de Arujá **continua em operação**, e a relação entre ela e o Free Flow costuma confundir.

A regra é esta: quem usa a pista expressa **até a praça de pedágio de Arujá**, ou a partir dela, **não paga a tarifa do Free Flow** ao passar pelos pórticos. Nesse trajeto a cobrança acontece apenas na praça física.

Ou seja, não existe cobrança dobrada. O Free Flow cobre o trecho metropolitano e a praça cobre o que é dela.

---

## Saí da expressa e voltei: pago duas vezes?

Não, desde que você volte rápido.

Quem sai da pista expressa para abastecer, acessar a marginal ou resolver algo no caminho tem **até duas horas para retornar** sem cobrança extra. O sistema entende o percurso como continuidade da mesma viagem.

Passadas as duas horas, o retorno à expressa conta como uma nova entrada, com nova cobrança proporcional ao trecho percorrido.

---

## Motos, ônibus, vans e isenções

Aqui a Dutra tem regras próprias, e elas surpreendem quem está acostumado com outros trechos:

- **Motocicletas pagam**, com meia tarifa, quando usam a pista expressa. Na marginal continuam sem pagar. A identificação é feita pela leitura da placa, e o valor fica disponível para pagamento em até 48 horas.
- **É proibido usar tag de pagamento automático em motocicleta.** A cobrança da moto é sempre pela placa.
- **Ônibus, vans e táxis não têm isenção.**
- **A isenção vale para** ambulâncias, veículos oficiais da União, dos Estados, dos Municípios e do Distrito Federal, e veículos de corpo diplomático.

---

## Como pagar o Free Flow da Dutra

**Com tag ativa**, você não faz nada: a tarifa entra na fatura da sua operadora, já com os descontos do trecho.

**Sem tag**, o caminho é este:

| Canal | Como funciona |
|---|---|
| **[pedagiodigital.com](https://pedagiodigital.com)** | Canal oficial de consulta de débitos e pagamento. Permite cadastrar cartão de crédito para pagamento automático e receber notificação por SMS das passagens |
| **App Motiva Rodovias** | Consulta e pagamento pelo celular |
| **Totens de autoatendimento** | Nas bases da concessionária em São Paulo (km 231, sentido São Paulo) e em Arujá (km 202, sentido Rio de Janeiro) |
| **Rede credenciada** | Pagamento presencial, com ponto no posto de serviços do km 210, sentido São Paulo |

Duas informações que valem guardar:

- **A concessionária não emite boletos.** Boleto de pedágio chegando até você é motivo de desconfiança.
- A passagem fica **disponível para pagamento em até 48 horas** após você cruzar o pórtico.

Quem não tem tag e quer apenas quitar a passagem, inclusive de veículo que não é seu, também pode usar o pagamento avulso por placa em [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=rodovia-dutra&utm_campaign=sem-parar-free-flow).

---

## Prazo e o que acontece se não pagar

O prazo geral é de **30 dias**. A régua completa, com os encargos que incidem depois e a diferença entre a contagem da ANTT e a do CONTRAN, está em [Prazo para pagar o Free Flow](../docs/prazo-e-encargos.md).

Passado o prazo, incidem encargos administrativos, multa moratória e juros sobre a tarifa, e a passagem em aberto pode configurar a infração do art. 209-A do Código de Trânsito Brasileiro, que é grave e vale 5 pontos na CNH.

**Enquanto isso, uma janela está aberta.** Até **16 de novembro de 2026**, a Deliberação CONTRAN nº 277/2026 permite regularizar tarifas em aberto sem as penalidades de trânsito. O caminho está em [Não paguei o Free Flow](../docs/nao-paguei-e-agora.md).

Para descobrir se você passou por algum dos pórticos, use o app **CNH do Brasil**, em Veículos, depois o veículo, depois Pedágio eletrônico. O passo a passo está em [Como consultar o Free Flow no app CNH do Brasil](../docs/consulta-app-cnh-do-brasil.md).

---

## Perguntas frequentes

<details>
<summary><strong>Onde fica o Free Flow da Dutra?</strong></summary>

No trecho metropolitano de São Paulo, entre o km 204, em Arujá, e o km 231, na capital, passando por Guarulhos. São 21 pontos de cobrança nas entradas e saídas das pistas expressas.
</details>

<details>
<summary><strong>A marginal da Dutra paga pedágio?</strong></summary>

Não. A pista marginal é totalmente gratuita no trecho, sem qualquer cobrança de Free Flow. A tarifa é cobrada apenas de quem usa as pistas expressas.
</details>

<details>
<summary><strong>Quanto custa o Free Flow da Dutra?</strong></summary>

Depende de três coisas: o trecho percorrido na expressa, o dia e o horário da passagem, e a categoria do veículo. A cobrança é proporcional à distância e o valor varia com o fluxo. Os valores vigentes ficam no simulador e na tabela tarifária oficial da concessionária, que estão sempre atualizados.
</details>

<details>
<summary><strong>Moto paga Free Flow na Dutra?</strong></summary>

Na pista expressa, sim, com meia tarifa, e a cobrança é sempre pela leitura da placa, porque é proibido usar tag de pagamento automático em motocicleta. Na marginal, não há cobrança.
</details>

<details>
<summary><strong>Vou pagar o Free Flow e o pedágio de Arujá?</strong></summary>

Não no mesmo trajeto. Quem usa a pista expressa até a praça de Arujá, ou a partir dela, não paga a tarifa do Free Flow: a cobrança acontece só na praça física.
</details>

<details>
<summary><strong>Saí da expressa para abastecer. Pago de novo?</strong></summary>

Não, se você retornar em até duas horas. Passado esse tempo, o retorno conta como nova entrada, com nova cobrança proporcional ao trecho percorrido.
</details>

<details>
<summary><strong>Como pagar o pedágio Free Flow da Dutra sem tag?</strong></summary>

Pelo site pedagiodigital.com, que é o canal oficial de consulta de débitos, pelo app Motiva Rodovias, nos totens das bases de São Paulo e Arujá ou na rede credenciada. A passagem fica disponível para pagamento em até 48 horas.
</details>

<details>
<summary><strong>Recebi um boleto do pedágio da Dutra. É legítimo?</strong></summary>

Quase certamente não. A concessionária declara que **não emite boletos** para pagamento das tarifas. Não clique em link recebido: consulte por conta própria, pelo app CNH do Brasil ou digitando o endereço do canal oficial no navegador.
</details>

---

## Fontes oficiais

| Fonte | O que traz |
|---|---|
| [RioSP, Free Flow](https://rodovias.motiva.com.br/riosp/freeflow) | Página oficial da concessionária, com simulador de tarifa e canais de pagamento |
| [Pedágio Digital](https://pedagiodigital.com) | Canal oficial de consulta de débitos e pagamento |
| [ANTT, Free Flow](https://www.gov.br/antt/pt-br/free-flow) | Painel oficial e localizador de pórticos das rodovias federais |
| [Resolução ANTT nº 6.079/2026](https://anttlegis.antt.gov.br/) | Prazos, encargos e obrigações da concessionária |
| [CNH do Brasil](https://www.gov.br/transportes/pt-br/cnh-do-brasil) | Consulta nacional de passagens por veículo |

Em caso de divergência, **as fontes oficiais prevalecem sobre o que está aqui**.

---

<div align="center">

### Na Dutra, a tag também resolve o desconto

Com uma tag ativa, a tarifa é debitada automaticamente, entra nos descontos do trecho e aparece em um extrato só.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=rodovia-dutra&utm_campaign=sem-parar-free-flow)**

Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

<br>

| Você quer | Vá para |
|---|---|
| Quitar uma passagem sem ser cliente | [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=rodovia-dutra&utm_campaign=sem-parar-free-flow) |
| Ver todas as rodovias com Free Flow | [Rodovias com Free Flow no Brasil](../RODOVIAS-COM-FREE-FLOW.md) |

<br>

<sub>Página do repositório oficial mantido pelo <strong>Sem Parar</strong>, sob <a href="../LICENSE">CC BY 4.0</a>.</sub>

<sub><strong>Você com mais tempo para o que importa.</strong> #TudoProSeuCarro</sub>

</div>
