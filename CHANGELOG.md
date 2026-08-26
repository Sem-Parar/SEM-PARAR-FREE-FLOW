# Changelog

Todas as mudanças relevantes deste repositório são registradas aqui. O formato é baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/) e as datas seguem o padrão ISO (`AAAA-MM-DD`).

**Por que um changelog num repositório de conteúdo:** os dados de Free Flow mudam toda semana. Pórtico inaugura, inauguração é adiada, canal de pagamento muda de endereço. O changelog é o que permite a qualquer pessoa saber o que mudou e quando, e é o registro de frescor da base.

## [Não publicado]

Nada por enquanto.

---

## [0.4.0], 2026-08-26

Dores. O repositório passa a cobrir a régua completa do que acontece quando a tarifa não é paga: prazo, encargos, multa, recurso e o caminho de regularização enquanto a janela de transição está aberta.

### Adicionado

- **[`docs/passei-sem-tag.md`](docs/passei-sem-tag.md)**, em tom de alívio: passar sem tag não é infração, é o funcionamento normal do sistema. Traz os três passos para resolver, a tabela de quando isso vira problema e quando não vira, os casos de carro alugado, de terceiro e vendido, e o que se perde sem tag.
- **[`docs/prazo-e-encargos.md`](docs/prazo-e-encargos.md)**, a régua degrau por degrau, os três acréscimos que incidem depois dos 30 dias com base legal de cada um, a separação entre tarifa e multa, e a lista do que a norma exige da concessionária em contrapartida.
- **[`docs/multa-free-flow.md`](docs/multa-free-flow.md)**, o texto do art. 209-A, a penalidade, a distinção entre concessionária e órgão autuador, a janela de cancelamento e ressarcimento, o rito de defesa e recursos (JARI e CETRAN) e os argumentos que a própria regulação coloca do lado do usuário. Inclui, por honestidade, a lista do que **não** funciona como defesa.
- **[`docs/nao-paguei-e-agora.md`](docs/nao-paguei-e-agora.md)**, o caminho de regularização em três passos, a tabela de cenários por situação, o de-para de quando falar com a concessionária e quando falar com o órgão autuador, e o alerta de golpe específico desta janela.
- Nota de **12 de junho de 2025** em [`docs/novidades.md`](docs/novidades.md), sobre a Portaria Senatran nº 442/2025, que criou a homologação obrigatória e é a norma que tornou possível a consulta nacional de 2026.
- Linha da **Lei nº 14.157/2021** na tabela de regras vigentes de Novidades.

### Corrigido

- **A contagem do prazo de 30 dias, de novo, e agora completa.** A versão 0.3.0 dizia que os 30 dias contam da confirmação do processamento do registro. Está certo para a **infração de trânsito**, mas incompleto: a Resolução ANTT nº 6.079/2026 conta **da passagem pelo pórtico** para efeito dos **encargos financeiros** nas rodovias federais concedidas. As duas fontes são oficiais e tratam de planos distintos. A divergência agora está registrada em tabela no README, em [`docs/como-pagar.md`](docs/como-pagar.md), em [`docs/o-que-e-free-flow.md`](docs/o-que-e-free-flow.md), em [`docs/consulta-app-cnh-do-brasil.md`](docs/consulta-app-cnh-do-brasil.md) e, com o detalhamento completo, em [`docs/prazo-e-encargos.md`](docs/prazo-e-encargos.md).
- **Pagar a multa não quita a tarifa.** O README dizia apenas que a passagem não paga vira infração. Faltava a consequência que mais surpreende, e que está expressa na Resolução ANTT nº 6.079/2026: o pagamento da multa não exime o usuário de quitar a tarifa, os encargos administrativos, a multa moratória e os juros legais.

### Alterado

