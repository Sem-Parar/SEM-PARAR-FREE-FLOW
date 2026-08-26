# Dados abertos do Free Flow no Brasil

Esta pasta é o coração do repositório: sete bases públicas sobre o pedágio eletrônico brasileiro, em **CSV**, publicadas pelo Sem Parar sob licença **[CC BY 4.0](../LICENSE)**. O reuso é livre, inclusive comercial, desde que citada a fonte.

| Base | O que traz | Linhas |
|---|---|:---:|
| [rodovias-free-flow](rodovias-free-flow.csv) | Inventário nacional de rodovias com Free Flow ativo, previsto ou adiado | 46 |
| [porticos-free-flow](porticos-free-flow.csv) | Inventário pórtico a pórtico, com município, quilômetro, sentido e situação | 64 |
| [concessionarias-free-flow](concessionarias-free-flow.csv) | Quem opera cada trecho, com plataforma de pagamento e canais | 24 |
| [canais-oficiais-pagamento](canais-oficiais-pagamento.csv) | Lista verificada de canais legítimos de consulta e pagamento | 29 |
| [tags-aceitas-free-flow](tags-aceitas-free-flow.csv) | Aceitação de tag por concessionária, com regime de autorização, operadoras publicadas e descontos | 15 |
| [base-legal-free-flow](base-legal-free-flow.csv) | As leis, resoluções e portarias que sustentam o Free Flow, com o que cada uma define | 12 |
| [homologacao-senatran-free-flow](homologacao-senatran-free-flow.csv) | Homologações de sistema de livre passagem pela Senatran, com número e data de portaria | 12 |

Codificação **UTF-8**, separador **vírgula**, quebra de linha **CRLF** (padrão RFC 4180, que é o que o Excel espera), datas em **ISO** (`AAAA-MM-DD`). Listas dentro de uma célula usam **ponto e vírgula** como separador.

---

## Três regras que valem para todas as bases

**1. Nenhum valor monetário é armazenado.** Não há tarifa em reais nem percentual de desconto em lugar nenhum. Esses números mudam com frequência e um dataset com valor congelado engana mais do que ajuda. O que guardamos é o campo `url_tarifa_oficial`, com o link da tabela da concessionária, que está sempre atualizada na origem.

**2. `n/d` em vez de chute.** Campo não confirmado em fonte oficial aparece como `n/d`. Nenhum dado aqui foi inferido, deduzido ou preenchido por analogia.

**3. Divergência se registra.** Quando a ANTT e a concessionária publicam quilometragens diferentes para o mesmo pórtico, e isso acontece, adotamos o valor da ANTT e anotamos a divergência no campo `trecho`.

---

## `rodovias-free-flow.csv`

Uma linha por **rodovia e concessionária**. Uma mesma concessão pode ocupar várias linhas quando abrange rodovias diferentes. A EPR Iguaçu, por exemplo, aparece em BR-163, PR-182 e PR-280.

| Coluna | Tipo | Descrição |
|---|---|---|
| `rodovia` | texto | Nome usual do trecho ou da concessão, como `Rio-Santos (Costa Verde)` |
| `sigla` | texto | Designação oficial: `BR-101`, `SP-270`, `ERS-122`, `MG-459` |
| `uf` | texto | Sigla do estado. Múltiplos estados separados por ponto e vírgula |
| `trecho` | texto | Extensão, municípios e localização dos pórticos. Também abriga notas de divergência e menção a pórticos que só monitoram |
| `concessionaria` | texto | Razão social ou nome usual da concessionária responsável |
| `grupo_economico` | texto | Grupo controlador, quando confirmado. `n/d` quando não |
| `esfera` | enum | `federal` ou `estadual` |
| `orgao_regulador` | texto | `ANTT`, `ARTESP`, `AGERGS`, `DER-MG`, `AGER-MT`, `AGEMS` |
| `n_porticos` | inteiro | Pórticos **de cobrança** em operação. Estruturas que só monitoram tráfego não entram na contagem |
| `inicio_operacao` | data | Data de início da **cobrança**, não da instalação. Em linhas com status `previsto`, traz a data anunciada quando existe, e fica vazia quando não há data divulgada |
| `status` | enum | `ativo`, `previsto` ou `adiado` |
| `descontos_dbt_duf` | enum | `sim` ou `n/d`. Marcado `sim` nas concessões federais, onde DBT e DUF são previstos no Regulamento das Concessões Rodoviárias da ANTT, e nas estaduais em que o desconto foi confirmado na concessionária |
| `url_pagamento_oficial` | URL | Canal oficial para pagar a passagem daquele trecho |
| `url_tarifa_oficial` | URL | Tabela tarifária oficial. É aqui que se consulta valor |
| `fonte` | URL | Fonte primária consultada para a linha |
| `atualizado_em` | data | Última verificação desta linha |

