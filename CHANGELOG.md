# Changelog

Todas as mudanças relevantes deste repositório são registradas aqui. O formato é baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/) e as datas seguem o padrão ISO (`AAAA-MM-DD`).

**Por que um changelog num repositório de conteúdo:** os dados de Free Flow mudam toda semana. Pórtico inaugura, inauguração é adiada, canal de pagamento muda de endereço. O changelog é o que permite a qualquer pessoa saber o que mudou e quando, e é o registro de frescor da base.

## [Não publicado]

- **Comparativo de tags de pedágio**, a peça do Programa Escolher: seis critérios de decisão, tabela das cinco operadoras autorizadas pela ARTESP e veredito por perfil de motorista. Produzida e revisada, **aguardando aprovação do cliente** antes de publicar.

---

## [0.9.0], 2026-08-26

Proteção e base legal. O repositório ganha a camada documental: a cadeia normativa inteira, a lista de homologações da Senatran, o roteiro anti-golpe e o caminho da contestação. Duas bases abertas novas, e um fato de agosto que faltava na linha do tempo.

### Adicionado

- **[`BASE-LEGAL-DO-FREE-FLOW.md`](BASE-LEGAL-DO-FREE-FLOW.md)**, na raiz: o texto do art. 209-A palavra por palavra, as **duas condutas** que ele tipifica e por que a segunda alcança o Free Flow, a defesa de atipicidade e por que os tribunais a rejeitam, a separação entre tarifa e multa, as onze normas da cadeia, a divergência de prazo entre ANTT e CONTRAN, o efeito da falta de homologação e os direitos criados pela Resolução ANTT nº 6.079/2026.
- **[`docs/golpe-do-falso-pedagio.md`](docs/golpe-do-falso-pedagio.md)**: as duas modalidades descritas pela ANTT, o teste do endereço em dez segundos, as quatro coisas que nenhum canal oficial faz, os sinais dentro da página falsa, o risco do resultado patrocinado e o roteiro de seis passos para quem já pagou.
- **[`docs/homologacao-senatran-free-flow.md`](docs/homologacao-senatran-free-flow.md)**: o que a homologação significa, a lista das doze publicadas, por que homologação não é início de cobrança e a segunda proteção, menos conhecida, sobre a ausência de dados impedir a emissão de autos.
- **[`docs/cobranca-indevida-como-contestar.md`](docs/cobranca-indevida-como-contestar.md)**: as cinco situações que parecem erro e não são, os seis casos que são erro de verdade, onde contestar conforme quem cobrou, os seis itens a pedir e a resposta sobre pagar ou contestar primeiro.
- **[`dados/base-legal-free-flow.csv`](dados/base-legal-free-flow.csv)**, a sexta base aberta, com **12 registros**, um por norma, incluindo órgão, data, o que estabelece, alcance, vigência e link oficial.
- **[`dados/homologacao-senatran-free-flow.csv`](dados/homologacao-senatran-free-flow.csv)**, a sétima base aberta, com **12 registros**, um por portaria de homologação, com CNPJ, número, data e se a concessionária cobra por pórtico hoje.
- Nota em [`docs/novidades.md`](docs/novidades.md) sobre as homologações publicadas entre 31 de julho e 10 de agosto de 2026, que faltavam na linha do tempo.

### Alterado

- **README**: quatro páginas novas na seção Conteúdos, duas bases novas na seção Dados abertos, badge de bases abertas e ponteiro para a página de golpe na Regra de ouro.
- **[`docs/novidades.md`](docs/novidades.md)**: o bloco "O que está valendo agora" ganha uma quarta linha sobre homologação.
- **Dicionário de dados**: capítulos das duas bases novas, com o limite declarado da base de homologações.

### Notas de dado