- **README**: quatro páginas novas na seção Conteúdos, com link direto para cada arquivo, e correção dos blocos de prazo e de consequência do não pagamento.
- **`docs/como-pagar.md`**: tabela de contagem de prazo por norma e detalhamento dos meios de pagamento obrigatórios previstos na Resolução ANTT nº 6.079/2026.
- **`docs/novidades.md`**: a nota de 27/03/2026 sobre a Resolução ANTT nº 6.079/2026 ganhou a régua financeira completa, com encargos, moratória, juros, devolução em dobro, meios de pagamento obrigatórios e prazo de armazenamento das transações.

### Notas de dado

- **Encargos após o vencimento, nas federais concedidas** (Resolução ANTT nº 6.079/2026): encargos administrativos limitados ao ressarcimento dos custos de identificação e notificação, sujeitos à aprovação da ANTT; **multa moratória de 2%**, com base no art. 52, § 1º, do Código de Defesa do Consumidor; e **juros legais de 1% ao mês**, pro rata temporis, com base nos arts. 395, 397 e 406 do Código Civil. São percentuais de lei e de regulação, não política comercial de empresa, e por isso são publicados. Nenhum valor de tarifa segue armazenado.
- **Penalidade do art. 209-A**, incluído no Código de Trânsito Brasileiro pela Lei nº 14.157/2021: infração **grave**, **5 pontos na CNH** e multa de **R$ 195,23**, valor da infração grave verificado em 26/08/2026 e sujeito a atualização pela regulação de trânsito. É a única cifra em reais publicada no repositório, e ela está sempre acompanhada de data e da ressalva de atualização.
- **Regime de transição:** o Ministério dos Transportes informou, em 28/04/2026, a suspensão de **3,4 milhões de multas** em rodovias federais e estaduais, e estimou em cerca de **R$ 93 milhões** o montante a ressarcir considerando as federais. O cancelamento da multa não paga e da pontuação é feito pelo próprio órgão autuador após a regularização da tarifa, sem pedido do usuário; o **ressarcimento de multa já paga depende de solicitação** ao órgão autuador, com comprovação.
- **Órgão autuador não é a concessionária.** Ele é identificado no próprio auto de infração e varia por via e por estado. Nas rodovias estaduais do Rio Grande do Sul, por exemplo, é o DAER.
- **Obrigações da concessionária** que sustentam defesa: opção de pagamento pós-passagem em até 2 horas para 90% das passagens e 24 horas para 99%; múltiplos meios de pagamento incluindo Pix, cartões, dinheiro e sistemas automáticos; devolução em dobro de cobrança indevida em até 7 dias corridos; armazenamento das transações por cinco anos e fornecimento do histórico para instruir defesa ou recurso.
- **Jurisprudência registrada, não inferida:** turmas recursais já decidiram que a ausência de cancela é irrelevante para a tipicidade do art. 209-A e que não há bis in idem entre a tarifa, de natureza civil, e a multa, de natureza administrativa. A informação entra como contexto honesto, com a ressalva de que o material é informativo e não substitui orientação jurídica.
- Nenhuma mudança na contagem nacional: seguem **74 pórticos** em operação, em 26 rodovias, 15 concessionárias e 7 estados.

---

## [0.3.0], 2026-08-26

Pagar e consultar. O repositório passa a responder, com caminho completo, as duas perguntas que mais aparecem depois da passagem pelo pórtico: onde eu pago e como eu descubro que passei.

### Adicionado