**O que `status` significa na prática:**

- **`ativo`**: há cobrança de tarifa por pórtico acontecendo hoje.
- **`previsto`**: free flow contratado ou anunciado, com ou sem data de início divulgada. Quando há data anunciada, ela está em `inicio_operacao`.
- **`adiado`**: havia data e ela caiu. Casos relevantes são o Sistema Anchieta-Imigrantes, adiado em 27/07/2026 sem nova data, e a Via Campo no Paraná, com sistema em homologação.

> **Uso anti-golpe:** cobrança de Free Flow em rodovia com status `previsto` ou `adiado` é motivo de desconfiança, porque ali ainda não se cobra por pórtico.

---

## `porticos-free-flow.csv`

O dado mais granular do repositório, e o que nenhuma outra fonte reúne em âmbito nacional: a ANTT cobre só as federais, cada concessionária cobre só as próprias.

| Coluna | Tipo | Descrição |
|---|---|---|
| `rodovia` | texto | Nome usual do trecho ou da concessão |
| `sigla` | texto | Designação oficial: `BR-116`, `SP-270`, `ERS-122`, `MG-459` |
| `uf` | texto | Sigla do estado |
| `municipio` | texto | Município onde o pórtico está instalado. Vários municípios separados por ponto e vírgula, quando o registro é agregado |
| `km` | texto | Quilometragem, no formato usado pela fonte oficial (`414`, `092+740`, `156,1`). `n/d` quando a concessionária não publica |
| `sentido` | texto | `ambos`, ou o sentido específico quando a cobrança é assimétrica, como na Rodovia dos Imigrantes |
| `porticos_no_registro` | inteiro | Quantos pórticos **de cobrança** aquele registro representa. A soma da coluna, nas linhas com `status = ativo`, é o total nacional |
| `tipo` | enum | `cobranca` ou `monitoramento` |
| `concessionaria` | texto | Concessionária responsável |
| `data_ativacao` | data | Início da **cobrança** naquele ponto. Vazio quando não há cobrança |
| `status` | enum | `ativo`, `monitoramento` ou `instalado_aguardando` |
| `observacao` | texto | Particularidades, divergências e por que um registro é agregado |
| `fonte` | URL | Fonte primária consultada |
| `atualizado_em` | data | Última verificação |

**O que `status` significa aqui:**

- **`ativo`**: o pórtico cobra tarifa hoje.
- **`monitoramento`**: a estrutura existe e só monitora tráfego, sem previsão de cobrar.
- **`instalado_aguardando`**: o pórtico está instalado e a cobrança foi adiada ou ainda não começou. É o caso do Sistema Anchieta-Imigrantes e dos trechos da Rota Sorocabana.

**Como contamos um pórtico.** Contamos pórticos **de cobrança**. Onde a concessionária opera um por sentido no mesmo ponto, os dois entram, porque são duas cobranças possíveis. Estrutura de monitoramento nunca entra na contagem.

**Todo pórtico ativo tem quilometragem.** Até agosto de 2026 esta base trazia registros agregados, com `km = n/d`, para a BR-381, a BR-364 e as duas rodovias da Rota Verde em Goiás, porque as concessionárias não publicavam a posição individual. O cadastro de pórticos das concessões federais da ANTT trouxe essas quilometragens, e os registros agregados foram desmembrados em uma linha por pórtico. **Nenhuma linha ativa aparece hoje com `km = n/d`.**