- **O art. 209-A tipifica duas condutas, não uma.** O texto é "evadir-se da cobrança pelo uso de rodovias e vias urbanas para não efetuar o seu pagamento, **ou deixar de efetuá-lo na forma estabelecida**". A primeira não alcança o Free Flow, porque não há barreira física; a segunda alcança. Infração grave, penalidade de multa.
- **A defesa de atipicidade vem sendo rejeitada.** O TJ-SP, julgando multas em Pindamonhangaba, registrou que o dispositivo prevê mais de uma conduta típica, aplicável tanto às praças tradicionais quanto ao sistema de livre passagem. O TJ-RS decidiu na mesma linha e afastou também a alegação de bis in idem entre tarifa, de natureza civil, e multa, de natureza administrativa.
- **Portaria Senatran nº 442/2025, art. 8º, § 2º:** sistema de livre passagem não homologado não pode ser usado para os fins do art. 115, § 10 do CTB, **afastando a infração do art. 209-A**. A tarifa continua devida, porque é obrigação civil. O § 3º traz regra de transição para atos praticados sob as Resoluções CONTRAN nº 984/2022 e nº 1.013/2024, e o § 4º determina que a relação de sistemas homologados fique no sítio da Senatran.
- **Doze homologações publicadas entre 31/07 e 10/08/2026**, pelas Portarias 603, 604, 607, 612, 613, 615, 616, 617, 618, 620, 638 e 640. As portarias obrigam o envio à Senatran dos dados de passagem e pagamento, inclusive anteriores, e determinam que, enquanto a ausência desses dados impedir a comprovação da infração, **não podem ser emitidos autos de infração**.
- **Homologação não é aprovação técnica** nem validação de projeto, e a responsabilidade pelos dados segue das concessionárias, conforme a própria Senatran declara.
- **Homologação não é início de cobrança.** A Ecovias dos Imigrantes foi homologada pela Portaria 613, de 03/08/2026, e os pórticos do Sistema Anchieta-Imigrantes seguem sem cobrar, com o início adiado pelo Governo de São Paulo e sem nova data.
- **Concessionária nova no radar:** a Rota Agro MT-GO foi homologada pela Portaria 640, de 10/08/2026, e ainda não consta no inventário de pórticos deste repositório, por falta de confirmação oficial de cobrança em operação. Registrada como `n/d`.
- **Resolução CONTRAN nº 984/2022** entra na base legal: foi o primeiro regulamento do sistema de livre passagem e seus atos seguem produzindo efeitos por regra de transição.
- **Modalidades de golpe descritas pela ANTT:** páginas falsas de consulta que geram chave Pix para o golpista, e boletos falsos enviados a endereço físico ou e-mail com dados obtidos de forma irregular. A ANTT afirma que **não há envio automático de boletos nem site único nacional** de consulta de débitos.
- **O sinal que entrega o golpe é o endereço**, não o visual. Páginas falsas copiam marca, cores e layout com precisão, e chegam por anúncio patrocinado acima do site oficial nos buscadores. O trecho imediatamente antes do `.com` ou `.com.br` precisa ser exatamente o nome da empresa.
- **Páginas falsas citam o art. 209-A com texto inventado**, e usam contagem regressiva de minutos e ameaça de encaminhamento imediato ao Detran. Nenhum canal oficial faz isso.

---

## [0.8.0], 2026-08-26

Camada das concessionárias. O repositório passa a responder "pago para quem", com o índice nacional por grupo econômico e as páginas das quatro operadoras de maior demanda. Esta versão traz também a correção de dois dados que envelheceram no site da própria concessionária.

### Adicionado

- **[`CONCESSIONARIAS-FREE-FLOW.md`](CONCESSIONARIAS-FREE-FLOW.md)**, na raiz: as 15 concessionárias em operação, ordenadas por número de pórticos, agrupadas por grupo econômico, e o mapa das quatro plataformas que processam o pagamento. Inclui a seção **Por que o site de pagamento tem outro nome**, que explica por que o endereço de pagamento raramente traz o nome da rodovia, e a lista das concessionárias com Free Flow previsto ou adiado, útil para reconhecer cobrança falsa.
- **[`concessionarias/free-flow-motiva-ccr.md`](concessionarias/free-flow-motiva-ccr.md)**: as três concessões do maior grupo do país, a transição de marca de CCR para Motiva, o Pedágio Digital e o alerta sobre o domínio terminado em `.com`, a janela de duas horas para reentrada e as regras próprias da Via Dutra.
- **[`concessionarias/free-flow-ecovias.md`](concessionarias/free-flow-ecovias.md)**: os quatro pórticos em operação, o pioneirismo estadual paulista, as duas informações que mudaram desde o lançamento e a situação do Sistema Anchieta-Imigrantes, que tem pórtico instalado e não cobra.
- **[`concessionarias/free-flow-csg.md`](concessionarias/free-flow-csg.md)**: os seis pórticos gaúchos um a um, os dois pioneirismos da concessionária, as cinco operadoras de tag que ela publica, o caminho do motociclista com cadastro sem tag e por que o Bloco 3 lista rodovias que não têm pórtico.
- **[`concessionarias/free-flow-epr.md`](concessionarias/free-flow-epr.md)**: as três concessões que já cobram, o pagamento da passagem eletrônica nas praças físicas, as duas declarações do grupo que desarmam golpe e a regra do eixo suspenso com MDF-e para veículos pesados.
- Pasta **`concessionarias/`**, que vai receber as demais páginas de concessionária.

