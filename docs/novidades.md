# Novidades do Free Flow no Brasil (atualização contínua)

**Esta é a linha do tempo do pedágio eletrônico brasileiro: cada mudança confirmada em pórtico, prazo ou regra entra aqui com data, resumo e fonte oficial linkada.** As notas ficam em ordem do mais recente para o mais antigo. Mudanças de status de rodovia entram em até 72 horas após o fato confirmado, e a base de dados é corrigida no mesmo movimento.

> Última verificação em 26 de agosto de 2026.
> Parte do repositório [Free Flow e Tag de Pedágio, pelo Sem Parar](../README.md). Termos técnicos estão no [glossário](glossario.md).

---

## O que está valendo agora, em três linhas

1. **85 pórticos de cobrança em operação**, em 26 rodovias, 15 concessionárias e 7 estados: GO, MG, PR, RJ, RO, RS e SP.
2. **O prazo de regularização sem penalidade de trânsito termina em 16 de novembro de 2026.** A tarifa continua devida.
3. **O app CNH do Brasil já mostra passagens de Free Flow**, de rodovias federais, estaduais e municipais integradas.

---

## 2026

### 24 de agosto de 2026: o app CNH do Brasil passa a mostrar passagens de Free Flow

O Ministério dos Transportes liberou no app **CNH do Brasil** a consulta integrada das passagens de Free Flow registradas para o veículo, em rodovias federais, estaduais e municipais integradas ao sistema. O caminho no app é Veículos, depois o veículo, depois Pedágio eletrônico. A consulta estreou com **14 concessionárias integradas**, mostra placa, data e local, valor, concessionária, prazo e situação, permite **contestar** uma passagem e envia dois alertas, um em até 24 horas após a passagem e outro cinco dias antes do vencimento. O histórico alcança os últimos cinco anos. O app **não recebe pagamento**: ele identifica a concessionária responsável e encaminha ao canal dela. Pessoas físicas também podem consultar pelo **Portal de Serviços Senatran**, com mais detalhe, e frotas e empresas consultam **exclusivamente** por ele.

A escala ajuda a entender as lacunas: segundo o Ministério e o Serpro, a solução foi construída em três meses, com 27 organizações envolvidas, e já processou mais de 200 milhões de registros de passagem do passivo do sistema, com cerca de 10 milhões de novas passagens só em agosto de 2026.

Na mesma comunicação, o Ministério confirmou o marco de **17 de novembro de 2026**: a partir dessa data, tarifas não quitadas dentro do prazo regulamentar voltam a poder gerar auto de infração, com os processos administrativos seguindo o curso regular previsto no Código de Trânsito Brasileiro.