**A divergência da Via Dutra, registrada e em aberto.** A concessionária comunica **21 pontos de cobrança** na pista expressa entre os km 204 e 231; o cadastro da ANTT registra **10 pórticos** entre os km 206 e 231,3, anotando que **cada pórtico concentra vários pontos de cobrança de entrada e saída**. São unidades de medida diferentes para a mesma realidade física, e não um erro de uma das partes. Esta base adota **21**, o número da concessionária, e o registro do trecho traz a faixa de quilometragem em vez de uma posição por linha. É a única linha ativa que não tem um pórtico por registro, e a observação da linha descreve a divergência. **Se o critério for revisto para contar estruturas físicas, o total nacional muda**, e por isso a escolha está declarada aqui em vez de embutida no número.

> **Uso anti-golpe:** as linhas com `status` diferente de `ativo` são a lista de pórticos que **existem mas não cobram**. Cobrança apresentada em qualquer um deles é motivo de desconfiança.

---

## `concessionarias-free-flow.csv`

Uma linha por concessionária. Responde à pergunta que mais confunde o motorista: passei, mas pago para quem?

| Coluna | Tipo | Descrição |
|---|---|---|
| `concessionaria` | texto | Razão social ou nome usual |
| `grupo_economico` | texto | Grupo controlador, quando confirmado |
| `plataforma_pagamento` | texto | Plataforma que processa o pagamento, como `Pedágio Digital`, `Movvia` ou `própria`, com o nome do produto entre parênteses |
| `rodovias` | texto | Siglas das rodovias operadas com free flow, separadas por ponto e vírgula |
| `ufs` | texto | Estados de atuação, separados por ponto e vírgula |
| `esfera` | enum | `federal` ou `estadual` |
| `n_porticos_free_flow` | inteiro | Total de pórticos de cobrança da concessionária |
| `status` | enum | `ativo`, `previsto` ou `adiado` |
| `canais` | texto | Meios de atendimento e pagamento disponíveis, separados por ponto e vírgula |
| `url_oficial` | URL | Página oficial de free flow da concessionária |
| `observacao` | texto | Particularidades do trecho, como isenções, prazos próprios, decisões judiciais e avisos |
| `fonte` | URL | Fonte primária consultada |
| `atualizado_em` | data | Última verificação |

O campo `observacao` costuma ser o mais útil, porque é onde ficam as exceções que quebram a regra geral: trechos em que motos não são isentas, concessionárias com prazo menor que 30 dias, passagens por tag que não aparecem no app da concessionária.

---

## `canais-oficiais-pagamento.csv`

A camada anti-golpe. Cada canal foi acessado e conferido individualmente, com o nível de verificação declarado, inclusive quando a conferência não foi completa.

| Coluna | Tipo | Descrição |
|---|---|---|
| `canal` | texto | Nome do canal |
| `operador` | texto | Empresa ou órgão responsável |
| `tipo` | enum | `site`, `app`, `governo` ou `tag` |
| `url_oficial` | URL | Endereço oficial exato |
| `funcao` | enum | `consulta`, `pagamento`, `informação` ou `tag` |
| `quem_pode_usar` | texto | Quem é atendido por aquele canal, e quem não é |
| `observacao` | texto | Limitações, alertas e particularidades |
| `verificacao` | enum | `verificado` ou uma das variações de `parcial` |
| `verificado_em` | data | Data da conferência |

**O que cada nível de `verificacao` quer dizer:**

- **`verificado`**: a página foi acessada e o conteúdo conferido.
- **`parcial (bloqueio anti-bot)`**: o site recusa acesso automatizado, com erro 403, mas o endereço está confirmado por citação explícita em fonte oficial primária. É o caso de portais grandes, como o Pedágio Digital.
- **`parcial`**: endereço confirmado por fonte oficial, com conferência incompleta.
- **`parcial (instabilidade no acesso)`**: o canal apresentou falha de resposta no momento da checagem.

### Três coisas que este arquivo deixa explícitas

**Nenhum canal de governo recebe pagamento.** ANTT, app CNH do Brasil, Portal Senatran e Siga Fácil apenas mostram a passagem e encaminham à concessionária. Qualquer tela com marca de governo pedindo dados de cartão para quitar pedágio é fraude.

**Portal integrador cobre menos do que aparenta.** Plataformas que reúnem várias concessionárias processam pagamento apenas das que estão efetivamente integradas, embora publiquem páginas informativas sobre dezenas de outras. A coluna `quem_pode_usar` diz exatamente o alcance de cada uma.