### Corrigido

- **O endereço de pagamento da Ecovias Noroeste Paulista mudou.** O repositório apontava para `freeflow.ecoviasnoroestepaulista.com.br`, que não aparece em nenhuma comunicação oficial atual. O endereço divulgado hoje pela concessionária é **`freeflow.eco.br`**, e o portal do grupo é `freeflow.ecovias.com.br`. Corrigido em 8 arquivos e em duas bases.
- **O prazo da Ecovias Noroeste Paulista não é mais menor que a regra geral.** No lançamento, em setembro de 2024, a concessionária divulgava 15 dias; hoje divulga 30. O repositório repetia a informação antiga em três páginas, orientando o leitor a esperar um prazo mais curto do que o vigente. Reescrito em `docs/como-pagar.md`, `docs/prazo-e-encargos.md` e `docs/sites-e-apps-oficiais.md`, agora usando a própria mudança como exemplo de por que confirmar o prazo no canal da concessionária.
- **O pórtico de Taiúva, na SP-326, entrou em operação em 01/12/2025, e não em 01/11/2025.** A data de Dobrada foi aplicada aos dois pórticos da rodovia. Corrigido na base de pórticos, no índice nacional e no README.
- **A CSG publica sim a lista de operadoras de tag aceitas.** A base `tags-aceitas-free-flow.csv` registrava `n/d` para ela. A concessionária divulga as cinco no próprio site: ConectCar, Move Mais, Sem Parar, Taggy e Veloe.

### Alterado

- **`dados/concessionarias-free-flow.csv`**: plataforma de pagamento da Ecovias Noroeste Paulista passa de "Pedágio Digital e Pedágio Pay" para **Pedágio Digital**, que é o que a concessionária divulga hoje.
- **`dados/canais-oficiais-pagamento.csv`**: endereço e observação do canal da Ecovias Noroeste Paulista atualizados.
- **README**: seis páginas novas na seção Conteúdos e ponteiro para o índice de concessionárias logo abaixo da tabela nacional.

### Notas de dado

- **Sete grupos econômicos identificados, mais três concessionárias que não divulgam o controlador, operam os 85 pórticos.** Motiva, ex-CCR, opera 29, mais de um terço do total, distribuídos entre RioSP, Motiva Sorocabana e PRVias. Grupo EPR opera 13; 4UM e Opportunity, 12, com Nova 364 e Nova 381; Fundo Aviva e 4i Capital, 11, com a Rota Verde Goiás. Os três maiores grupos somados passam de metade dos pórticos do país.
- **Quatro plataformas processam o pagamento de quem passa sem tag.** Pedágio Digital atende 33 pórticos, de concessionárias da Motiva e da EcoRodovias, que são grupos concorrentes. Plataformas próprias das concessionárias atendem 24. Alpdex atende 23, nas três concessões de 4UM, Opportunity e Aviva. Movvia atende 5, na Novo Litoral, e figura como parceiro da CSG. **Plataforma de pagamento não é operadora de tag:** ela processa apenas o pagamento por placa.
- **A EcoRodovias aparece pequena na contagem de pórticos e não é uma operadora pequena.** A maior parte da malha dela ainda cobra em praça com cancela, e as conversões estão contratadas. O contrato da Ecovias Noroeste Paulista prevê a substituição de todas as praças por pórticos até o sétimo ano da concessão.
- **A EPR aceita o pagamento da passagem eletrônica em todas as praças físicas dela**, em dinheiro ou cartão, bastando consultar o operador da cabine. É um canal presencial que nenhuma outra concessionária do inventário oferece nesse formato.
- **Duas declarações públicas da EPR que desarmam confusão:** a concessionária não envia boletos e não emite multas, e afirma que pagar a multa não quita a tarifa, que permanece em aberto.
- **Regra de eixo suspenso na EPR:** a cobrança de veículo pesado usa o MDF-e como critério. Com MDF-e em aberto o veículo é tratado como carregado e todos os eixos entram na conta; sem MDF-e em aberto, apenas os eixos em contato com o solo.
- **A CSG nunca teve praça de pedágio.** Os pórticos do Bloco 3 não substituíram cabines: substituíram as praças previstas em contrato e nunca construídas. E a concessionária concede desconto ao motociclista que se cadastra no site ou no app, reconhecendo que a moto não pode usar tag.
- **A CSG publica canais parceiros de consulta e pagamento**, entre eles o `pedagioeletronicosemparar.com.br`, o canal do Sem Parar para pagamento avulso de quem não é cliente.
- **Na EPR Paraná, 8 pórticos correspondem a 4 pontos tarifários**, com um pórtico por sentido. A cobrança começou em 04/05/2026, após dez dias de operação assistida em caráter educativo.
- **Nem toda rodovia de concessionária com Free Flow tem Free Flow.** As praças da BR-277, na EPR Iguaçu, seguem convencionais, e a Motiva Sorocabana opera cinco pórticos apenas de monitoramento na SP-270, que não cobram.