- **[`docs/como-pagar.md`](docs/como-pagar.md)**, o guia definitivo de pagamento: o que muda com tag e sem tag, o passo a passo de quem não tem tag, a tabela de canal oficial por concessionária das 15 concessionárias com Free Flow em operação, o prazo, o que acontece se ele passar e como pagar a passagem de um carro que não é seu.
- **[`docs/consultar-pela-placa.md`](docs/consultar-pela-placa.md)**, os três caminhos de consulta (app CNH do Brasil, Portal de Serviços Senatran e canal da concessionária) e o **roteador de rodovia para concessionária**, que responde à pergunta "passei, mas pago para quem". Inclui as razões pelas quais uma passagem pode não aparecer e o caminho de contestação.
- **[`docs/consulta-app-cnh-do-brasil.md`](docs/consulta-app-cnh-do-brasil.md)**, o passo a passo da consulta nacional liberada em 24/08/2026: o que a tela mostra campo a campo, filtros e período, os dois alertas do app, o que ele não faz e como contestar.
- **[`docs/sites-e-apps-oficiais.md`](docs/sites-e-apps-oficiais.md)**, a lista verificada dos 29 canais legítimos, separada em canais de governo, canais de concessionária e plataformas de pagamento, e operadoras de tag, com os quatro sinais que identificam um canal oficial e as três armadilhas que a lista deixa visíveis.
- Nota de **29 de abril de 2026** em [`docs/novidades.md`](docs/novidades.md), sobre a Deliberação CONTRAN nº 277/2026, que faltava na linha do tempo.
- Linha da **Portaria Senatran nº 442/2025** na tabela de regras vigentes de Novidades: sistema de livre passagem não homologado não gera a infração do art. 209-A.

### Corrigido

- **Contagem do prazo de pagamento.** O repositório dizia "até 30 dias após a passagem". A Deliberação CONTRAN nº 277/2026 alterou o art. 7º da Resolução CONTRAN nº 1.013/2024, e o prazo de 30 dias passou a ser contado **da confirmação do processamento do registro da passagem** junto ao órgão máximo executivo de trânsito da União. Corrigido no README e em [`docs/o-que-e-free-flow.md`](docs/o-que-e-free-flow.md), com a ressalva de extensão para o próximo dia útil.
- **Referência à versão do app CNH do Brasil.** A menção a "versão 7.3.0 ou superior" saiu de todas as páginas e da base, substituída por "com o app atualizado". O número não foi confirmado em fonte oficial primária na revalidação de 26/08/2026, e a regra da casa é não afirmar o que não se confirma.
- **Valores de situação do débito** no FAQ do README: são em processamento, pendente, isento ou pago, e não "vencido".

### Alterado

- **`dados/canais-oficiais-pagamento.csv`**: as linhas do **app CNH do Brasil** e do **Portal de Serviços Senatran** foram enriquecidas com o que a consulta nacional passou a oferecer em 24/08/2026, e reverificadas nesta data. As 29 linhas foram mantidas.
- **README**: quatro páginas novas na seção Conteúdos, com link direto para cada arquivo, correção do bloco de prazo e ponteiros para os guias a partir das seções "Como pagar o Free Flow", "Regra de ouro contra golpes" e do FAQ.
- **`docs/novidades.md`**: a nota de 24/08/2026 ganhou o detalhamento da consulta nacional, com as 14 concessionárias integradas na estreia, os dois alertas, a contestação e o Portal de Serviços Senatran.
- **`docs/glossario.md`**: verbete do app CNH do Brasil atualizado.

### Notas de dado

- **Consulta nacional de Free Flow, 24/08/2026:** estreou com **14 concessionárias** integradas, em rodovias federais, estaduais e municipais. Pessoa física consulta pelo app CNH do Brasil ou pelo Portal de Serviços Senatran, que traz mais detalhe; **empresas e frotas consultam exclusivamente pelo Portal**. Nenhum dos dois recebe pagamento.
- **Escala da operação:** segundo o Ministério dos Transportes e o Serpro, a solução foi construída em três meses, com 27 organizações envolvidas, e já processou mais de 200 milhões de registros de passagem do passivo do sistema, com cerca de 10 milhões de novas passagens somente em agosto de 2026.
- **Regime de transição:** prazo excepcional de 200 dias contados da publicação da Deliberação CONTRAN nº 277/2026, em 29/04/2026, encerrando em **16/11/2026**. Para passagens feitas no período, prevalece o prazo mais favorável ao usuário. Quitar dentro do prazo cancela os processos de infração, exclui penalidade e pontuação e, se a multa já tinha sido paga, autoriza pedido de revisão e restituição.
- **Homologação:** a mesma Deliberação concedeu 100 dias para homologação dos sistemas de livre passagem junto à Senatran. Sistema não homologado não pode ser usado para os fins do art. 115, § 10, do Código de Trânsito Brasileiro, o que afasta a infração do art. 209-A, conforme a Portaria Senatran nº 442/2025.
- **Meios de pagamento aceitos:** deliberadamente não publicados por canal. A Resolução CONTRAN nº 1.013/2024 admite quaisquer canais válidos de recebimento e cada concessionária define o próprio cardápio, que muda com frequência. A regra da casa vale aqui: dado perecível fica na origem.
- Nenhuma mudança na contagem nacional: seguem **74 pórticos** em operação, em 26 rodovias, 15 concessionárias e 7 estados.