**Cobrança legítima nunca chega por mensagem.** Nem a ANTT nem as concessionárias enviam cobrança por WhatsApp, e-mail, SMS ou anúncio. Quem inicia o pagamento é o motorista, digitando o endereço, nunca clicando em link recebido.

---

## `tags-aceitas-free-flow.csv`

Uma linha por **concessionária com Free Flow em operação**. Responde à pergunta que o motorista faz antes da viagem: a minha tag funciona nesse pórtico?

O recorte é deliberado. Só entram as concessionárias que **cobram hoje**, porque aceitação de tag em trecho que ainda não cobra é informação sem uso e que muda até a inauguração.

| Coluna | Tipo | Descrição |
|---|---|---|
| `concessionaria` | texto | Razão social ou nome usual, no mesmo padrão de `concessionarias-free-flow.csv` |
| `uf` | texto | Estados de atuação, separados por ponto e vírgula |
| `esfera` | enum | `federal` ou `estadual` |
| `orgao_regulador` | texto | `ANTT`, `ARTESP`, `AGERGS`, `DER-MG` |
| `aceita_tag` | enum | `sim`, `nao` ou `n/d` |
| `regime_de_aceitacao` | texto | De onde vem a autorização: `interoperabilidade obrigatoria (ANTT)` nas federais, ou a lista da agência estadual |
| `operadoras_publicadas` | texto | Operadoras nomeadas **pela própria concessionária**, separadas por ponto e vírgula. `n/d` quando ela não publica lista própria |
| `moto_pode_usar_tag` | enum | `nao` em todas as linhas. Nenhuma tag no Brasil é homologada para motocicleta, e o campo existe para que a resposta esteja completa em qualquer linha lida isoladamente |
| `desconto_por_tag` | texto | `DBT`, `DUF`, `DBT; DUF` ou `n/d`. **Nunca percentual** |
| `prazo_com_tag` | texto | Em regra `definido pela operadora de tag`. O prazo de 30 dias é o de quem paga pela placa, não o de quem tem tag |
| `observacao` | texto | Exceções do trecho: isenção de moto, proibição de tag em moto, cadastro sem tag, vale-pedágio |
| `fonte` | URL | Fonte primária consultada para a linha |
| `atualizado_em` | data | Última verificação |

**Por que tantos `n/d` em `operadoras_publicadas`.** Nas rodovias federais a interoperabilidade é obrigatória: autorizada pela ANTT, a operadora é lida por qualquer pórtico federal. Publicar lista ali seria redundante, e a maioria das concessionárias federais não publica. Preferimos registrar `n/d` e explicar o regime na coluna ao lado a inventar uma lista.

**Divergência registrada.** As concessionárias Novo Litoral e Tamoios publicam a mesma lista de cinco operadoras autorizadas pela ARTESP: ConectCar, Move Mais, Sem Parar, Taggy e Veloe. Parte da cobertura de imprensa cita GreenPass no lugar de Taggy. Adotamos a lista publicada pelas próprias concessionárias, por hierarquia de fonte, e a divergência está anotada na página [Quais tags funcionam no Free Flow](../docs/tags-aceitas-no-free-flow.md).

> **Uso anti-golpe:** operadora de tag que não consta em nenhuma lista oficial e cobra adesão por link recebido em mensagem é motivo de desconfiança. Quem autoriza operadora de tag é a ANTT nas federais e a agência reguladora nas estaduais.

---

## `base-legal-free-flow.csv`

Uma linha por **norma**. Responde à pergunta que sustenta todo o resto: com base em quê se cobra, e com base em quê se multa.

O recorte inclui leis, resoluções, deliberações e portarias em vigor, mais a Resolução CONTRAN nº 984/2022, que foi substituída mas cujos atos seguem produzindo efeitos por regra de transição.

| Coluna | Tipo | Descrição |
|---|---|---|
| `norma` | texto | Identificação usual, como `Lei nº 14.157/2021` ou `Art. 209-A do CTB` |
| `tipo` | enum | `lei federal`, `artigo de lei`, `resolução`, `deliberação` ou `portaria` |
| `orgao` | texto | Quem editou: `Congresso Nacional`, `ANTT`, `CONTRAN` ou `Senatran` |
| `data_publicacao` | data | Data de publicação, em ISO |
| `o_que_estabelece` | texto | Resumo do conteúdo normativo, sem interpretação |
| `aplica_se_a` | texto | Alcance: `todo o país`, `rodovias federais concedidas` ou `transporte de carga` |
| `vigencia` | texto | `vigente`, `vigente até` com data, ou a norma que a substituiu |
| `relevancia_para_o_motorista` | texto | Por que aquela norma importa na prática de quem dirige |
| `url_oficial` | URL | Endereço do texto oficial |
| `fonte` | URL | Fonte primária consultada |
| `atualizado_em` | data | Última verificação |