---

## [0.7.0], 2026-08-26

Camada da tag. O repositório passa a responder o outro lado do Free Flow: não só como pagar quando não se tem tag, mas o que muda quando se tem. Entra o terceiro pilar na raiz, a quinta base aberta e a correção de um erro de contagem que estava publicado desde a 0.5.0.

### Adicionado

- **[`TAG-DE-PEDAGIO.md`](TAG-DE-PEDAGIO.md)**, na raiz: o pilar da tag. O que é o dispositivo e como o pórtico o lê, a separação entre concessionária e operadora de tag, a tabela com tag e sem tag lado a lado, a interoperabilidade obrigatória nas federais, por que o desconto depende de identificação eletrônica, e uma seção sobre o que a tag **não** resolve.
- **[`docs/tags-aceitas-no-free-flow.md`](docs/tags-aceitas-no-free-flow.md)**: a tabela de aceitação nas 15 concessionárias com Free Flow em operação, a diferença entre o regime federal e o estadual, as cinco operadoras autorizadas pela ARTESP publicadas nominalmente, e as três situações em que a tag não entra.
- **[`docs/como-funciona-a-cobranca-da-tag.md`](docs/como-funciona-a-cobranca-da-tag.md)**: o caminho do pórtico até a fatura com os quatro atores envolvidos, quanto tempo cada sistema leva para mostrar a passagem, cinco situações que parecem erro de cobrança e não são, e o que a Resolução ANTT nº 6.079/2026 garante ao usuário.
- **[`docs/tag-em-moto-e-outros-veiculos.md`](docs/tag-em-moto-e-outros-veiculos.md)**: por que não existe tag para moto no Brasil, a tabela nacional de onde a moto paga e onde é isenta, o caso do carro alugado e a regra de uma tag por placa.
- **[`dados/tags-aceitas-free-flow.csv`](dados/tags-aceitas-free-flow.csv)**, a quinta base aberta, com **15 registros**, um por concessionária em operação: regime de autorização, operadoras publicadas, descontos e regra de moto, com fonte oficial em cada linha.
- Dicionário da nova base em [`dados/README.md`](dados/README.md), com a explicação de por que `operadoras_publicadas` traz `n/d` na maioria das federais.

### Corrigido

- **A RioSP tem 24 pórticos de cobrança, e não 13.** A base `concessionarias-free-flow.csv` ficou com o número antigo da Via Dutra quando a contagem foi corrigida de 10 para 21 pórticos na versão 0.5.0. A soma da coluna `n_porticos_free_flow` nas linhas ativas voltou a bater com o total nacional de 85, que sempre esteve correto nas demais bases e no índice nacional.
- **Nome da PRVias alinhado entre as bases**, de `PRVias (Motiva Paraná)` para `PRVias (Motiva Paraná, ex-CCR RodoNorte)`, como já aparecia em `porticos-free-flow.csv` e no índice nacional.
- **README**: o índice anunciava as bases abertas "em CSV e JSON". Não há espelho JSON no repositório e nunca houve. Corrigido para as cinco bases em CSV.
- **`dados/README.md`**: a tabela de atualização falava em revisão completa "das três bases", quando já eram quatro. Agora são cinco.
- **Quebra de linha dos CSVs padronizada em CRLF.** Três das quatro bases já usavam CRLF, que é o padrão do RFC 4180 e o formato que o Excel espera; `concessionarias-free-flow.csv` estava em LF e passou a acompanhar as demais. Nenhum dado muda, e o dicionário agora declara o formato de arquivo.

### Alterado

