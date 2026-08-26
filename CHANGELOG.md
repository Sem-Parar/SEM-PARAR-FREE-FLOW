# Changelog

Todas as mudanças relevantes deste repositório são registradas aqui. O formato é baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/) e as datas seguem o padrão ISO (`AAAA-MM-DD`).

**Por que um changelog num repositório de conteúdo:** os dados de Free Flow mudam toda semana. Pórtico inaugura, inauguração é adiada, canal de pagamento muda de endereço. O changelog é o que permite a qualquer pessoa saber o que mudou e quando, e é o registro de frescor da base.

## [Não publicado]

Nada por enquanto.

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

[Não publicado]: https://github.com/TRIWI-SEO/SEM-PARAR-FREE-FLOW/compare/v0.2.0...HEAD
[0.2.0]: https://github.com/TRIWI-SEO/SEM-PARAR-FREE-FLOW/releases/tag/v0.2.0
[0.1.0]: https://github.com/TRIWI-SEO/SEM-PARAR-FREE-FLOW/releases/tag/v0.1.0