**Por que a coluna `relevancia_para_o_motorista` existe.** Uma lista de normas sem tradução é inútil para quem não é advogado. Essa coluna é o único campo interpretativo da base, e ele diz o efeito prático, não a opinião sobre o mérito.

> **Uso anti-golpe:** páginas falsas de pedágio costumam citar o art. 209-A com texto inventado. O texto real está nesta base e no [pilar da base legal](../BASE-LEGAL-DO-FREE-FLOW.md).

---

## `homologacao-senatran-free-flow.csv`

Uma linha por **homologação de sistema de livre passagem** publicada pela Senatran. Importa porque, pela Portaria Senatran nº 442/2025, art. 8º, § 2º, sistema não homologado não pode ser usado para os fins do art. 115, § 10 do CTB, o que afasta a infração do art. 209-A.

| Coluna | Tipo | Descrição |
|---|---|---|
| `concessionaria_na_portaria` | texto | Razão social exatamente como aparece na portaria |
| `concessionaria_no_repositorio` | texto | Nome usado nas demais bases, para permitir o cruzamento. `n/d` quando a concessionária ainda não consta no inventário |
| `cnpj` | texto | CNPJ informado na portaria |
| `portaria_senatran` | inteiro | Número da portaria de homologação |
| `data_publicacao` | data | Data de publicação da portaria |
| `uf` | texto | Estados de atuação, separados por ponto e vírgula |
| `cobra_por_portico_hoje` | enum | `sim`, `nao` ou `n/d`. **Homologação não é início de cobrança** |
| `observacao` | texto | Particularidades relevantes |
| `fonte` | URL | Página de portarias da Senatran |
| `atualizado_em` | data | Última verificação |

**A coluna `cobra_por_portico_hoje` existe por um motivo específico.** A Ecovias dos Imigrantes teve o sistema homologado e não cobra: os pórticos do Sistema Anchieta-Imigrantes estão instalados e a cobrança segue adiada. Sem essa coluna, a base induziria ao erro de tratar homologação como sinal de que a rodovia já cobra.

**Limite declarado desta base.** Ela reúne as homologações que localizamos na página de portarias da Senatran, e não é uma extração oficial consolidada. Concessionárias ativas que não aparecem aqui podem ter sido homologadas em portaria que não localizamos. **A ausência de uma linha não é afirmação de que a concessionária não foi homologada.**

---

## Como abrir

Clique no arquivo, depois no botão **Download raw file**, no canto superior direito. O arquivo baixa em CSV e abre direto no Excel, no Numbers ou no Google Sheets.

Se o Excel embaralhar os acentos, abra pelo menu Dados, opção "De Texto/CSV", e escolha a codificação UTF-8.

---

## Atualização

| Evento | Prazo |
|---|---|
| Inauguração, adiamento ou mudança de status de pórtico | até 72 horas após o fato confirmado |
| Revisão completa das sete bases | mensal |
| Revisão editorial dos textos | trimestral |

Todas as mudanças ficam registradas no [CHANGELOG](../CHANGELOG.md). Achou um erro? [Abra uma issue](../../../issues/new). O caminho está em [CONTRIBUTING.md](../CONTRIBUTING.md).

---

## Como citar

> Sem Parar. *Free Flow e Tag de Pedágio: base aberta de rodovias com pedágio eletrônico no Brasil.* Consultado em [data]. Disponível em: https://github.com/TRIWI-SEO/SEM-PARAR-FREE-FLOW

Licença [CC BY 4.0](../LICENSE): use, adapte e redistribua à vontade, inclusive comercialmente, bastando citar a fonte. Dados de origem pública, vindos da ANTT, das agências estaduais e das concessionárias, permanecem sujeitos aos termos de suas fontes, indicadas na coluna `fonte` de cada linha.