- **README**: quatro páginas novas na seção Conteúdos, quinta base na seção Dados abertos, badge de bases abertas, e a seção Tag de Pedágio deixa de prometer conteúdo futuro e passa a linkar o pilar e os três apoios.

### Notas de dado

- **Interoperabilidade nas federais é obrigação legal, não cortesia.** A Lei nº 14.157/2021 determinou a interoperabilidade do pagamento eletrônico de pedágio e a Resolução ANTT nº 4.281/2014 padroniza o sistema de arrecadação e define a figura da **AMAP**, Administradora de Meios de Pagamento para Arrecadação de Pedágio. Autorizada a operadora, todas as concessionárias federais leem a tag dela.
- **A Resolução ANTT nº 6.079/2026, art. 63-D**, deixou explícito que o usuário pode optar entre os sistemas das empresas autorizadas pela ANTT, os sistemas próprios das concessionárias e os sistemas interoperáveis entre concessionárias.
- **Cinco operadoras autorizadas pela ARTESP**, publicadas nominalmente pelas concessionárias Novo Litoral e Tamoios nos próprios sites: ConectCar, Move Mais, Sem Parar, Taggy e Veloe. **Divergência registrada:** parte da cobertura de imprensa cita GreenPass no lugar de Taggy. Adotamos a lista das concessionárias, por hierarquia de fonte.
- **Nenhuma tag no Brasil é homologada para motocicleta**, e a restrição é do sistema, não da operadora. A razão declarada pela ARTESP é segurança nas pistas automáticas com cancela, pelo risco de colisão traseira em caso de falha de abertura. Sem Parar publica no próprio canal de ajuda que a tag só deve ser instalada em carro de passeio, ônibus ou caminhão, e a Via Dutra declara proibido o uso de qualquer tag de pagamento automático em motocicleta. O Free Flow, por não ter cancela, é apontado como o caminho que pode destravar o tema, e a ARTESP afirma que ainda não há solução específica.
- **O prazo de 30 dias é de quem paga pela placa.** Para quem tem tag, o prazo e a forma de pagamento seguem o contrato com a operadora, como a Concessionária Novo Litoral declara no próprio site. Tag inativa ou sem saldo faz a leitura cair para a placa, e o prazo do trecho volta a valer.
- **Passagem cobrada por tag em regra não aparece no portal de pagamento avulso da concessionária**, porque aquele portal lista o que está em aberto. O registro fica no extrato da operadora. Comportamento confirmado na Tamoios e na RioSP.
- **Exceção gaúcha:** a CSG concede o desconto ao usuário que se cadastra no site ou no aplicativo, sem tag, e é o caminho do motociclista naquele trecho. A concessionária declara a tag como forma recomendada de pagamento e aceita vale-pedágio apenas em formato tag.
- **Vale-pedágio é outro produto.** O Vale-Pedágio Obrigatório da Lei nº 10.209/2001 é instrumento de transporte de carga e, desde 2025, existe apenas em meio eletrônico: cartões, cupons e outros meios físicos foram descontinuados pela regulamentação da ANTT.

---

## [0.6.0], 2026-08-26

Hub geográfico, onda 2. Os corredores de praia de São Paulo e os dois estados-âncora do território ganham página própria, e a linha do tempo do repositório passa a cobrir desde a estreia do Free Flow no Brasil.

### Adicionado

- **[`rodovias/free-flow-tamoios.md`](rodovias/free-flow-tamoios.md)**: o pórtico do km 13+500 do Contorno Sul, por que aqui a motocicleta paga, as operadoras de tag autorizadas pela ARTESP, os totens do SAU 3 e SAU 4, e a armadilha da passagem que não aparece no portal avulso quando a cobrança já foi por tag.
- **[`rodovias/free-flow-mogi-bertioga.md`](rodovias/free-flow-mogi-bertioga.md)**: o ponto do km 92+740, o mapa das quatro rodovias da Concessionária Novo Litoral, a isenção total de motos, a ambiguidade do nome Rio-Santos entre SP e RJ, e os dois pórticos de Itariri que só monitoram.
- **[`estados/free-flow-sp.md`](estados/free-flow-sp.md)**: o panorama do estado com mais Free Flow do país, a convivência entre o regime federal da ANTT e o estadual da ARTESP, o que é o Siga Fácil e a tabela de isenção de motos trecho a trecho, que varia dentro do próprio estado.
- **[`estados/free-flow-rs.md`](estados/free-flow-rs.md)**: os seis pórticos do Bloco 3, o marco do primeiro pórtico em rodovia estadual do Brasil, a resposta direta sobre a FreeWay e a explicação de por que o contrato do Bloco 3 lista rodovias que não têm pórtico.
- Pasta **`estados/`**, que vai receber as demais páginas de estado.
- Seções **2024** e **2023** em [`docs/novidades.md`](docs/novidades.md), com seis marcos que faltavam: a estreia da Rio-Santos, o primeiro pórtico estadual do país, os cinco pórticos restantes do Bloco 3, a MG-459, a SP-333 e a Tamoios. A linha do tempo agora cobre desde o início do Free Flow no Brasil.

