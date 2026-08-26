# Free Flow da Concessionária Novo Litoral: SP-055, SP-088, SP-098 e como pagar

**A Concessionária Novo Litoral, a CNL, opera 5 pontos de cobrança de Free Flow em três rodovias do litoral e do alto Tietê paulista: a SP-055, a SP-088 e a SP-098. A cobrança começou em 1º de novembro de 2025 e a concessão nasceu 100% eletrônica, sem nenhuma cabine. Quem tem tag não faz nada. Quem não tem paga em até 30 dias corridos no portal, no aplicativo ou presencialmente nas oito bases de atendimento. Motocicletas são isentas em todas as rodovias da concessão.**

Um detalhe que evita susto e é explorado por golpistas: **dois pórticos da concessão, em Itariri, não cobram nada.** Eles existem só para monitorar tráfego.

> Publicado em 26 de agosto de 2026. Última atualização em 26 de agosto de 2026.
> Parte do repositório [Free Flow e Tag de Pedágio, pelo Sem Parar](../README.md). Base de dados em [`dados/porticos-free-flow.csv`](../dados/porticos-free-flow.csv).

---

## Índice

- [Quem é a Concessionária Novo Litoral](#quem-é-a-concessionária-novo-litoral)
- [Onde a CNL cobra por pórtico](#onde-a-cnl-cobra-por-pórtico)
- [Os dois pórticos que não cobram](#os-dois-pórticos-que-não-cobram)
- [Como pagar sem tag](#como-pagar-sem-tag)
- [Moto é isenta nas três rodovias](#moto-é-isenta-nas-três-rodovias)
- [Por que o site de pagamento tem outro nome](#por-que-o-site-de-pagamento-tem-outro-nome)
- [A armadilha das duas Rio-Santos](#a-armadilha-das-duas-rio-santos)
- [Com tag, você não faz nada](#com-tag-você-não-faz-nada)
- [Perguntas frequentes](#perguntas-frequentes)
- [Fontes oficiais](#fontes-oficiais)

---

## Quem é a Concessionária Novo Litoral

Concessionária **estadual paulista**, regulada pela **ARTESP**, responsável por um conjunto de rodovias que liga a região metropolitana de São Paulo ao litoral sul e à Baixada Santista. O controlador não é divulgado em fonte oficial que possamos citar, e preferimos registrar a lacuna a preencher por dedução.

A cobrança integra o **Siga Fácil**, nome do programa de Free Flow das rodovias estaduais paulistas, conduzido pelo Governo de São Paulo e pela ARTESP. O processamento do pagamento roda em plataforma de terceiro, a **Movvia**, e é daí que vem o endereço oficial `cnl.pedagioeletronico.com.br`.

**É a primeira concessão 100% eletrônica de São Paulo**: não existe praça com cabine em nenhuma das rodovias. O panorama do estado está em [Free Flow em São Paulo](../estados/free-flow-sp.md).

---

## Onde a CNL cobra por pórtico

| Rodovia | Nome | Município | km |
|---|---|---|---|
| **SP-088** | Pedro Eroles (Mogi-Dutra) | Arujá | 37+150 norte e 37+780 sul |
| **SP-088** | Pedro Eroles (Mogi-Dutra) | Mogi das Cruzes | 41+600 norte e 40+800 sul |
| **SP-098** | Dom Paulo Rolim Loureiro (Mogi-Bertioga) | Bertioga | 92+740 |
| **SP-055** | Manoel Hipólito do Rego | Santos | 236+000 |
| **SP-055** | Padre Manoel da Nóbrega | Miracatu | 389+560 |

**Cinco pontos de cobrança.** Os valores de tarifa mudam com o reajuste e não são publicados aqui: consulte a tabela oficial da concessionária, sempre atualizada na origem.

> **Divergência registrada.** O portal Siga Fácil publica quilometragens diferentes das da concessionária em três destes pontos, e chega a listar Santos numa quilometragem que corresponde a Bertioga. Adotamos a fonte mais detalhada e mantemos a divergência declarada, conforme a regra descrita em [Metodologia e fontes](../docs/metodologia-e-fontes.md). Para o motorista isso não muda nada: o ponto de cobrança é o mesmo, e o pagamento também.

A página dedicada ao trecho da serra está em [Free Flow na Mogi-Bertioga](../rodovias/free-flow-mogi-bertioga.md).

---

## Os dois pórticos que não cobram

Na **SP-055, em Itariri**, existem duas estruturas de pórtico, nos km 369+860 e 360+200, que **não cobram tarifa**. Elas operam apenas como monitoramento de tráfego.

Isso importa por dois motivos. O primeiro é que passar por elas não gera cobrança nenhuma, e ver o pórtico não significa ter uma passagem a pagar. O segundo é de segurança: **cobrança apresentada como sendo de Itariri é motivo de desconfiança**. Todos os pórticos do país que existem mas não cobram estão registrados em [`dados/porticos-free-flow.csv`](../dados/porticos-free-flow.csv), com o status separado.

---

## Como pagar sem tag

O pórtico lê a placa e a passagem fica disponível para quitação. **O prazo é de até 30 dias corridos após a passagem**, conforme a concessionária publica.

| Onde | Como funciona |
|---|---|
| **Portal oficial** | [cnl.pedagioeletronico.com.br](https://cnl.pedagioeletronico.com.br), consulta pela placa e pagamento |
| **Aplicativo** | Mesma conta do portal, com acompanhamento de passagens e valores |
| **Oito bases de atendimento** | Pagamento presencial no totem, com crédito, débito ou Pix |
| **Conta com saldo** | Dá para deixar crédito e ter as passagens baixadas automaticamente |

Quem tem tag tem o prazo definido pelo contrato com a operadora, e não por este de 30 dias. A distinção está em [Como funciona a cobrança da tag](../docs/como-funciona-a-cobranca-da-tag.md).

> **A CNL não envia cobrança por mensagem.** Não existe boleto automático de Free Flow nem site único nacional de consulta. Quem inicia o pagamento é você, digitando o endereço no navegador. Ver [Golpe do falso pedágio](../docs/golpe-do-falso-pedagio.md).

---

## Moto é isenta nas três rodovias

**Motocicletas têm isenção total nas rodovias da concessão.** Vale para a SP-055, a SP-088 e a SP-098, sem cadastro e sem pedido.

É uma regra diferente da que vale a poucos quilômetros dali: na pista expressa da Via Dutra a moto paga meia tarifa, no Rodoanel Norte paga e no Contorno Sul da Tamoios paga. **A isenção de moto não é regra nacional**, ela está no contrato de cada concessão. A tabela trecho a trecho está em [Tag em moto, carro alugado e segundo veículo](../docs/tag-em-moto-e-outros-veiculos.md).

---

## Por que o site de pagamento tem outro nome

Quem passa por um pórtico da CNL e procura onde pagar chega a um endereço que não tem o nome da rodovia nem o da concessionária. Não é golpe, e a explicação é simples.

Boa parte das concessionárias brasileiras **contrata uma plataforma** para processar o pagamento das passagens, e o nome dessa plataforma é o que aparece no endereço. No caso da CNL, a plataforma é a **Movvia**, e o endereço oficial é um subdomínio dela.

**A regra que resolve qualquer dúvida:** legítimo é o endereço que a própria concessionária publica nos canais dela. Todos os canais verificados um a um estão em [Sites e apps oficiais para pagar o Free Flow](../docs/sites-e-apps-oficiais.md) e no dado bruto em [`dados/canais-oficiais-pagamento.csv`](../dados/canais-oficiais-pagamento.csv). Quem opera o quê no país inteiro está em [Concessionárias com Free Flow no Brasil](../CONCESSIONARIAS-FREE-FLOW.md).

---

## A armadilha das duas Rio-Santos

**Existem duas rodovias chamadas Rio-Santos, e elas têm concessionárias, regras e canais de pagamento diferentes.**

| Qual | Onde | Quem opera | Moto |
|---|---|---|---|
| **SP-055**, Manoel Hipólito do Rego | São Paulo | Concessionária Novo Litoral | Isenta |
| **BR-101**, Costa Verde | Rio de Janeiro | RioSP, do grupo Motiva | Isenta |

As duas isentam moto, mas por contratos diferentes, e **o canal de pagamento não é o mesmo**. Pagar no portal errado não quita a sua passagem. A do Rio está em [Free Flow na Rio-Santos](../rodovias/free-flow-rio-santos.md).

---

## Com tag, você não faz nada

O pórtico identifica a tag, a tarifa cai na fatura da sua operadora e o prazo deixa de ser problema seu. A concessionária divulga desconto para quem paga com tag ativa, e o percentual fica publicado no canal oficial dela, porque muda com o tempo.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=novo-litoral&utm_campaign=sem-parar-free-flow)**, o canal mais indicado. Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

---

## Perguntas frequentes

<details>
<summary><strong>Quantos pórticos a Novo Litoral tem?</strong></summary>

Cinco pontos de cobrança, em três rodovias: dois na SP-088 (Arujá e Mogi das Cruzes), um na SP-098 (Bertioga) e dois na SP-055 (Santos e Miracatu). Existem ainda dois pórticos em Itariri, na SP-055, que apenas monitoram tráfego e não cobram.
</details>

<details>
<summary><strong>Qual o prazo para pagar sem tag?</strong></summary>

Até 30 dias corridos após a passagem, conforme a concessionária publica. Com tag, o prazo é o do seu contrato com a operadora. Depois do prazo incidem encargos, e a passagem em aberto pode configurar infração de trânsito. Veja [Prazo para pagar o Free Flow](../docs/prazo-e-encargos.md).
</details>

<details>
<summary><strong>Moto paga na Mogi-Bertioga ou na Rio-Santos paulista?</strong></summary>

Não. Motocicletas são isentas em todas as rodovias da Concessionária Novo Litoral, sem necessidade de cadastro.
</details>

<details>
<summary><strong>Passei em Itariri e não achei a cobrança. Está errado?</strong></summary>

Não. Os dois pórticos de Itariri, nos km 369+860 e 360+200 da SP-055, operam apenas como monitoramento de tráfego e não cobram tarifa. Não há o que pagar ali.
</details>

<details>
<summary><strong>O site cnl.pedagioeletronico.com.br é oficial?</strong></summary>

Sim. É o endereço que a própria concessionária publica, num subdomínio da plataforma que ela contratou para processar os pagamentos. A lista completa de canais verificados está em [Sites e apps oficiais](../docs/sites-e-apps-oficiais.md).
</details>

<details>
<summary><strong>Tem praça de pedágio com cabine nas rodovias da CNL?</strong></summary>

Não. A concessão nasceu 100% eletrônica e é a primeira de São Paulo nessa condição. Toda a cobrança acontece por pórtico.
</details>

---

## Fontes oficiais

| Fonte | O que traz |
|---|---|
| [CNL, pedágio eletrônico](https://cnl.pedagioeletronico.com.br) | Consulta por placa, pagamento, prazo e bases de atendimento |
| [Siga Fácil, Governo de SP e ARTESP](https://www.sigafacil.sp.gov.br) | Free Flow nas rodovias estaduais paulistas |
| [Sem Parar, Novo Litoral](https://www.semparar.com.br/novo-litoral-cnl) | Detalhamento dos pontos de cobrança da concessão |

Em caso de divergência, as fontes oficiais prevalecem sobre o que está aqui. Como cada dado foi levantado está em [Metodologia e fontes](../docs/metodologia-e-fontes.md).

Viu algo desatualizado? [Abra uma issue](../../../issues/new) com a fonte.

---

### Do alto Tietê à Baixada, numa fatura só

Quem desce a serra no fim de semana ou roda o trecho Mogi, Bertioga e Santos atravessa mais de um ponto de cobrança na mesma viagem. Com uma tag ativa, tudo cai na mesma fatura e nenhum prazo depende da sua memória.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=novo-litoral&utm_campaign=sem-parar-free-flow)**

Passou e não é cliente? Dá para quitar só aquela passagem, pela placa, em [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=novo-litoral&utm_campaign=sem-parar-free-flow).

<sub>Página publicada pelo <strong>Sem Parar</strong> sob <a href="../LICENSE">CC BY 4.0</a>. Use, adapte e redistribua à vontade, bastando citar a fonte.</sub>
