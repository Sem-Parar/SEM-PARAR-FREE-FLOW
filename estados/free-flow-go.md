# Free Flow em Goiás: onde tem, quem cobra e como pagar

**Goiás tem 11 pórticos de cobrança de Free Flow, todos operados pela Rota Verde Goiás, em duas rodovias federais: a BR-060, entre o Anel Viário de Goiânia e o Contorno de Rio Verde, e a BR-452, entre Rio Verde e Itumbiara. A cobrança começou em 27 de maio de 2026 e foi o primeiro pedágio eletrônico do estado. É também a concessão com o maior número de pontos em fluxo livre do cadastro federal da ANTT.**

Uma particularidade goiana: na BR-060 os pórticos operam **em pares**, um por sentido, com quilometragens distintas para cada lado da pista.

> Publicado em 26 de agosto de 2026. Última atualização em 26 de agosto de 2026.
> Parte do repositório [Free Flow e Tag de Pedágio, pelo Sem Parar](../README.md). Base de dados em [`dados/porticos-free-flow.csv`](../dados/porticos-free-flow.csv).

---

## Índice

- [Os 11 pórticos, um a um](#os-11-pórticos-um-a-um)
- [Sete pontos de cobrança, onze estruturas](#sete-pontos-de-cobrança-onze-estruturas)
- [Onde pagar](#onde-pagar)
- [O desconto que cresce até a trigésima passagem](#o-desconto-que-cresce-até-a-trigésima-passagem)
- [A concessionária não vende tag](#a-concessionária-não-vende-tag)
- [Uma segunda concessão a caminho](#uma-segunda-concessão-a-caminho)
- [Perguntas frequentes](#perguntas-frequentes)
- [Fontes oficiais](#fontes-oficiais)

---

## Os 11 pórticos, um a um

Verificado em **26 de agosto de 2026**. Quilometragens do cadastro de pórticos das concessões federais da ANTT.

| Rodovia | Município | Km | Pórticos | Desde |
|---|---|:---:|:---:|:---:|
| **BR-060** | Abadia de Goiás | 172 e 182,6 | 2 | 27/05/2026 |
| **BR-060** | Indiara | 233,75 e 233,85 | 2 | 27/05/2026 |
| **BR-060** | Jandaia | 281,6 e 281,7 | 2 | 27/05/2026 |
| **BR-060** | Acreúna | 325,89 e 326 | 2 | 27/05/2026 |
| **BR-452** | Santa Helena de Goiás | 44,9 | 1 | 27/05/2026 |
| **BR-452** | Bom Jesus de Goiás | 99,85 | 1 | 27/05/2026 |
| **BR-452** | Bom Jesus de Goiás | 147,59 | 1 | 27/05/2026 |

**Total de 11 pórticos de cobrança**, todos da **Rota Verde Goiás**, concessão federal regulada pela ANTT. Goiás é o terceiro estado do país em número de pórticos, atrás de São Paulo e Paraná.

A concessão cobre **229,6 quilômetros na BR-060** e **196,6 quilômetros na BR-452**, ligando a região metropolitana de Goiânia ao sul do estado e à divisa com Minas Gerais.

O mapa nacional está em [Rodovias com Free Flow no Brasil](../RODOVIAS-COM-FREE-FLOW.md).

---

## Sete pontos de cobrança, onze estruturas

Aqui está a informação que evita erro de conta.

Na **BR-060**, os pórticos são instalados **em pares, um por sentido**, e o cadastro da ANTT registra quilometragens diferentes para cada lado. Em Abadia de Goiás, por exemplo, um fica no km 172 e o outro no km 182,6. Em Indiara, no km 233,75 e no 233,85.

Na **BR-452**, os três pórticos são **únicos**, com cobrança nos dois sentidos.

| | BR-060 | BR-452 |
|---|:---:|:---:|
| **Pontos de cobrança** | 4 | 3 |
| **Estruturas de pórtico** | 8 | 3 |
| **Modelo** | Par por sentido | Pórtico único |

Ou seja: **7 pontos tarifários, 11 estruturas físicas.** Quem atravessa a BR-060 num sentido cruza quatro pontos de cobrança, não oito.

Este repositório conta **estruturas de cobrança**, e é por isso que o número publicado aqui é 11. O critério está declarado no [dicionário de dados](../dados/README.md).

---

## Onde pagar

| Canal | Endereço ou local |
|---|---|
| **Site** | [pedagioeletronico.rotaverdegoias.com.br](https://pedagioeletronico.rotaverdegoias.com.br) |
| **App** | Rota Verde Goiás |
| **Totens** | Nas 9 bases do Serviço de Atendimento ao Usuário |
| **Tag** | Cobrança automática, com desconto |

O prazo sem tag é de **30 dias** a partir da passagem. A concessionária permite cadastrar a placa no site para acompanhar as passagens.

O guia completo, com o de-para de concessionária para canal, está em [Como pagar o pedágio Free Flow](../docs/como-pagar.md).

---

## O desconto que cresce até a trigésima passagem

A Rota Verde aplica o **Desconto de Usuário Frequente**, e a mecânica dela é uma das mais detalhadas do país. Vale entender porque muda o cálculo de quem roda todo dia:

- Vale para **veículos de passeio**, categorias 1, 3 e 5.
- Exige **pagamento automático por tag**, com cobrança pela antena.
- É **progressivo**: começa a partir da **segunda passagem** pelo mesmo pórtico, no mesmo sentido, dentro do mês.
- Cresce a cada passagem até a **trigésima**, quando o valor com desconto fica fixo até o último dia do mês.
- O cálculo é automático, cobrado já com desconto na fatura da operadora de tag.

Existe também o **Desconto Básico de Tarifa**, aplicado desde a primeira passagem a quem é identificado eletronicamente.

Os percentuais mudam por contrato e ficam na tabela tarifária oficial da concessionária. Este repositório não guarda percentual nenhum, de propósito. A explicação do mecanismo está em [Tag de Pedágio](../TAG-DE-PEDAGIO.md#por-que-a-tag-dá-desconto-no-free-flow).

**A consequência prática:** quem passa pelo mesmo pórtico diariamente, no mesmo sentido, paga cada vez menos ao longo do mês, e só com tag. Quem paga pela placa fica de fora, sempre na tarifa cheia.

---

## A concessionária não vende tag

Ponto que gera dúvida e vale registrar: **a Rota Verde Goiás declara que não comercializa tags.** Ela opera a rodovia e processa o pagamento por placa; a tag é contratada com uma operadora autorizada.

É a separação que vale em todo o país: a concessionária registra a passagem, a operadora de tag processa o pagamento e cobra na sua fatura. Quem quiser tag contrata direto com uma das operadoras. A lista está em [Quais tags funcionam no Free Flow](../docs/tags-aceitas-no-free-flow.md), e a explicação em [Concessionárias com Free Flow no Brasil](../CONCESSIONARIAS-FREE-FLOW.md).

Por isso, desconfie de qualquer oferta de tag que se apresente como sendo da concessionária.

---

## Uma segunda concessão a caminho

Goiás vai ganhar um segundo operador de Free Flow.

| Rodovia | Concessionária | Situação |
|---|---|---|
| **BR-060** e **BR-364**, de Rio Verde a Rondonópolis | Rota Agro MT-GO, do grupo Way Brasil | **Previsto.** Concessão assumida em 02/04/2026, com 490 km em Goiás e Mato Grosso. Cinco pontos de cobrança contratados, em Jataí, Portelândia, Alto Garças e Pedra Preta. Sistema de livre passagem **homologado pela Senatran em 10/08/2026**, sem cobrança confirmada |

Atenção ao detalhe: **homologação não é início de cobrança.** O sistema da Rota Agro foi homologado, e isso não significa que os pontos já cobrem. Enquanto não houver confirmação oficial, **cobrança apresentada em nome desse trecho é motivo de desconfiança**. A explicação está em [Homologação do Free Flow pela Senatran](../docs/homologacao-senatran-free-flow.md) e o roteiro anti-golpe em [Golpe do falso pedágio](../docs/golpe-do-falso-pedagio.md).

Quando a cobrança começar, a BR-060 passará a ter dois operadores de Free Flow em trechos diferentes, o que torna ainda mais importante conferir **em que quilômetro** você passou.

---

## Perguntas frequentes

<details>
<summary><strong>Onde tem Free Flow em Goiás?</strong></summary>

Em duas rodovias federais operadas pela Rota Verde Goiás: a BR-060, com pontos de cobrança em Abadia de Goiás, Indiara, Jandaia e Acreúna, e a BR-452, em Santa Helena de Goiás e em dois pontos de Bom Jesus de Goiás. São 11 estruturas de pórtico e 7 pontos tarifários.
</details>

<details>
<summary><strong>Por que são 11 pórticos se são 7 pontos de cobrança?</strong></summary>

Porque na BR-060 os pórticos operam em pares, um por sentido, com quilometragens distintas registradas no cadastro da ANTT. Na BR-452 são pórticos únicos, com cobrança nos dois sentidos. Este repositório conta estruturas de cobrança, e por isso publica 11.
</details>

<details>
<summary><strong>Quando começou o pedágio eletrônico em Goiás?</strong></summary>

Em 27 de maio de 2026, nas BR-060 e BR-452, com a Rota Verde Goiás. Foi o primeiro pedágio eletrônico do estado.
</details>

<details>
<summary><strong>Como funciona o desconto para quem passa todo dia?</strong></summary>

Pelo Desconto de Usuário Frequente, que é progressivo e exige tag: começa na segunda passagem pelo mesmo pórtico, no mesmo sentido, dentro do mês, e cresce até a trigésima, quando o valor fica fixo até o fim do mês. Quem paga pela placa não recebe. Os percentuais estão na tabela tarifária oficial da concessionária.
</details>

<details>
<summary><strong>Compro a tag com a concessionária?</strong></summary>

Não. A Rota Verde declara que não comercializa tags. A tag é contratada com uma operadora autorizada, e a concessionária apenas registra a passagem. Oferta de tag que se apresente como sendo da concessionária é motivo de desconfiança.
</details>

<details>
<summary><strong>Qual o prazo para pagar sem tag?</strong></summary>

Trinta dias a partir da passagem, pelo site, pelo app ou nos totens das nove bases de atendimento ao usuário. Confirme sempre no canal oficial, porque o prazo vem do contrato de concessão.
</details>

---

## Fontes oficiais

| Fonte | O que traz |
|---|---|
| [ANTT, Free Flow](https://www.gov.br/antt/pt-br/free-flow) | Cadastro de pórticos, com a quilometragem de cada par na BR-060 |
| [Rota Verde Goiás, pedágio](https://rotaverdegoias.com.br/pedagio) | Funcionamento, canais e mecânica do Desconto de Usuário Frequente |
| [Rota Verde Goiás, pagamento](https://pedagioeletronico.rotaverdegoias.com.br) | Consulta e pagamento por placa |
| [ANTT, projeto Rota Agro CN2](https://www.gov.br/antt/pt-br/assuntos/rodovias/novos-projetos-em-rodovias/bndes-cn2-centro-oeste-norte) | A concessão prevista para as BR-060 e BR-364 |

Em caso de divergência, as fontes oficiais prevalecem sobre o que está aqui.

---

<div align="center">

### Quem roda todo dia é quem mais ganha com a tag

Em Goiás o desconto de usuário frequente cresce até a trigésima passagem do mês, e só vale para quem é identificado por tag.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=estado-go&utm_campaign=sem-parar-free-flow)**

Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

<br>

| Você quer | Vá para |
|---|---|
| Quitar uma passagem sem ser cliente | [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=estado-go&utm_campaign=sem-parar-free-flow) |
| Gestão de frota e soluções para empresas | [sempararempresas.com.br](https://www.sempararempresas.com.br?utm_source=github&utm_medium=estado-go&utm_campaign=sem-parar-free-flow) |

<br>

<sub>Página do repositório oficial mantido pelo <strong>Sem Parar</strong>, sob <a href="../LICENSE">CC BY 4.0</a>.</sub>

<sub><strong>Você com mais tempo para o que importa.</strong> #TudoProSeuCarro</sub>

</div>