### Corrigido

- **São Paulo tem 36 pórticos de cobrança, e não 35.** Erro de soma na primeira versão do índice nacional, publicada na 0.5.0. O total nacional de 85 estava certo e não muda.
- **Quilometragem da Concessionária Novo Litoral detalhada por sentido.** Arujá passa a registrar km 37+150 (norte) e 37+780 (sul); Mogi das Cruzes, km 41+600 (norte) e 40+800 (sul). São pontos tarifários únicos com estruturas em quilômetros diferentes por sentido, e a base agora diz isso.
- **Os pórticos de monitoramento de Itariri são dois, e têm quilometragem conhecida:** km 369+860 e km 360+200, na Padre Manoel da Nóbrega. A base registrava um, sem quilometragem.
- **Quilometragem dos pórticos gaúchos refinada** com a casa decimal publicada pela concessionária: São Sebastião do Caí km 4,6; Farroupilha km 45,5; Antônio Prado km 108,3; Ipê km 151,9; Capela de Santana km 30,1.

### Alterado

- **`dados/porticos-free-flow.csv`**: quilometragens, sentidos e observações refinados nos registros da CNL, da CSG e da Tamoios, sem mudança na contagem nacional.
- **`RODOVIAS-COM-FREE-FLOW.md`**: contagem de São Paulo corrigida, quilometragens atualizadas e ponteiros para as páginas de estado.
- **README**: cinco páginas novas na seção Conteúdos.

### Notas de dado

- **Concessionária Novo Litoral:** cinco pontos tarifários ativos, em Arujá e Mogi das Cruzes (SP-088), Bertioga (SP-098), Santos (SP-055 Manoel Hipólito do Rego) e Miracatu (SP-055 Padre Manoel da Nóbrega), mais dois pórticos de monitoramento em Itariri. Motocicletas têm isenção total. Pagamento com Pix ou cartão no site e no app, e presencialmente nos totens de oito bases SAU. A concessionária declara que não envia links nem boletos.
- **Ambiguidade de nome registrada:** em São Paulo, o trecho da SP-055 Doutor Manoel Hipólito do Rego também é chamado de **Rio-Santos**, mesmo nome popular da **BR-101 no Rio de Janeiro**. São rodovias diferentes, de concessionárias diferentes, com regras de isenção opostas quanto a motocicletas.
- **Tamoios:** cobrança de todos os tipos de veículo nos dois sentidos, inclusive motocicletas. Operadoras aceitas são as autorizadas pela ARTESP: ConectCar, Move Mais, Sem Parar, Taggy e Veloe. Pagamento por site, app, ou totens no SAU 3 (km 10,8) e SAU 4 (km 20). Cadastro no site ou app gera alerta a cada passagem. Não pagamento: os dados vão ao DER.
- **Bloco 3 gaúcho:** 271,5 km concedidos por 30 anos à CSG, abrangendo ERS-122, ERS-240, ERS-446, RSC-287, RSC-453 e um trecho da BR-470. **Só as três primeiras têm pórtico.** O projeto prevê segmentação futura dos pórticos, para tornar a cobrança mais proporcional ao trecho, sem data. No Bloco 3 os pórticos substituíram as praças que estavam previstas, então essas rodovias nunca tiveram cabine. Órgão autuador no estado: DAER.
- **BR-290 FreeWay:** confirmado que **não tem Free Flow**. O projeto da ViaSul prevê substituir as sete praças físicas das BR-290, BR-101, BR-386 e BR-448, está **em análise, sem prazo**, e ainda depende de encaminhamento à ANTT. Praças em operação hoje: BR-386 em Montenegro, Paverama, Fontoura Xavier e Victor Graeff; BR-290 em Santo Antônio da Patrulha e Gravataí; BR-101 em Três Cachoeiras.
- **Isenção de motocicleta varia dentro de São Paulo:** pagam na pista expressa da Via Dutra (meia tarifa, com uso de tag proibido), no Rodoanel Norte e no Contorno Sul da Tamoios; são isentas nas quatro rodovias da CNL. A regra vem do contrato de cada concessão.

