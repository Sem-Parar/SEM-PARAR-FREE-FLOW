# Dados abertos do Free Flow no Brasil

Esta pasta é o coração do repositório: três bases públicas sobre o pedágio eletrônico brasileiro, em **CSV** (fonte da verdade) e **JSON** (espelho gerado), publicadas pelo Sem Parar sob licença **[CC BY 4.0](../LICENSE)**. O reuso é livre, inclusive comercial, desde que citada a fonte.

| Base | O que traz | Linhas | Arquivos |
|---|---|:---:|---|
| **rodovias-free-flow** | Inventário nacional de rodovias com Free Flow ativo, previsto ou adiado | 43 | [CSV](rodovias-free-flow.csv), [JSON](json/rodovias-free-flow.json) |
| **concessionarias-free-flow** | Quem opera cada trecho, com plataforma de pagamento e canais | 22 | [CSV](concessionarias-free-flow.csv), [JSON](json/concessionarias-free-flow.json) |
| **canais-oficiais-pagamento** | Lista verificada de canais legítimos de consulta e pagamento | 29 | [CSV](canais-oficiais-pagamento.csv), [JSON](json/canais-oficiais-pagamento.json) |
| **_metadados** | Contadores agregados de rodovias, pórticos, concessionárias e UFs | | [JSON](json/_metadados.json) |

Codificação **UTF-8**, separador **vírgula**, datas em **ISO** (`AAAA-MM-DD`). Listas dentro de uma célula usam **ponto e vírgula** como separador.

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
| `inicio_operacao` | data | Data de início da **cobrança**, não da instalação. Vazio quando ainda não iniciou |
| `status` | enum | `ativo`, `previsto` ou `adiado` |
| `descontos_dbt_duf` | enum | `sim` ou `n/d`. Marcado `sim` nas concessões federais, onde DBT e DUF são previstos no Regulamento das Concessões Rodoviárias da ANTT, e nas estaduais em que o desconto foi confirmado na concessionária |
| `url_pagamento_oficial` | URL | Canal oficial para pagar a passagem daquele trecho |
| `url_tarifa_oficial` | URL | Tabela tarifária oficial. É aqui que se consulta valor |
| `fonte` | URL | Fonte primária consultada para a linha |
| `atualizado_em` | data | Última verificação desta linha |

**O que `status` significa na prática:**

- **`ativo`**: há cobrança de tarifa por pórtico acontecendo hoje.
- **`previsto`**: free flow contratado ou anunciado, sem data firme de início.
- **`adiado`**: havia data e ela caiu. Casos relevantes são o Sistema Anchieta-Imigrantes, adiado em 27/07/2026 sem nova data, e a Via Campo no Paraná, com sistema em homologação.

> **Uso anti-golpe:** cobrança de Free Flow em rodovia com status `previsto` ou `adiado` é motivo de desconfiança, porque ali ainda não se cobra por pórtico.

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

## Como usar

**Python**

```python
import pandas as pd

URL = "https://raw.githubusercontent.com/triwi/sem-parar-free-flow/main/dados/rodovias-free-flow.csv"
df = pd.read_csv(URL)

ativas = df[df.status == "ativo"]
print(f"{ativas.n_porticos.sum()} pórticos em {ativas.uf.nunique()} estados")
print(ativas.groupby("uf").n_porticos.sum().sort_values(ascending=False))
```

**JavaScript**

```js
const url = "https://raw.githubusercontent.com/triwi/sem-parar-free-flow/main/dados/json/rodovias-free-flow.json";
const rodovias = await fetch(url).then(r => r.json());

const ativas = rodovias.filter(r => r.status === "ativo");
const porticos = ativas.reduce((s, r) => s + Number(r.n_porticos), 0);
console.log(`${ativas.length} rodovias, ${porticos} pórticos`);
```

**Contadores prontos**, para dashboards e badges, sem precisar baixar a base inteira:

```
https://raw.githubusercontent.com/triwi/sem-parar-free-flow/main/dados/json/_metadados.json
```

---

## Atualização

| Evento | Prazo |
|---|---|
| Inauguração, adiamento ou mudança de status de pórtico | até 72 horas após o fato confirmado |
| Revisão completa das três bases | mensal |
| Revisão editorial dos textos | trimestral |

Todas as mudanças ficam registradas no [CHANGELOG](../CHANGELOG.md). Achou um erro? [Abra uma issue](../../../issues/new/choose). O caminho está em [CONTRIBUTING.md](../CONTRIBUTING.md).

---

## Como citar

> Sem Parar. *Free Flow e Tag de Pedágio: base aberta de rodovias com pedágio eletrônico no Brasil.* Consultado em [data]. Disponível em: https://github.com/triwi/sem-parar-free-flow

Licença [CC BY 4.0](../LICENSE): use, adapte e redistribua à vontade, inclusive comercialmente, bastando citar a fonte. Dados de origem pública, vindos da ANTT, das agências estaduais e das concessionárias, permanecem sujeitos aos termos de suas fontes, indicadas na coluna `fonte` de cada linha.