---

## [0.2.0], 2026-08-26

Base de entendimento. O repositório ganha as páginas que explicam o sistema, definem o vocabulário, registram o que muda e apresentam quem publica.

### Adicionado

- **[`docs/o-que-e-free-flow.md`](docs/o-que-e-free-flow.md)**, a explicação completa do sistema: como o pórtico identifica o veículo, o que muda com tag e sem tag, prazo de pagamento, descontos DBT e DUF, consequências do não pagamento e por que o país está trocando a praça pelo pórtico.
- **[`docs/glossario.md`](docs/glossario.md)**, com 41 verbetes do pedágio eletrônico, de ANPR e RFID a trecho tarifário e Vale-Pedágio, incluindo os termos da Resolução ANTT nº 6.079/2026.
- **[`docs/novidades.md`](docs/novidades.md)**, página viva com a linha do tempo do Free Flow no Brasil, uma nota por fato com data e fonte oficial, a tabela de próximas datas a observar e as regras vigentes.
- **[`SEM-PARAR.md`](SEM-PARAR.md)**, a página de identidade do repositório: história desde 2000, verticais da plataforma, cobertura, governança regulatória e a lista de canais oficiais da marca.
- Seção **Conteúdos deste repositório** no README, com link direto para cada página.

### Alterado

- **`dados/rodovias-free-flow.csv`** passa de 43 para 44 linhas, com a inclusão da **MT-130**, entre Primavera do Leste e Paranatinga, com status `previsto`.
- **`dados/concessionarias-free-flow.csv`** passa de 22 para 23 linhas, com a inclusão da **Concessionária de Rodovias Rota dos Grãos**.
- **`dados/README.md`**: a definição de `status = previsto` e a de `inicio_operacao` passam a contemplar trechos com data de início já anunciada.
- Correção do endereço do repositório no badge de última atualização e nos blocos "Como citar" do README e do dicionário de dados.

### Notas de dado

- **MT-130 (Rota dos Grãos):** a concessionária anunciou o início da cobrança por pórtico para **10/10/2026**, com seis pórticos substituindo as duas praças físicas do trecho. Registrada como `previsto`, com a data em `inicio_operacao`. Quando a cobrança começar, Mato Grosso será o oitavo estado com Free Flow ativo.
- **Sistema Anchieta-Imigrantes:** revalidado em 26/08/2026, segue **adiado e sem nova data**, com o ponto de cobrança da subida da Imigrantes mantido após o km 38.
- **App CNH do Brasil:** confirmada a disponibilidade da consulta de passagens desde 24/08/2026, e o marco de **17/11/2026**, quando tarifas em aberto voltam a poder gerar auto de infração.
- Nenhuma mudança na contagem de pórticos em operação: seguem **74 pórticos**, em 26 rodovias, 15 concessionárias e 7 estados.

---

## [0.1.0], 2026-08-25

Primeira versão pública do repositório de Free Flow e Tag de Pedágio do Sem Parar. Fundação: hub, infraestrutura e as três bases de dados iniciais.