---

## [0.5.0], 2026-08-26

Hub geográfico, onda 1. O repositório ganha a camada "onde tem", com o mapa nacional pórtico a pórtico, uma base de dados nova e as páginas das três rodovias de maior urgência. Esta versão também traz a maior correção de dado desde a publicação.

### Adicionado

- **[`RODOVIAS-COM-FREE-FLOW.md`](RODOVIAS-COM-FREE-FLOW.md)**, na raiz: o índice nacional pórtico a pórtico, organizado por estado, com município, quilômetro, concessionária, data de início e canal de pagamento. Inclui a seção **Pórticos instalados que ainda não cobram**, que não existe em nenhuma outra fonte e serve para reconhecer cobrança falsa.
- **[`dados/porticos-free-flow.csv`](dados/porticos-free-flow.csv)**, a quarta base aberta, com **49 registros** cobrindo **85 pórticos de cobrança ativos**, 7 pórticos instalados aguardando cobrança e 1 estrutura de monitoramento. É o dado mais granular do repositório: a ANTT publica só as federais e cada concessionária publica só as próprias.
- **[`rodovias/free-flow-dutra.md`](rodovias/free-flow-dutra.md)**: os 21 pontos de cobrança, a regra da pista expressa contra a marginal gratuita, o cálculo proporcional com tarifa dinâmica, a relação com a praça física de Arujá, a janela de duas horas para reentrada, as regras de moto e isenção, e os canais de pagamento com totens e rede credenciada.
- **[`rodovias/free-flow-rio-santos.md`](rodovias/free-flow-rio-santos.md)**: os três pórticos de Itaguaí, Mangaratiba e Paraty, a comparação com o modelo da Dutra, a lista de isentos, os totens ao longo da rodovia e o registro histórico da primeira operação de Free Flow do país.
- **[`rodovias/free-flow-anchieta-imigrantes.md`](rodovias/free-flow-anchieta-imigrantes.md)**: página de acompanhamento de um fato em movimento. Por que ainda não cobra, onde ficam os pórticos, a realocação do ponto da subida, o que muda no modelo tarifário, a linha do tempo dos adiamentos e o que acontece com as praças físicas.
- Nota de **19 de julho de 2026** em [`docs/novidades.md`](docs/novidades.md), sobre a realocação do pórtico da Imigrantes no sentido capital, que faltava na linha do tempo e é a causa do adiamento seguinte.
- Dicionário da nova base em [`dados/README.md`](dados/README.md), com o critério de contagem de pórticos e a explicação de por que alguns registros são agregados.

### Corrigido

- **A Via Dutra tem 21 pontos de cobrança, e não 10.** A contagem publicada desde o PAC-01 estava errada. Quatro fontes independentes convergem em 21 pontos entre o km 204 (Arujá) e o km 231 (São Paulo), e a própria concessionária informa 19 acessos à pista expressa. Corrigido na base, no README, no badge e na tabela nacional.
- **O trecho começa no km 204, e não no km 206.** Comunicações oficiais da concessionária e da ANTT indicam km 231 ao km 204.
- **Total nacional recontado: de 74 para 85 pórticos de cobrança em operação.** A mudança decorre integralmente da correção da Dutra. O número de rodovias, concessionárias e estados não muda: seguem 26, 15 e 7.

### Alterado

- **`dados/rodovias-free-flow.csv`**: linha da Via Dutra corrigida em `n_porticos` e `trecho`, com a data de verificação atualizada.
- **README**: badge de pórticos, resposta extraível, tabela nacional, total ao pé da tabela, seção Conteúdos com as quatro páginas novas, seção de dados abertos com a quarta base e ponteiro para o índice nacional.
- **`O-QUE-E-FREE-FLOW.md`** e **`docs/novidades.md`**: contagem nacional atualizada e nota de 06/12/2025 corrigida com o número de pontos, o quilômetro inicial e o modelo de cobrança da Dutra.

### Notas de dado

