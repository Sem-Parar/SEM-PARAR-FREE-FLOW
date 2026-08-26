# Free Flow na BR-376: a única rodovia do país com duas concessionárias cobrando

**A BR-376, no Paraná, tem 5 pórticos de Free Flow operados por duas concessionárias diferentes: a EPR Paraná, com quatro pórticos em Mandaguaçu (km 145,8) e Marialva (km 196), e a PRVias, com um pórtico em Mauá da Serra (km 294,8), no trecho conhecido como Rodovia do Café. É a única rodovia brasileira em que dois operadores cobram Free Flow, e cada um tem canal de pagamento próprio. Pagar no portal errado não quita a sua passagem.**

Quem roda de Maringá a Londrina pela BR-376 pode atravessar pórticos das duas concessionárias na mesma viagem.

> Publicado em 26 de agosto de 2026. Última atualização em 26 de agosto de 2026.
> Parte do repositório [Free Flow e Tag de Pedágio, pelo Sem Parar](../README.md). Base de dados em [`dados/porticos-free-flow.csv`](../dados/porticos-free-flow.csv).

---

## Índice

- [Os 5 pórticos, e quem cobra cada um](#os-5-pórticos-e-quem-cobra-cada-um)
- [Duas concessionárias, dois canais](#duas-concessionárias-dois-canais)
- [Quatro pórticos, dois pontos de cobrança](#quatro-pórticos-dois-pontos-de-cobrança)
- [A janela de duas horas da PRVias](#a-janela-de-duas-horas-da-prvias)
- [A divergência de quilometragem em Mauá da Serra](#a-divergência-de-quilometragem-em-mauá-da-serra)
- [Com tag, a diferença some](#com-tag-a-diferença-some)
- [Perguntas frequentes](#perguntas-frequentes)
- [Fontes oficiais](#fontes-oficiais)

---

## Os 5 pórticos, e quem cobra cada um

| Município | km | Estruturas | Concessionária | Desde |
|---|---|:---:|---|:---:|
| **Presidente Castelo Branco / Mandaguaçu** | 145,8 | 2, uma por sentido | EPR Paraná | 04/05/2026 |
| **Marialva / Mandaguari** | 196 | 2, uma por sentido | EPR Paraná | 04/05/2026 |
| **Mauá da Serra** | 294,8 | 1 | PRVias | 01/06/2026 |

**Cinco estruturas de cobrança.** Os valores de tarifa mudam com o reajuste anual da ANTT e não são publicados aqui: consulte a tabela oficial de cada concessionária.

Dois pórticos aparecem com o nome de duas cidades porque ficam na divisa entre elas. É uma estrutura só, registrada sob os dois municípios.

**A BR-376 é rodovia federal concedida**, regulada pela **ANTT**, nos dois trechos. Isso significa que valem ali a interoperabilidade obrigatória de tag e os direitos da Resolução ANTT nº 6.079/2026, independentemente de qual das duas concessionárias cobrou.

---

## Duas concessionárias, dois canais

| | **EPR Paraná** | **PRVias** |
|---|---|---|
| Trecho | Lote 4, norte e noroeste do Paraná | Rodovia do Café |
| Grupo | Grupo EPR, Equipav e Perfin | Motiva, ex-CCR |
| Pórticos na BR-376 | 4, em dois pontos | 1 |
| Plataforma de pagamento | Própria | **Pedágio Digital** |
| Onde pagar | [eprpedagioeletronico.com.br](https://www.eprpedagioeletronico.com.br) | [pedagiodigital.com](https://pedagiodigital.com) |
| Página completa | [Free Flow do Grupo EPR](../concessionarias/free-flow-epr.md) | [Free Flow da Motiva](../concessionarias/free-flow-motiva-ccr.md) |

**Se você não sabe qual dos dois cobrou**, consulte pelo app **CNH do Brasil**, com o app atualizado, em Veículos, depois o veículo, depois Pedágio eletrônico. Ele identifica a concessionária responsável por cada passagem e encaminha ao canal certo, sem receber pagamento. Ver [Como consultar o Free Flow no app CNH do Brasil](../docs/consulta-app-cnh-do-brasil.md).

> **Nenhuma das duas concessionárias envia cobrança por WhatsApp, SMS ou e-mail**, e não existe boleto automático de Free Flow. Quem inicia o pagamento é você, digitando o endereço no navegador. Ver [Golpe do falso pedágio](../docs/golpe-do-falso-pedagio.md).

---

## Quatro pórticos, dois pontos de cobrança

No trecho da EPR Paraná, os pórticos operam **em pares**: uma estrutura para cada sentido da pista, no mesmo ponto. São quatro estruturas em dois pontos tarifários.

**Você paga uma vez por ponto que atravessar**, não duas. O par existe por engenharia da via, não por cobrança dobrada. Ida e volta pelo mesmo ponto, sim, são duas passagens.

Este repositório conta **estruturas que cobram**, e por isso publica 4 no trecho da EPR. Quem conta pontos tarifários publica 2. O critério está declarado em [Metodologia e fontes](../docs/metodologia-e-fontes.md).

---

## A janela de duas horas da PRVias

Regra própria do trecho da Rodovia do Café que não vale no da EPR: **a PRVias adota uma janela de duas horas para cobrança única**.

Na prática, quem passa pelo pórtico e retorna dentro desse intervalo não gera uma segunda cobrança pelo mesmo ponto. É a mesma lógica que a Motiva aplica na Via Dutra, e faz sentido em trechos com deslocamento local frequente.

**No trecho da EPR Paraná não há janela equivalente publicada.** Cada travessia de ponto tarifário é uma passagem.

---

## A divergência de quilometragem em Mauá da Serra

Registrada, porque credibilidade de dado depende disso.

| Fonte | O que publica |
|---|---|
| **Cadastro de pórticos da ANTT** | km **294,8** |
| **Comunicação da concessionária** | km **292** |

**Adotamos o valor da ANTT**, por hierarquia de fonte, e anotamos a divergência na observação da linha. Para o motorista isso não muda nada: o pórtico é o mesmo, o pagamento é o mesmo, e a diferença é de registro.

A mesma concessionária tem outra divergência registrada, na PR-445: a ANTT registra o município como Londrina e a concessionária comunica Tamarana. Nos dois casos a regra é a mesma, e está em [Metodologia e fontes](../docs/metodologia-e-fontes.md).

---

## Com tag, a diferença some

Numa rodovia com dois operadores, a tag resolve o problema mais chato: **você não precisa saber quem cobrou**. As passagens das duas concessionárias caem na mesma fatura, cada uma com o desconto do seu trecho.

Como a BR-376 é federal, valem ali os dois descontos oficiais, o **DBT, Desconto Básico de Tarifa**, e o **DUF, Desconto de Usuário Frequente**, ambos dependentes de identificação eletrônica. Quem paga pela placa não recebe nenhum dos dois.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=br-376&utm_campaign=sem-parar-free-flow)**, o canal mais indicado. Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

---

## Perguntas frequentes

<details>
<summary><strong>Quantos pedágios eletrônicos tem a BR-376?</strong></summary>

Cinco estruturas de cobrança, em três pontos: Mandaguaçu (km 145,8) e Marialva (km 196), da EPR Paraná, com um pórtico por sentido em cada; e Mauá da Serra (km 294,8), da PRVias. As praças físicas do trecho seguem sua própria regra.
</details>

<details>
<summary><strong>Por que duas concessionárias na mesma rodovia?</strong></summary>

Porque a BR-376 foi dividida em lotes de concessão diferentes. O trecho do norte e noroeste ficou com a EPR Paraná, e o da Rodovia do Café, com a PRVias. É a única rodovia do país em que dois operadores cobram Free Flow.
</details>

<details>
<summary><strong>Como sei qual das duas cobrou a minha passagem?</strong></summary>

Pelo quilômetro em que você passou, ou pelo app CNH do Brasil, que mostra a concessionária responsável por cada passagem registrada e encaminha ao canal de pagamento correto.
</details>

<details>
<summary><strong>Passei duas vezes pelo mesmo pórtico no mesmo dia. Pago duas vezes?</strong></summary>

Depende do trecho. No da PRVias, em Mauá da Serra, há janela de duas horas para cobrança única. No da EPR Paraná não há janela equivalente publicada, e cada travessia de ponto tarifário é uma passagem.
</details>

<details>
<summary><strong>A mesma tag funciona nos dois trechos?</strong></summary>

Sim. A BR-376 é rodovia federal concedida, e ali a interoperabilidade entre as operadoras autorizadas é obrigatória. Ver [Quais tags funcionam no Free Flow](../docs/tags-aceitas-no-free-flow.md).
</details>

<details>
<summary><strong>Moto paga na BR-376?</strong></summary>

A regra de isenção de motocicleta no Paraná não está confirmada em fonte oficial que possamos citar, e por isso o estado aparece como "consulte" na nossa tabela nacional. Confirme no canal da concessionária do trecho antes de contar com isenção. Ver [Tag em moto, carro alugado e segundo veículo](../docs/tag-em-moto-e-outros-veiculos.md).
</details>

---

## Fontes oficiais

| Fonte | O que traz |
|---|---|
| [ANTT, Free Flow](https://www.gov.br/antt/pt-br/free-flow) | Cadastro de pórticos das concessões federais, com quilômetro por estrutura |
| [EPR, pedágio eletrônico](https://www.eprpedagioeletronico.com.br) | Consulta e pagamento das passagens do trecho da EPR Paraná |
| [Pedágio Digital](https://pedagiodigital.com) | Consulta e pagamento das passagens do trecho da PRVias |

Em caso de divergência, as fontes oficiais prevalecem sobre o que está aqui. Como cada dado foi levantado está em [Metodologia e fontes](../docs/metodologia-e-fontes.md).

Viu algo desatualizado? [Abra uma issue](../../../issues/new) com a fonte.

---

### Duas concessionárias, uma fatura

Quem roda o eixo Maringá, Londrina e Apucarana atravessa pórticos de operadores diferentes na mesma viagem. Com uma tag ativa, tudo cai no mesmo extrato, com os descontos de cada trecho, e você não precisa descobrir quem cobrou.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=br-376&utm_campaign=sem-parar-free-flow)**

Passou e não é cliente? Dá para quitar só aquela passagem, pela placa, em [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=br-376&utm_campaign=sem-parar-free-flow).

<sub>Página publicada pelo <strong>Sem Parar</strong> sob <a href="../LICENSE">CC BY 4.0</a>. Use, adapte e redistribua à vontade, bastando citar a fonte.</sub>
