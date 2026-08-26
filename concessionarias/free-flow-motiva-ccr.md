# Free Flow da Motiva, ex-CCR: rodovias, pórticos e como pagar

**A Motiva, nome atual do grupo CCR, é a maior operadora de Free Flow do Brasil: 29 dos 85 pórticos de cobrança do país, distribuídos por três concessões. São elas a RioSP, com a pista expressa da Via Dutra e a Rio-Santos no Rio de Janeiro; a Motiva Sorocabana, na Raposo Tavares; e a PRVias, no Paraná. Quem passa sem tag por qualquer uma delas paga no mesmo lugar, o portal Pedágio Digital, em `pedagiodigital.com`, ou pelo app Motiva Rodovias.**

Se você procurou por "CCR free flow" e chegou aqui, é esta a informação: a marca mudou para Motiva, o sistema é o mesmo e o pagamento é centralizado.

> Publicado em 26 de agosto de 2026. Última atualização em 26 de agosto de 2026.
> Parte do repositório [Free Flow e Tag de Pedágio, pelo Sem Parar](../README.md). Índice em [Concessionárias com Free Flow](../CONCESSIONARIAS-FREE-FLOW.md).

---

## Índice

- [CCR virou Motiva: o que mudou e o que não mudou](#ccr-virou-motiva-o-que-mudou-e-o-que-não-mudou)
- [Onde a Motiva cobra por pórtico](#onde-a-motiva-cobra-por-pórtico)
- [Como pagar sem tag](#como-pagar-sem-tag)
- [As três regras próprias que vale conhecer](#as-três-regras-próprias-que-vale-conhecer)
- [Com tag, você não faz nada](#com-tag-você-não-faz-nada)
- [Perguntas frequentes](#perguntas-frequentes)
- [Fontes oficiais](#fontes-oficiais)

---

## CCR virou Motiva: o que mudou e o que não mudou

O grupo CCR passou a se chamar **Motiva**. As concessionárias mantiveram os nomes de operação, agora com a assinatura "uma empresa Motiva", e os sites migraram para o domínio `rodovias.motiva.com.br`.

Para quem dirige, **nada mudou na prática**: os mesmos pórticos, as mesmas tarifas aprovadas pela agência reguladora, os mesmos canais de pagamento. O que muda é o nome que aparece na placa, no site e no aplicativo, e é isso que gera a dúvida de quem procura por "CCR" e encontra "Motiva".

O grupo reúne 13 concessionárias rodoviárias. **Três delas já cobram por pórtico**, e é o que esta página cobre.

---

## Onde a Motiva cobra por pórtico

Verificado em **26 de agosto de 2026**.

| Concessão | Rodovia e trecho | UF | Pórticos | Desde |
|---|---|:---:|:---:|:---:|
| **RioSP** | BR-116 Via Dutra, pista expressa entre Arujá (km 204) e São Paulo (km 231) | SP | 21 | 06/12/2025 |
| **RioSP** | BR-101 Rio-Santos, Itaguaí (km 414), Mangaratiba (km 447) e Paraty (km 538) | RJ | 3 | 31/03/2023 |
| **Motiva Sorocabana** | SP-270 Raposo Tavares, São Roque (km 48), Alumínio (km 83) e Araçoiaba da Serra (km 111) | SP | 3 | 01/10/2025 |
| **PRVias** | BR-376 Rodovia do Café, Mauá da Serra (km 294,8) | PR | 1 | 01/06/2026 |
| **PRVias** | PR-445 Celso Garcia Cid, Tamarana (km 2,47) | PR | 1 | 01/06/2026 |

**Total de 29 pórticos de cobrança**, mais de um terço do total nacional.

Duas marcas históricas estão aqui. A **Rio-Santos foi o primeiro Free Flow em rodovia federal do Brasil**, em março de 2023. E a **Via Dutra é o maior trecho contínuo com cobrança proporcional** do país, com 21 pontos em 27 quilômetros de pista expressa.

A Motiva Sorocabana opera ainda **cinco pórticos apenas de monitoramento** na SP-270, que não cobram tarifa. Cobrança apresentada em nome deles é motivo de desconfiança. Eles estão registrados em [`dados/porticos-free-flow.csv`](../dados/porticos-free-flow.csv).

O detalhe rodovia a rodovia está em [Free Flow na Via Dutra](../rodovias/free-flow-dutra.md) e [Free Flow na Rio-Santos](../rodovias/free-flow-rio-santos.md).

---

## Como pagar sem tag

As três concessões usam a mesma plataforma, o **Pedágio Digital**, e o mesmo aplicativo de grupo.

| Canal | Endereço | Observação |
|---|---|---|
| **Site** | [pedagiodigital.com](https://pedagiodigital.com) | Domínio terminado em `.com`, não `.com.br`. Alvo frequente de imitação |
| **App** | Motiva Rodovias | Consulta automática por veículo cadastrado, sem informar data e hora da passagem |
| **App** | Pedágio Digital | O mesmo portal, em aplicativo |
| **WhatsApp** | 0800-017-3536, opção 4 do menu | Canal da RioSP |
| **Totens e rede credenciada** | Na BR-101 Rio-Santos | Ver abaixo |

Na **Rio-Santos**, o pagamento presencial funciona em totens em Ubatuba (km 31,8), Mangaratiba (km 417,4), Angra dos Reis (km 471,45 e km 528) e Paraty (km 580), além da rede credenciada no Auto Posto Velamar, em Paraty (km 533+800), e no Itacuruçá Plaza Hotel, em Mangaratiba.

O valor da passagem fica disponível para pagamento em **até 48 horas**, e o prazo geral é de **30 dias**. As formas aceitas são Pix e cartão de crédito.

> **Atenção ao domínio.** O endereço oficial é `pedagiodigital.com`, sem `.br` no fim. É um dos alvos mais imitados por sites falsos de pedágio, justamente porque não carrega o nome de nenhuma rodovia. As próprias concessionárias da Motiva mantêm uma seção de alerta de golpes no site. A lista verificada de canais legítimos está em [Sites e apps oficiais para pagar o Free Flow](../docs/sites-e-apps-oficiais.md).

---

## As três regras próprias que vale conhecer

**1. Na Via Dutra, só a pista expressa cobra.** A pista marginal continua gratuita, para todos os veículos. E quem usa a praça física de Arujá e depois segue pela expressa **não paga duas vezes**.

**2. Existe janela de reentrada.** Na Via Dutra, quem retorna em até **duas horas** não paga nova cobrança. A PRVias tem regra equivalente: passagem pelos dois pórticos no mesmo sentido em até duas horas gera cobrança única. É a regra que evita punir quem faz o mesmo trajeto de ida e volta no mesmo turno.

**3. Motocicleta na Dutra paga, e não pode usar tag.** Na pista expressa, a moto paga meia tarifa, e a concessionária declara **proibido o uso de qualquer tag de pagamento automático em motocicleta**. Na marginal, a moto não paga nada. Já na Rio-Santos, no Rio de Janeiro, motos, motonetas, triciclos e bicicletas são **isentos**. O assunto completo está em [Tag em moto, carro alugado e segundo veículo](../docs/tag-em-moto-e-outros-veiculos.md).

E uma quarta, que desmente uma crença comum: **ônibus, vans e táxis não são isentos** no Free Flow da Dutra. A isenção vale para ambulâncias, veículos oficiais e corpo diplomático.

---

## Com tag, você não faz nada

Nas três concessões, tag ativa significa cobrança automática na fatura da sua operadora, com os descontos do trecho aplicados, e nenhum prazo para controlar. A Motiva Sorocabana publica o Desconto Básico de Tarifa para quem usa tag; a RioSP informa faixas de desconto que variam bastante conforme frequência e trecho.

Os percentuais mudam por contrato e ficam na tabela tarifária oficial de cada concessionária. Este repositório não guarda percentual nenhum, de propósito.

Uma consequência que confunde: **a passagem cobrada por tag em regra não aparece no Pedágio Digital**, porque aquele portal lista o que está em aberto. O registro fica no extrato da sua operadora. O detalhe está em [Como funciona a cobrança da tag](../docs/como-funciona-a-cobranca-da-tag.md).

---

## Perguntas frequentes

<details>
<summary><strong>CCR e Motiva são a mesma empresa?</strong></summary>

Sim. O grupo CCR passou a se chamar Motiva, e as concessionárias mantiveram os nomes de operação com a assinatura "uma empresa Motiva". Os sites migraram para `rodovias.motiva.com.br`. Para quem dirige, nada muda: mesmos pórticos, mesmas tarifas, mesmos canais.
</details>

<details>
<summary><strong>Como pagar o Free Flow da CCR sem tag?</strong></summary>

Pelo site `pedagiodigital.com`, pelo app Motiva Rodovias, pelo app Pedágio Digital, pelo WhatsApp 0800-017-3536 na opção 4, ou presencialmente nos totens e na rede credenciada da BR-101. O valor fica disponível em até 48 horas após a passagem e o prazo é de 30 dias. Aceita Pix e cartão de crédito.
</details>

<details>
<summary><strong>Pago pedágio na Dutra mesmo passando pela marginal?</strong></summary>

Não. O Free Flow da Via Dutra cobra apenas de quem usa a **pista expressa** entre o km 204, em Arujá, e o km 231, em São Paulo. A pista marginal continua gratuita. Essa é a diferença mais importante do trecho e a origem de boa parte das dúvidas.
</details>

<details>
<summary><strong>O Free Flow substituiu as praças da Dutra?</strong></summary>

Não. As praças físicas da Via Dutra seguem em operação, inclusive a de Arujá. O Free Flow foi implantado nas pistas expressas do trecho metropolitano, e quem passa pela praça e depois segue pela expressa não paga cobrança dobrada.
</details>

<details>
<summary><strong>O site pedagiodigital.com é confiável?</strong></summary>

É o canal oficial, publicado pelas próprias concessionárias da Motiva e também usado pela Ecovias. O cuidado necessário é com o endereço: termina em `.com`, sem `.br`, e não carrega o nome de nenhuma rodovia, o que o torna alvo frequente de imitação. O caminho mais seguro é chegar até ele pelo site da concessionária, digitando o endereço no navegador.
</details>

<details>
<summary><strong>A RioSP é a mesma coisa que CCR RioSP?</strong></summary>

Sim, é a Concessionária do Sistema Rodoviário Rio-São Paulo, hoje identificada como "uma empresa Motiva". Ela opera a Via Dutra e a Rio-Santos, e é a concessionária com mais pórticos de Free Flow do país, com 24.
</details>

---

## Fontes oficiais

| Fonte | O que traz |
|---|---|
| [RioSP, Free Flow](https://rodovias.motiva.com.br/riosp/freeflow) | Pórticos, canais de pagamento, totens e rede credenciada |
| [RioSP, dúvidas frequentes](https://rodovias.motiva.com.br/riosp/central-de-ajuda/duvidas-frequentes) | Pagamento com e sem tag, prazo e disponibilização em 48 horas |
| [Motiva Sorocabana, Pedágio Eletrônico](https://rodovias.motiva.com.br/sorocabana/pedagio-eletronico) | Funcionamento e canais na SP-270 |
| [Pedágio Digital](https://pedagiodigital.com) | Consulta e pagamento por placa |
| [ANTT, Free Flow](https://www.gov.br/antt/pt-br/free-flow) | Base normativa das concessões federais |

Em caso de divergência, as fontes oficiais prevalecem sobre o que está aqui.

---

<div align="center">

### Três concessões, um extrato só

Com a Tag Sem Parar, a cobrança da Dutra, da Rio-Santos, da Raposo e do Paraná cai na mesma fatura, com os descontos do trecho aplicados.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=concessionaria-motiva&utm_campaign=sem-parar-free-flow)**

Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

<br>

| Você quer | Vá para |
|---|---|
| Quitar uma passagem sem ser cliente | [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=concessionaria-motiva&utm_campaign=sem-parar-free-flow) |
| Gestão de frota e soluções para empresas | [sempararempresas.com.br](https://www.sempararempresas.com.br?utm_source=github&utm_medium=concessionaria-motiva&utm_campaign=sem-parar-free-flow) |

<br>

<sub>Página do repositório oficial mantido pelo <strong>Sem Parar</strong>, sob <a href="../LICENSE">CC BY 4.0</a>.</sub>

<sub><strong>Você com mais tempo para o que importa.</strong> #TudoProSeuCarro</sub>

</div>