- **Via Dutra, trecho metropolitano:** 21 pontos de cobrança entre o km 204 e o km 231, instalados nas entradas e saídas das pistas expressas, com 19 acessos. Cobrança **proporcional ao trecho percorrido**, com tarifa que varia por dia, horário e condições de fluxo. A pista marginal é gratuita. A praça física de Arujá segue em operação, e quem usa a expressa até ela, ou a partir dela, não paga a tarifa do Free Flow. Quem sai da expressa tem até 2 horas para retornar sem cobrança extra. Motocicletas pagam meia tarifa na expressa e é proibido usar tag em moto. Ônibus, vans e táxis não são isentos. A concessionária não emite boletos e a passagem fica disponível para pagamento em até 48 horas.
- **Rio-Santos:** cobrança **por pórtico**, com valor fechado, e não proporcional à distância, conforme a própria ANTT informou no anúncio de início. Isentos: motocicletas, motonetas, triciclos, bicicletas, ambulâncias, veículos oficiais e do Corpo de Bombeiros. Operação assistida desde 30/01/2023 e cobrança a partir de março de 2023.
- **Sistema Anchieta-Imigrantes:** pórticos instalados em fevereiro de 2026, testes desde o fim de maio, início previsto para 01/07/2026, remarcado para 01/08/2026 em 13/07, com o pórtico da subida realocado em 19/07 do km 29 para depois do km 38, e o início adiado de novo em 27/07 **sem nova data**. No período de testes, 93% dos veículos comerciais e 71% dos de passeio já tinham tag ativa. Os pórticos integram o programa Muralha Paulista.
- **Critério de contagem declarado:** contam-se pórticos **de cobrança**; onde há um por sentido no mesmo ponto, os dois entram; estrutura de monitoramento nunca entra. Registros agregados são usados onde a concessionária não publica a quilometragem individual, com `km` em `n/d`.

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

- **A contagem do prazo de 30 dias, de novo, e agora completa.** A versão 0.3.0 dizia que os 30 dias contam da confirmação do processamento do registro. Está certo para a **infração de trânsito**, mas incompleto: a Resolução ANTT nº 6.079/2026 conta **da passagem pelo pórtico** para efeito dos **encargos financeiros** nas rodovias federais concedidas. As duas fontes são oficiais e tratam de planos distintos. A divergência agora está registrada em tabela no README, em [`docs/como-pagar.md`](docs/como-pagar.md), em [`O-QUE-E-FREE-FLOW.md`](O-QUE-E-FREE-FLOW.md), em [`docs/consulta-app-cnh-do-brasil.md`](docs/consulta-app-cnh-do-brasil.md) e, com o detalhamento completo, em [`docs/prazo-e-encargos.md`](docs/prazo-e-encargos.md).
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

- **Contagem do prazo de pagamento.** O repositório dizia "até 30 dias após a passagem". A Deliberação CONTRAN nº 277/2026 alterou o art. 7º da Resolução CONTRAN nº 1.013/2024, e o prazo de 30 dias passou a ser contado **da confirmação do processamento do registro da passagem** junto ao órgão máximo executivo de trânsito da União. Corrigido no README e em [`O-QUE-E-FREE-FLOW.md`](O-QUE-E-FREE-FLOW.md), com a ressalva de extensão para o próximo dia útil.
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

- **[`O-QUE-E-FREE-FLOW.md`](O-QUE-E-FREE-FLOW.md)**, a explicação completa do sistema: como o pórtico identifica o veículo, o que muda com tag e sem tag, prazo de pagamento, descontos DBT e DUF, consequências do não pagamento e por que o país está trocando a praça pelo pórtico.
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

[Não publicado]: https://github.com/TRIWI-SEO/SEM-PARAR-FREE-FLOW/compare/v0.6.0...HEAD
[0.6.0]: https://github.com/TRIWI-SEO/SEM-PARAR-FREE-FLOW/releases/tag/v0.6.0
[0.5.0]: https://github.com/TRIWI-SEO/SEM-PARAR-FREE-FLOW/releases/tag/v0.5.0
[0.4.0]: https://github.com/TRIWI-SEO/SEM-PARAR-FREE-FLOW/releases/tag/v0.4.0
[0.3.0]: https://github.com/TRIWI-SEO/SEM-PARAR-FREE-FLOW/releases/tag/v0.3.0
[0.2.0]: https://github.com/TRIWI-SEO/SEM-PARAR-FREE-FLOW/releases/tag/v0.2.0
[0.1.0]: https://github.com/TRIWI-SEO/SEM-PARAR-FREE-FLOW/releases/tag/v0.1.0