### Adicionado

- **README**, o hub do projeto, com a tabela nacional de rodovias com Free Flow, guia de pagamento, seção de Tag de Pedágio, FAQ com 10 perguntas e a seção de dados abertos.
- **`dados/rodovias-free-flow.csv`** com 43 rodovias mapeadas: 26 com Free Flow ativo, somando 74 pórticos em operação, e 17 com operação prevista ou adiada.
- **`dados/concessionarias-free-flow.csv`** com 22 concessionárias, sendo 15 com Free Flow ativo, incluindo grupo econômico, plataforma de pagamento, canais e situação.
- **`dados/canais-oficiais-pagamento.csv`** com 29 canais oficiais de consulta e pagamento verificados um a um, com nível de verificação declarado. É a base da camada anti-golpe.
- **`dados/README.md`**, o dicionário de dados, com significado, formato e valores aceitos de cada coluna.
- Infraestrutura do repositório: `LICENSE` (CC BY 4.0), `CONTRIBUTING.md` e `CODE_OF_CONDUCT.md`.
- Banner do projeto em `.github/assets/banner.svg`, nas cores oficiais da marca.

### Cobertura desta versão

Rodovias com Free Flow em operação em 7 estados: SP, PR, MG, GO, RS, RJ e RO.

### Notas de dado

- Levantamento com data de corte em 2026-08-25, a partir do painel oficial da ANTT, dos portais das agências estaduais (ARTESP, AGERGS e DER-MG) e dos sites das concessionárias.
- **Sistema Anchieta-Imigrantes (SP-150 e SP-160):** registrado como adiado. O início foi adiado em 27/07/2026 sem nova data, e o pórtico da subida da Imigrantes foi realocado do km 29 para a região do km 38, com ponto exato ainda em estudo. As praças físicas de Riacho Grande e Piratininga seguem em operação.
- **Via Campo (Lote 5, PR):** registrada como adiada. O próprio site da concessionária informa que o sistema está em homologação, sem previsão de início da cobrança por pórticos.
- **FreeWay (BR-116/290, RS):** registrada como prevista, não ativa. É uma confusão comum causada pelo nome comercial da rodovia. A conversão das praças da CCR ViaSul segue em estudo, sem prazo.
- **Divergências de quilometragem** entre o cadastro da ANTT e as concessionárias, nos casos de BR-381 em João Monlevade, BR-376 em Mauá da Serra e PR-445 em Tamarana, foram resolvidas em favor do valor da ANTT, com a divergência anotada no campo de trecho.
- Nenhum valor de tarifa, mensalidade ou percentual de desconto é armazenado nas bases. Apenas o link da tabela tarifária oficial de cada concessionária.

### Contexto regulatório vigente nesta versão

- **Resolução ANTT nº 6.079/2026**, publicada em 27/03/2026, que regulamenta o sistema de livre passagem nas rodovias federais concedidas.
- **Deliberação CONTRAN nº 277/2026**, regra de transição com prazo até 16/11/2026 para regularização de tarifas em aberto sem as penalidades de trânsito. A tarifa continua devida.
- **App CNH do Brasil** com consulta de passagens de Free Flow disponível desde 24/08/2026, na versão 7.3.0 ou superior.

[Não publicado]: https://github.com/TRIWI-SEO/SEM-PARAR-FREE-FLOW/compare/v0.4.0...HEAD
[0.4.0]: https://github.com/TRIWI-SEO/SEM-PARAR-FREE-FLOW/releases/tag/v0.4.0
[0.3.0]: https://github.com/TRIWI-SEO/SEM-PARAR-FREE-FLOW/releases/tag/v0.3.0
[0.2.0]: https://github.com/TRIWI-SEO/SEM-PARAR-FREE-FLOW/releases/tag/v0.2.0
[0.1.0]: https://github.com/TRIWI-SEO/SEM-PARAR-FREE-FLOW/releases/tag/v0.1.0