Fonte: [Ministério dos Transportes](https://www.gov.br/transportes/pt-br/assuntos/noticias-/2026/08/app-cnh-do-brasil-oferece-consulta-ao-free-flow-a-partir-desta-segunda-24) e [Serpro](https://www.serpro.gov.br/menu/noticias/noticias-2026/free-flow). Afeta: [Como consultar o Free Flow no app CNH do Brasil](consulta-app-cnh-do-brasil.md), [Como consultar pela placa](consultar-pela-placa.md) e [`dados/canais-oficiais-pagamento.csv`](../dados/canais-oficiais-pagamento.csv).

### 24 de agosto de 2026: MT-130 anuncia início do Free Flow para 10 de outubro

A concessionária **Rota dos Grãos** anunciou o início da cobrança eletrônica na **MT-130, entre Primavera do Leste e Paranatinga**, para **10 de outubro de 2026**. O projeto substitui as duas praças físicas do trecho por **seis pórticos** distribuídos ao longo dos cerca de 140 quilômetros da rodovia, com cobrança proporcional ao trecho efetivamente percorrido. Até lá não há cobrança por pórtico na MT-130, e o portal oficial de consulta e pagamento da concessionária já está no ar.

Quando a operação começar, Mato Grosso passa a ser o **oitavo estado** com Free Flow ativo no país. A rodovia entra agora na base com status `previsto`.

Fonte: [Rota dos Grãos, portal de pedágio eletrônico](https://pedagioeletronico.rotadosgraos130.com.br). Afeta: [`dados/rodovias-free-flow.csv`](../dados/rodovias-free-flow.csv) e [`dados/concessionarias-free-flow.csv`](../dados/concessionarias-free-flow.csv).

### 27 de julho de 2026: Sistema Anchieta-Imigrantes adiado, sem nova data

O Governo de São Paulo adiou o início da operação do Free Flow no **Sistema Anchieta-Imigrantes**, que estava previsto para 1º de agosto de 2026, e não divulgou nova data. A reprogramação decorre da determinação de que o ponto de cobrança no sentido Capital da Rodovia dos Imigrantes fique **depois do km 38**, e não no km 29, para preservar deslocamentos locais. As praças físicas seguem em operação normal enquanto isso.

Este é hoje o adiamento mais relevante do país, porque envolve o corredor de acesso à Baixada Santista. Enquanto não houver nova data, **não existe cobrança por pórtico na Anchieta nem na Imigrantes**, e qualquer cobrança que se apresente como tal merece desconfiança.

Fonte: [G1 Santos e Região](https://g1.globo.com/sp/santos-regiao/noticia/2026/07/27/governo-de-sp-adia-inicio-do-pedagio-eletronico-no-sistema-anchieta-imigrantes-entenda.ghtml) e [Siga Fácil](https://www.sigafacil.sp.gov.br). Afeta: [Free Flow no Sistema Anchieta-Imigrantes](../rodovias/free-flow-anchieta-imigrantes.md), [`dados/rodovias-free-flow.csv`](../dados/rodovias-free-flow.csv) e [`dados/porticos-free-flow.csv`](../dados/porticos-free-flow.csv).

### 19 de julho de 2026: o pórtico da Imigrantes sentido capital é realocado

A Secretaria de Parcerias em Investimentos do Estado de São Paulo e a **ARTESP** anunciaram a realocação do pórtico da **Rodovia dos Imigrantes no sentido capital**, do km 29 para um ponto mais próximo do trecho de serra, **depois do km 38**. A decisão veio após manifestação de moradores da região do Pós-Balsa, em São Bernardo do Campo, que apontaram que deslocamentos curtos e cotidianos entre bairros gerariam cobrança repetida ao longo do dia.

É essa redefinição que motivou o adiamento anunciado oito dias depois. O ponto exato segue em definição.

Fonte: [Siga Fácil](https://www.sigafacil.sp.gov.br). Afeta: [Free Flow no Sistema Anchieta-Imigrantes](../rodovias/free-flow-anchieta-imigrantes.md) e [`dados/porticos-free-flow.csv`](../dados/porticos-free-flow.csv).

### 1º de junho de 2026: PRVias inicia cobrança na Rodovia do Café e na PR-445

A **PRVias**, do grupo Motiva, começou a cobrar por pórtico na **BR-376, Rodovia do Café, em Mauá da Serra**, e na **PR-445, em Tamarana**. São dois pórticos de cobrança, com pagamento pela plataforma Pedágio Digital. O cadastro da ANTT e a comunicação da concessionária divergem na quilometragem do pórtico da BR-376, e a divergência está anotada na base.

Fonte: [ANTT, Free Flow](https://www.gov.br/antt/pt-br/free-flow). Afeta: [`dados/rodovias-free-flow.csv`](../dados/rodovias-free-flow.csv).

### 27 de maio de 2026: Rota Verde inicia o maior trecho contínuo de Goiás

A **Rota Verde Goiás** iniciou a cobrança eletrônica na **BR-060 e na BR-452**, do Anel Viário de Goiânia ao Contorno de Rio Verde e de Rio Verde a Itumbiara, somando **11 pórticos** em 7 pontos de cobrança e mais de 400 quilômetros de rodovia. É a maior operação de Free Flow do Centro-Oeste.

Fonte: [ANTT, Free Flow](https://www.gov.br/antt/pt-br/free-flow). Afeta: [`dados/rodovias-free-flow.csv`](../dados/rodovias-free-flow.csv).

### 4 de maio de 2026: EPR Paraná ativa oito pórticos no norte e noroeste

A **EPR Paraná** iniciou a cobrança na **BR-369**, em Jataizinho e Rolândia, e na **BR-376**, em Mandaguaçu e Marialva, com oito pórticos no total. O pagamento é feito no portal de pedágio eletrônico da família EPR.

Fonte: [ANTT, Free Flow](https://www.gov.br/antt/pt-br/free-flow). Afeta: [`dados/rodovias-free-flow.csv`](../dados/rodovias-free-flow.csv).

### 29 de abril de 2026: a Deliberação CONTRAN nº 277 muda a contagem do prazo e abre a regularização

Publicada no Diário Oficial da União em 29 de abril de 2026, a **Deliberação CONTRAN nº 277, de 26 de março de 2026**, fez três coisas ao mesmo tempo, e a segunda passou despercebida na cobertura de imprensa.

1. **Abriu um prazo excepcional de 200 dias**, até **16 de novembro de 2026**, para regularizar tarifas de Free Flow **sem as penalidades de trânsito**. No período não se configura a infração do art. 209-A do Código de Trânsito Brasileiro pelo não pagamento. Quitar dentro do prazo cancela os processos de infração correspondentes e exclui penalidade e pontuação, e quem já tinha pago a multa pode pedir revisão e restituição.
2. **Alterou o art. 7º da Resolução CONTRAN nº 1.013/2024.** O prazo de 30 dias, que era contado da data da passagem, passou a ser contado **da confirmação do processamento do registro da passagem** junto ao órgão máximo executivo de trânsito da União. Para as passagens feitas durante o regime de transição, prevalece o prazo mais favorável ao usuário entre os dois.
3. **Deu 100 dias para a homologação dos sistemas** de livre passagem junto à Senatran. Sistema não homologado não pode ser usado para os fins do art. 115, § 10, do Código de Trânsito Brasileiro, o que afasta a infração do art. 209-A, conforme a Portaria Senatran nº 442/2025.

A tarifa continua devida em qualquer cenário. A partir de **17 de novembro de 2026** a regra ordinária volta a valer integralmente.

Fonte: [Deliberação CONTRAN nº 277/2026](https://www.gov.br/transportes/pt-br/assuntos/transito/conteudo-contran/deliberacoes/Deliberacao2772026.pdf) e [Resolução CONTRAN nº 1.013/2024](https://www.gov.br/transportes/pt-br/assuntos/transito/conteudo-contran/resolucoes/Resolucao10132024.pdf). Afeta: [Como pagar](como-pagar.md#quanto-tempo-eu-tenho-para-pagar) e [O que é Free Flow](../O-QUE-E-FREE-FLOW.md#quanto-tempo-tenho-para-pagar).

### 27 de março de 2026: publicada a Resolução ANTT nº 6.079/2026

A ANTT publicou a resolução que **regulamenta o sistema de livre passagem** nas rodovias federais concedidas, com entrada em vigor prevista para até 120 dias após a publicação. Ela alterou as quatro normas do Regulamento das Concessões Rodoviárias e trouxe a régua financeira completa do Free Flow federal:

- **Prazo de 30 dias**, contados da passagem pelo pórtico, sem incidência de encargos, multas ou juros.
- **Depois dos 30 dias**, incidem encargos administrativos (limitados ao ressarcimento dos custos de identificação e notificação, sujeitos à aprovação da ANTT), **multa moratória de 2%**, com base no art. 52, § 1º, do Código de Defesa do Consumidor, e **juros legais de 1% ao mês** pro rata temporis, com base nos arts. 395, 397 e 406 do Código Civil, além da penalidade do art. 209-A do Código de Trânsito Brasileiro.
- **Pagar a multa não exime** de quitar a tarifa, os encargos, a moratória e os juros.
- **Cobrança indevida se devolve em dobro**, em até 7 dias corridos.
- **Múltiplos meios de pagamento obrigatórios**, incluindo Pix, cartões, dinheiro e sistemas automáticos, com opção de pagamento pós-passagem disponível em até 2 horas para 90% das passagens e em até 24 horas para 99%.
- **Transações armazenadas por cinco anos**, com obrigação de fornecer o histórico para instruir defesa ou recurso.

Fonte: [ANTT Legis](https://anttlegis.antt.gov.br/) e [ANTT, nota sobre a regulamentação](https://www.gov.br/antt/pt-br/assuntos/ultimas-noticias/antt-consolida-regulamentacao-do-pedagio-sem-cancela-com-foco-na-protecao-ao-usuario-e-na-seguranca-do-sistema). Afeta: [Prazo e encargos](prazo-e-encargos.md), [O que é Free Flow](../O-QUE-E-FREE-FLOW.md#quanto-tempo-tenho-para-pagar) e o [glossário](glossario.md#r).

### 23 de fevereiro de 2026: EPR Iguaçu começa a cobrar no oeste e sudoeste do Paraná

A **EPR Iguaçu** iniciou a cobrança na **BR-163**, em Santa Lúcia, na **PR-182**, em Ampére, e na **PR-280**, em Vitorino, com quatro pórticos.

Fonte: [ANTT, Free Flow](https://www.gov.br/antt/pt-br/free-flow). Afeta: [`dados/rodovias-free-flow.csv`](../dados/rodovias-free-flow.csv).

### 12 de janeiro de 2026: Nova 364 leva o Free Flow a Rondônia

A **Nova 364** iniciou a cobrança na **BR-364**, entre Porto Velho e a divisa com Mato Grosso, com **sete pórticos** ao longo de 686,7 quilômetros. É a operação de Free Flow com maior extensão contínua do país.

Fonte: [ANTT, Free Flow](https://www.gov.br/antt/pt-br/free-flow). Afeta: [`dados/rodovias-free-flow.csv`](../dados/rodovias-free-flow.csv).

---

## 2025

### 23 de dezembro de 2025: Rodoanel Norte passa a cobrar por pórtico

A **Via SP Serra** iniciou a cobrança no **Trecho Norte do Rodoanel Mário Covas**, em Guarulhos, com um pórtico por sentido no km 135. É uma das primeiras operações do programa Siga Fácil, do Governo de São Paulo.

Fonte: [Siga Fácil](https://www.sigafacil.sp.gov.br). Afeta: [`dados/rodovias-free-flow.csv`](../dados/rodovias-free-flow.csv).

### 6 de dezembro de 2025: Via Dutra ativa o trecho metropolitano

A **RioSP**, do grupo Motiva, iniciou a cobrança eletrônica na **BR-116, Via Dutra**, entre o **km 204**, em Arujá, e o km 231, em São Paulo, passando por Guarulhos, com **21 pontos de cobrança** nas entradas e saídas das pistas expressas. A marginal segue gratuita e a praça física de Arujá continua em operação. É o trecho com Free Flow de maior demanda de busca do país, e a cobrança aqui é proporcional ao trecho percorrido, com tarifa que varia por dia e horário.

Fonte: [ANTT, Free Flow](https://www.gov.br/antt/pt-br/free-flow). Afeta: [`dados/rodovias-free-flow.csv`](../dados/rodovias-free-flow.csv).

### 12 de junho de 2025: Portaria Senatran nº 442 cria a homologação obrigatória

A Senatran publicou a portaria que estabelece os **procedimentos de homologação** dos sistemas de livre passagem e de **interoperabilidade** dos dados de passagem e de pagamento com os sistemas nacionais. É a norma que, um ano depois, tornaria possível a consulta nacional no app CNH do Brasil.

Duas consequências diretas para o motorista:

- **Sistema não homologado não gera infração.** Sistemas de livre passagem não homologados junto à Senatran não podem ser usados para os fins do art. 115, § 10, do Código de Trânsito Brasileiro, o que afasta a infração do art. 209-A. A relação dos sistemas homologados fica no site da Senatran.
- **Falha técnica exige nova tentativa de cobrança.** Quando há falha na confirmação do pagamento automático, o operador deve realizar ao menos mais uma tentativa até o prazo máximo de pagamento, para mitigar autuação indevida de quem tem tag ativa.

Fonte: [Ministério dos Transportes, normas de trânsito](https://www.gov.br/transportes/pt-br/assuntos/transito). Afeta: [Multa do Free Flow](multa-free-flow.md) e [Prazo e encargos](prazo-e-encargos.md).

---

## Próximas datas a observar

| Quando | O que acontece | Onde |
|---|---|---|
| 10 de outubro de 2026 | Início anunciado da cobrança na MT-130, com seis pórticos | MT, Rota dos Grãos |
| 16 de novembro de 2026 | Fim do prazo de regularização sem penalidades de trânsito | Nacional |
| 17 de novembro de 2026 | Tarifas em aberto voltam a poder gerar auto de infração | Nacional |
| Dezembro de 2026 | Free Flow previsto em contrato na BR-116 e BR-251, norte de Minas | MG, Ecovias das Gerais |
| Novembro de 2026 | 14 pórticos previstos no corredor Três Lagoas, Água Clara e Campo Grande | MS, Rota da Celulose |
| Sem data | Retomada do Sistema Anchieta-Imigrantes, com o pórtico da subida após o km 38 | SP, Ecovias dos Imigrantes |

Trechos com status `previsto` ou `adiado` **não cobram tarifa por pórtico hoje**. A lista completa está na seção [Onde o Free Flow ainda vai chegar](../README.md#onde-o-free-flow-ainda-vai-chegar).

---

## Regras que valem hoje

| Regra | O que define |
|---|---|
| Resolução ANTT nº 6.079/2026 | Sistema de livre passagem nas rodovias federais concedidas, publicada em 27/03/2026 |
| Resolução CONTRAN nº 1.013/2024 | Prazo geral de 30 dias para pagamento da tarifa, ressalvado o contrato de cada concessão |
| Deliberação CONTRAN nº 277/2026 | Conta os 30 dias da confirmação do processamento do registro da passagem, e não da passagem; regularização sem penalidades de trânsito até 16/11/2026, mantida a obrigação de pagar a tarifa |
| Portaria Senatran nº 442/2025 | Homologação e interoperabilidade dos sistemas de livre passagem; sistema não homologado não gera a infração do art. 209-A |
| Lei nº 14.157/2021 | Incluiu o art. 209-A no Código de Trânsito Brasileiro e o § 10 do art. 115 |
| Art. 209-A do Código de Trânsito Brasileiro | Infração grave, com 5 pontos na CNH, para a passagem não paga |

---

## Como esta página é mantida

| Evento | Prazo de atualização |
|---|---|
| Inauguração, adiamento ou realocação de pórtico | até 72 horas após o fato confirmado |
| Mudança de regra ou de prazo por norma publicada | até 72 horas após a publicação |
| Revisão completa das notas e das bases | mensal |

Toda nota nasce de **fonte oficial**, seja a ANTT, uma agência estadual ou a concessionária responsável. Anúncio de imprensa entra com a fonte identificada e só vira mudança de status na base quando a concessionária ou o regulador confirma.

Viu um pórtico novo, uma data que mudou ou um link que quebrou? [Abra uma issue](../../../issues/new) contando o que viu, com a fonte. As regras estão em [CONTRIBUTING.md](../CONTRIBUTING.md), e o histórico de versões da base em [CHANGELOG.md](../CHANGELOG.md).

---

### Enquanto as regras mudam, a tag resolve

Com uma tag ativa, a tarifa do Free Flow é debitada automaticamente, entra nos descontos do trecho e nenhum prazo depende da sua memória.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=novidades&utm_campaign=sem-parar-free-flow)**, o canal mais indicado. Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

Passou num Free Flow e não é cliente? Dá para quitar só aquela passagem, pela placa, em [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=novidades&utm_campaign=sem-parar-free-flow).

<sub>Página viva mantida pelo <strong>Sem Parar</strong> sob <a href="../LICENSE">CC BY 4.0</a>. Em caso de divergência, as fontes oficiais linkadas em cada nota prevalecem sobre o que está aqui.</sub>
