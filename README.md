<div align="center">

<img src=".github/assets/banner.svg" alt="Sem Parar, Free Flow e Tag de Pedágio" width="100%">

<h1>Free Flow e Tag de Pedágio, pelo Sem Parar</h1>

<p><strong>O guia oficial do Sem Parar sobre pedágio eletrônico no Brasil, com a base de dados aberta<br>das rodovias que já cobram por pórtico.</strong></p>

<p>
<img src="https://img.shields.io/badge/mantido%20pelo-Sem%20Parar-D60B52?style=flat-square" alt="Mantido pelo Sem Parar">
<img src="https://img.shields.io/badge/rodovias%20com%20free%20flow-26-D60B52?style=flat-square" alt="Rodovias com Free Flow mapeadas">
<img src="https://img.shields.io/badge/p%C3%B3rticos-74-525251?style=flat-square" alt="Pórticos monitorados">
<img src="https://img.shields.io/badge/concession%C3%A1rias-15-525251?style=flat-square" alt="Concessionárias com Free Flow ativo">
<br>
<img src="https://img.shields.io/github/last-commit/triwi/sem-parar-free-flow?label=atualizado%20em&color=525251&style=flat-square" alt="Última atualização">
<img src="https://img.shields.io/badge/licen%C3%A7a-CC%20BY%204.0-525251?style=flat-square" alt="Licença CC BY 4.0">
<img src="https://img.shields.io/badge/dados-abertos-2E7D32?style=flat-square" alt="Dados abertos">
<img src="https://img.shields.io/badge/PRs-bem--vindos-2E7D32?style=flat-square" alt="PRs bem-vindos">
</p>

</div>

---

## Um repositório do Sem Parar

Sem Parar criou a primeira Identificação Automática Veicular do Brasil, em 2000, e desde então acompanha de perto cada mudança na forma como o brasileiro paga pedágio. Hoje são milhões de clientes passando em 100% das rodovias pedagiadas do país, além de mais de 7 mil pontos urbanos.

O Free Flow é a maior dessas mudanças. E ele chegou espalhado: a ANTT publica os dados das rodovias federais, cada agência estadual publica os seus, e cada concessionária publica o próprio canal de pagamento. Quem passou por um pórtico e quer só quitar a tarifa precisa descobrir sozinho qual concessionária cobra, onde pagar e até quando.

**Sem Parar publica aqui essa informação reunida, datada e versionada, como dado aberto.** Qualquer pessoa pode consultar, corrigir e reutilizar, com ou sem tag, cliente ou não. É a mesma informação que orienta quem usa a Tag Sem Parar, aberta para todo mundo.

O repositório cobre dois temas conectados:

1. **Free Flow**, o pedágio eletrônico sem cancela: onde já existe, como funciona, como pagar e o que acontece quando o prazo passa.
2. **Tag de Pedágio**, a camada que transforma tudo isso em automático: como a cobrança funciona, o que muda com os descontos e onde a tag vale além do pedágio.

---

## O que é o Free Flow

**Free Flow é o pedágio eletrônico sem cancela: o motorista passa pelo pórtico sem parar e sem fila.** Câmeras e sensores identificam o veículo automaticamente, pela tag ou pela leitura da placa, e a tarifa é cobrada depois. Quem tem tag não faz nada, porque a cobrança cai direto na fatura. Quem não tem paga pela placa, nos canais oficiais da concessionária, dentro do prazo. No Brasil o mesmo sistema também é chamado de **pedágio eletrônico** ou **pedágio sem cancela**.

Em **25 de agosto de 2026**, o Brasil tem **74 pórticos de Free Flow em operação**, distribuídos por **26 rodovias**, **15 concessionárias** e **7 estados**: GO, MG, PR, RJ, RO, RS, SP.

---

## Índice

- [Um repositório do Sem Parar](#um-repositório-do-sem-parar)
- [O que é o Free Flow](#o-que-é-o-free-flow)
- [Rodovias com Free Flow no Brasil](#rodovias-com-free-flow-no-brasil), a tabela nacional
- [Onde o Free Flow ainda vai chegar](#onde-o-free-flow-ainda-vai-chegar)
- [Como pagar o Free Flow](#como-pagar-o-free-flow)
- [Tag de Pedágio, quando a cobrança vira automática](#tag-de-pedágio-quando-a-cobrança-vira-automática)
- [Perguntas frequentes](#perguntas-frequentes)
- [Dados abertos](#dados-abertos), em CSV e JSON
- [Como contribuir](#como-contribuir)
- [Fontes oficiais](#fontes-oficiais)
- [Metodologia e limites](#metodologia-e-limites)

---

## Rodovias com Free Flow no Brasil

Rodovias com cobrança eletrônica **em operação**, ordenadas por estado. Gerada a partir de [`dados/rodovias-free-flow.csv`](dados/rodovias-free-flow.csv), atualizada em **25 de agosto de 2026**.

| UF | Rodovia | Trecho e pórticos | Concessionária | Pórticos | Desde | Pagar |
|---|---|---|---|:---:|:---:|---|
| SP | **BR-116** Via Dutra - Trecho Metropolitano | km 206 (Arujá) ao km 231 (São Paulo), via expressa; marginal gratuita | Concessionária do Sistema Rodoviário Rio-São Paulo (RioSP) | 10 | 06/12/2025 | [pagar](https://rodovias.motiva.com.br/riosp/freeflow) |
| SP | **SP-021** Rodoanel Mário Covas - Trecho Norte | Guarulhos, km 135 (um pórtico por sentido) | Via SP Serra (Rodoanel Norte SPE) | 2 | 23/12/2025 | [pagar](https://viaappia.com.br/sigafacil/) |
| SP | **SP-055** Manoel Hipólito do Rego / Padre Manoel da Nóbrega | Santos (km 236) e Miracatu (km 389+560); Itariri opera só como monitoramento | Concessionária Novo Litoral (CNL) | 2 | 01/11/2025 | [pagar](https://cnl.pedagioeletronico.com.br) |
| SP | **SP-088** Pedro Eroles (Mogi-Dutra) | Arujá (km 037) e Mogi das Cruzes (km 041) | Concessionária Novo Litoral (CNL) | 2 | 01/11/2025 | [pagar](https://cnl.pedagioeletronico.com.br) |
| SP | **SP-098** Dom Paulo Rolim Loureiro (Mogi-Bertioga) | Bertioga (km 092+740) | Concessionária Novo Litoral (CNL) | 1 | 01/11/2025 | [pagar](https://cnl.pedagioeletronico.com.br) |
| SP | **SP-099** Rodovia dos Tamoios - Contorno Sul | Contorno Sul, km 13+500, Caraguatatuba (ligação Caraguatatuba-São Sebastião) | Concessionária Tamoios | 1 | 18/11/2024 | [pagar](https://freeflowtamoios.com.br) |
| SP | **SP-270** Raposo Tavares | São Roque (km 48), Alumínio/Sorocaba (km 83) e Araçoiaba da Serra (km 111) | Motiva Sorocabana (CCR Sorocabana) | 3 | 01/10/2025 | [pagar](https://rodovias.motiva.com.br/sorocabana/freeflow/) |
| SP | **SP-326** Brigadeiro Faria Lima | Dobrada (km 307) e Taiúva (km 357) | Ecovias Noroeste Paulista | 2 | 01/11/2025 | [pagar](https://freeflow.ecoviasnoroestepaulista.com.br) |
| SP | **SP-333** Laurentino Mascari / Carlos Tonanni | Itápolis (km 179) e Jaboticabal (km 110) | Ecovias Noroeste Paulista | 2 | 04/09/2024 | [pagar](https://freeflow.ecoviasnoroestepaulista.com.br) |
| PR | **BR-163** Lote Iguaçu | Santa Lúcia (km 154 e km 156,1), Oeste do Paraná | EPR Iguaçu | 2 | 23/02/2026 | [pagar](https://www.eprpedagioeletronico.com.br) |
| PR | **BR-369** Lote 4 - Norte e Noroeste do Paraná | Jataizinho (km 126) e Rolândia/Arapongas (km 180,2) | EPR Paraná | 4 | 04/05/2026 | [pagar](https://www.eprpedagioeletronico.com.br) |
| PR | **BR-376** Lote 4 - Norte e Noroeste do Paraná | Pres. Castelo Branco/Mandaguaçu (km 145,8) e Marialva/Mandaguari (km 196) | EPR Paraná | 4 | 04/05/2026 | [pagar](https://www.eprpedagioeletronico.com.br) |
| PR | **BR-376** Rodovia do Café | Mauá da Serra (km 294,8 no cadastro ANTT; km 292 pela concessionária) | PRVias (Motiva Paraná, ex-CCR RodoNorte) | 1 | 01/06/2026 | [pagar](https://pedagiodigital.com) |
| PR | **PR-182** Lote Iguaçu | Ampére (km 517,4), Sudoeste do Paraná | EPR Iguaçu | 1 | 23/02/2026 | [pagar](https://www.eprpedagioeletronico.com.br) |
| PR | **PR-280** Lote Iguaçu | Vitorino (km 234,3), Sudoeste do Paraná | EPR Iguaçu | 1 | 23/02/2026 | [pagar](https://www.eprpedagioeletronico.com.br) |
| PR | **PR-445** Rodovia Celso Garcia Cid | Tamarana (km 2,47; ANTT registra o município como Londrina) | PRVias (Motiva Paraná, ex-CCR RodoNorte) | 1 | 01/06/2026 | [pagar](https://pedagiodigital.com) |
| MG | **BR-262** Rota do Zebu | Betim a Uberaba (pórticos em Nova Serrana e Ibiá) | Concessionária da Rodovia BR-262/MG (Way-262) | 2 | 17/11/2025 | [pagar](https://pedagioeletronico.way262.com.br) |
| MG | **BR-381** Vale do Aço | Belo Horizonte (km 450+540) a Governador Valadares (km 150), 303,4 km | Concessionária de Rodovia Nova 381 | 5 | 27/09/2025 | [pagar](https://pedagioeletronico.nova381.com) |
| MG | **MG-459** Doutor Francisco Bueno Brandão | Monte Sião (km 12,7), Sul de Minas | EPR Sul de Minas | 1 | 04/06/2024 | [pagar](https://www.pedagiosemcancela.com.br) |
| GO | **BR-060** Concessão Centro-Norte (Rota Verde) | Anel Viário de Goiânia ao Contorno de Rio Verde, 229,6 km (Abadia de Goiás, Indiara, Jandaia... | Rota Verde Goiás | 8 | 27/05/2026 | [pagar](https://pedagioeletronico.rotaverdegoias.com.br) |
| GO | **BR-452** Concessão Centro-Norte (Rota Verde) | Rio Verde a Itumbiara, 196,6 km (Santa Helena de Goiás, Bom Jesus de Goiás) | Rota Verde Goiás | 3 | 27/05/2026 | [pagar](https://pedagioeletronico.rotaverdegoias.com.br) |
| RS | **ERS-122** Rota da Serra Gaúcha | São Sebastião do Caí (km 4), Farroupilha (km 45), Antônio Prado (km 108), Ipê (km 151) | Caminhos da Serra Gaúcha (CSG) | 4 | 15/12/2023 | [pagar](https://freeflow.csg.com.br) |
| RS | **ERS-240** Vale do Caí | Capela de Santana (km 30) | Caminhos da Serra Gaúcha (CSG) | 1 | 30/03/2024 | [pagar](https://freeflow.csg.com.br) |
| RS | **ERS-446** Carlos Barbosa | Carlos Barbosa (km 6) | Caminhos da Serra Gaúcha (CSG) | 1 | 30/03/2024 | [pagar](https://freeflow.csg.com.br) |
| RJ | **BR-101** Rio-Santos (Costa Verde) | Itaguaí a Paraty (trecho concedido BR-101 RJ/SP) | Concessionária do Sistema Rodoviário Rio-São Paulo (RioSP) | 3 | 31/03/2023 | [pagar](https://rodovias.motiva.com.br/riosp/freeflow) |
| RO | **BR-364** Rota Agro Norte | Porto Velho/Candeias do Jamari a Vilhena/Pimenta Bueno, 686,7 km | Concessionária de Rodovia Nova 364 | 7 | 12/01/2026 | [pagar](https://pedagioeletronico.nova364.com) |

**Total de 74 pórticos em operação.** Alguns pórticos instalados nessas mesmas rodovias operam apenas como monitoramento de tráfego, sem cobrança. Eles não entram nesta contagem e estão sinalizados na coluna de trecho.

### Onde o Free Flow ainda vai chegar

Trechos com Free Flow **previsto** ou com início **adiado**. Nenhum deles cobra tarifa por pórtico hoje, e essa é uma informação útil contra golpes: cobrança de Free Flow em rodovia desta lista merece desconfiança.

| UF | Rodovia | Concessionária | Situação | Detalhe |
|---|---|---|:---:|---|
| SP | **SP-079** Tenente Celestino Américo (Rota Sorocabana, 2ª etapa) | Motiva Sorocabana (CCR Sorocabana) | **adiado** | Piedade e Tapiraí (km 114, 138 e 193); pórticos instalados, hoje só monitoramento |
| SP | **SP-139** Rota Sorocabana - 2ª etapa | Motiva Sorocabana (CCR Sorocabana) | **adiado** | São Miguel Arcanjo (km 110); pórtico instalado, hoje só monitoramento |
| SP | **SP-150** Via Anchieta (Sistema Anchieta-Imigrantes) | Ecovias dos Imigrantes | **adiado** | km 33, descida e subida da serra; praça física do km 31 (Riacho Grande) segue em operação |
| SP | **SP-160** Rodovia dos Imigrantes (Sistema Anchieta-Imigrantes) | Ecovias dos Imigrantes | **adiado** | km 29 na descida; na subida o pórtico foi realocado para a região do km 38 (ponto exato em estudo) |
| SP | **SP-250** Bunjiro Nakao (Rota Sorocabana, 2ª etapa) | Motiva Sorocabana (CCR Sorocabana) | **adiado** | Ibiúna (km 56), Piedade (km 93), Pilar do Sul (km 122) e Capão Bonito (km 162 e 188) |
| SP | **SP-264** João Leme dos Santos (Rota Sorocabana, 2ª etapa) | Motiva Sorocabana (CCR Sorocabana) | **adiado** | Salto de Pirapora (km 114 e km 230); pórticos instalados, hoje só monitoramento |
| SP | **SP-280** Nova Raposo | Ecovias Raposo Castello | previsto | Castello Branco e Raposo Tavares, RMSP; primeiros pórticos a partir de 2026 |
| PR | **BR-153** EPR Litoral Pioneiro | EPR Litoral Pioneiro | previsto | ANTT lista termo aditivo previsto; a concessionária declarou não haver previsão (fontes divergentes) |
| PR | **BR-163** Lote 5 - Via Campo | Via Campo | **adiado** | Corbélia, Mamborê e Floresta; sistema em homologação, sem previsão de início da cobrança |
| MG | **BR-116** Rota das Gerais | Ecovias das Gerais | previsto | BR-116 e BR-251, norte de MG; contrato prevê Free Flow a partir de dezembro de 2026 |
| RS | **BR-116** Rota Portuária do Sul | a licitar | previsto | Camaquã à ponte sobre o Rio Jaguarão; 14 pórticos previstos no projeto (BR-116 e BR-392) |
| RS | **BR-290** FreeWay e malha ViaSul | CCR ViaSul | previsto | Conversão das 7 praças físicas em estudo, sem prazo definido |
| RJ | **BR-101** BR-101/RJ Norte | Arteris Fluminense | previsto | Pórticos previstos em Tanguá, Itaboraí e São Gonçalo; sem cronograma público |
| RJ | **BR-116** Trecho Metropolitano do Rio | Ecovias Rio Minas | previsto | km 161,70 ao km 205,87; Free Flow previsto no contrato, sem cronograma público |
| MT | **BR-163** Nova Rota do Oeste | Nova Rota do Oeste | previsto | Itiquira a Sinop; ANTT lista termo aditivo previsto para adoção do Free Flow |
| MS | **BR-262** Rota da Celulose | a definir | previsto | Corredor Três Lagoas-Água Clara-Campo Grande; 14 pórticos previstos para novembro de 2026 |
| MT | **MT-449** Rodovia da Mudança | Rodovia da Mudança | previsto | Lucas do Rio Verde e Tapurah; 6 pórticos em 3 corredores tarifários aprovados pela AGER-MT |

---

## Como pagar o Free Flow

Depende de uma pergunta só: **você tem tag?**

| Situação | O que fazer | Onde |
|---|---|---|
| **Tem tag ativa** | Nada. A tarifa é debitada automaticamente e ainda entra nos descontos do trecho, o DBT e o DUF | Cai na fatura da sua operadora |
| **Não tem tag** | Pagar pela placa, dentro do prazo do trecho | No canal oficial da concessionária, na coluna "Pagar" da tabela acima |
| **Não sabe se passou** | Consultar as passagens do seu veículo | App CNH do Brasil, em Veículos, depois Pedágio Eletrônico |
| **Quer parar de se preocupar** | Ativar uma tag e deixar a cobrança automática | [Peça a Tag Sem Parar](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=readme&utm_campaign=sem-parar-free-flow) |
| **Passou e não é cliente** | Quitar só aquela passagem, pela placa | [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=readme&utm_campaign=sem-parar-free-flow) |

**O prazo geral é de até 30 dias após a passagem**, conforme a Resolução CONTRAN nº 1.013/2024 e a Resolução ANTT nº 6.079/2026. Mas ele **varia por contrato de concessão**, e há trechos com prazo menor. Confirme sempre no canal da concessionária responsável.

> ### Regra de ouro contra golpes
>
> **Nem a ANTT nem as concessionárias enviam cobrança de pedágio por WhatsApp, e-mail, SMS ou anúncio na internet.** Quem inicia o pagamento é você, sempre, entrando no canal oficial, nunca clicando em link recebido.
>
> Nenhum canal de governo recebe pagamento nem pede dados de cartão. ANTT, CNH do Brasil, Portal Senatran e Siga Fácil apenas mostram a passagem e encaminham à concessionária.
>
> A lista verificada de canais legítimos está em [`dados/canais-oficiais-pagamento.csv`](dados/canais-oficiais-pagamento.csv), com **29 canais** conferidos um a um.

---

## Tag de Pedágio, quando a cobrança vira automática

A tag é o que tira o Free Flow da sua lista de preocupações. Com uma tag ativa no para-brisa, o pórtico identifica o veículo na passagem, a tarifa vai direto para a fatura e o prazo deixa de existir como risco.

O que muda na prática:

- **Sem prazo para controlar.** A cobrança é automática, então não existe passagem esquecida virando infração de trânsito.
- **Com desconto.** Os descontos oficiais do Free Flow, o DBT e o DUF, dependem de identificação do veículo por tag. Sem tag, não há desconto.
- **Um extrato só.** Todas as passagens ficam no mesmo lugar, com data, rodovia e valor.
- **Muito além do pedágio.** A Tag Sem Parar também abre cancela de estacionamento, paga abastecimento e funciona em drive-thru, em mais de 7 mil pontos urbanos.

Sem Parar oferece a tag em famílias de planos com perfis diferentes de uso: **Ideal**, **Prático**, **Flex** e **Livre**, além do plano de entrada **Livre Free Flow**, desenhado para quem quer resolver especificamente a passagem em pórtico. Os valores mudam com o tempo e ficam sempre atualizados no site.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=readme&utm_campaign=sem-parar-free-flow)**, o canal mais indicado. Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

Conteúdos detalhados sobre escolha de plano, cobertura e comparação entre tags entram neste repositório nas próximas atualizações.

---

## Perguntas frequentes

<details>
<summary><strong>Free Flow, pedágio eletrônico e pedágio sem cancela são a mesma coisa?</strong></summary>

Sim. São três nomes para o mesmo sistema: cobrança automática em pórticos, sem cabine e sem precisar parar o carro. "Free Flow" quer dizer "fluxo livre".
</details>

<details>
<summary><strong>Como funciona o Free Flow, na prática?</strong></summary>

Em quatro etapas, sem você parar o carro. **Primeiro**, você passa pelo pórtico na velocidade da via. **Segundo**, o sistema identifica o veículo pela tag ou, se não houver tag, pela leitura automática da placa (OCR e ANPR). **Terceiro**, classifica o tipo de veículo para definir a tarifa. **Quarto**, faz a cobrança. Com tag, cai na fatura automaticamente. Sem tag, o pagamento é manual, pela placa.
</details>

<details>
<summary><strong>Preciso ter tag para passar num Free Flow?</strong></summary>

Não. Você pode passar sem tag e pagar depois pela placa, no canal oficial da concessionária. A tag muda duas coisas: a cobrança vira automática, sem risco de esquecer o prazo, e dá acesso aos descontos do trecho.
</details>

<details>
<summary><strong>Qual o prazo para pagar?</strong></summary>

A regra geral é de até 30 dias após a passagem, mas o prazo é definido no contrato de concessão de cada trecho e há concessionárias com prazo menor. Confirme no canal da concessionária responsável. A coluna "Pagar" da tabela nacional leva direto a ele.
</details>

<details>
<summary><strong>O que acontece se eu não pagar?</strong></summary>

Passado o prazo, incidem encargos administrativos, multa moratória e juros. A passagem não paga configura infração de trânsito **grave**, prevista no art. 209-A do Código de Trânsito Brasileiro, com **5 pontos na CNH** e multa em valor definido pela regulação de trânsito.

Atenção à regra de transição vigente: a Deliberação CONTRAN nº 277/2026 suspendeu penalidades e abriu prazo até **16 de novembro de 2026** para regularizar tarifas em aberto sem as penalidades de trânsito. A anistia dispensa a multa, mas **não a tarifa**. A obrigação de pagar continua.
</details>

<details>
<summary><strong>Como sei se passei por um pórtico Free Flow?</strong></summary>

A forma oficial mais simples é o app CNH do Brasil, o mesmo da antiga Carteira Digital de Trânsito, na versão 7.3.0 ou superior. O caminho é Veículos, depois selecionar o veículo, depois Pedágio Eletrônico. Ele lista as passagens com data, local, concessionária, prazo e situação, que pode ser em processamento, pendente, pago ou vencido. A passagem pode levar até 24 horas para aparecer.

Empresas e frotistas consultam pelo Portal de Serviços da Senatran, não pelo app. E o app **não recebe pagamento**: ele encaminha ao canal da concessionária.

Quem usa a Tag Sem Parar acompanha tudo pelo extrato, sem precisar consultar nada.
</details>

<details>
<summary><strong>O Free Flow tem desconto?</strong></summary>

Sim. Nas concessões federais reguladas pela ANTT existem dois descontos oficiais: o **DBT**, Desconto Básico de Tarifa, e o **DUF**, Desconto de Usuário Frequente, que cresce conforme a frequência de uso do trecho. Ambos dependem de identificação do veículo por tag, então quem passa pela placa não recebe desconto. Os percentuais variam por contrato e são publicados na tabela tarifária de cada concessionária, com os links em [`dados/rodovias-free-flow.csv`](dados/rodovias-free-flow.csv).
</details>

<details>
<summary><strong>Recebi um SMS ou WhatsApp cobrando pedágio. É golpe?</strong></summary>

Quase certamente sim. Nem a ANTT nem as concessionárias enviam cobranças por mensagem, e as próprias concessionárias publicam esse alerta. Não clique no link. Confira você mesmo: consulte pelo app CNH do Brasil ou entre direto no canal oficial da concessionária do trecho, digitando o endereço no navegador.

Um sinal prático de autenticidade: canais oficiais costumam exibir eles próprios um aviso de "cuidado com golpes". Sites fraudulentos raramente incluem isso.
</details>

<details>
<summary><strong>Onde tem Free Flow no Brasil?</strong></summary>

Hoje em GO, MG, PR, RJ, RO, RS, SP. A lista completa e datada está na [tabela nacional](#rodovias-com-free-flow-no-brasil) acima, e o dado bruto em [`dados/rodovias-free-flow.csv`](dados/rodovias-free-flow.csv). A lista muda rápido, porque pórticos são inaugurados e adiados com frequência, e este repositório é atualizado a cada mudança confirmada.
</details>

<details>
<summary><strong>A mesma tag funciona em qualquer Free Flow?</strong></summary>

As operadoras de tag autorizadas pela ANTT são interoperáveis nas rodovias federais concedidas. Em concessões estaduais, a lista de operadoras aceitas é definida pela agência reguladora do estado e pode variar. As operadoras autorizadas estão marcadas com o tipo `tag` em [`dados/canais-oficiais-pagamento.csv`](dados/canais-oficiais-pagamento.csv). A Tag Sem Parar funciona em 100% das rodovias pedagiadas do país.
</details>

---

## Dados abertos

Todo o conteúdo deste repositório nasce de três bases públicas em **CSV**, sob licença **CC BY 4.0**. O reuso é livre, inclusive comercial, desde que citada a fonte.

| Base | O que traz | Linhas |
|---|---|:---:|
| [`rodovias-free-flow`](dados/rodovias-free-flow.csv) | Inventário nacional de rodovias com Free Flow ativo, previsto ou adiado | 43 |
| [`concessionarias-free-flow`](dados/concessionarias-free-flow.csv) | Quem opera cada trecho, com plataforma de pagamento e canais | 22 |
| [`canais-oficiais-pagamento`](dados/canais-oficiais-pagamento.csv) | Lista verificada de canais legítimos de consulta e pagamento | 29 |

O dicionário de dados, com o significado de cada coluna e os valores aceitos, está em **[`dados/README.md`](dados/README.md)**.

**Como citar:**

> Sem Parar. *Free Flow e Tag de Pedágio: base aberta de rodovias com pedágio eletrônico no Brasil.* Consultado em [data]. Disponível em: https://github.com/triwi/sem-parar-free-flow

---

## Como contribuir

Pórtico novo? Data mudou? Link quebrado? [**Abra uma issue**](../../issues/new) contando o que viu.

Toda contribuição precisa vir com **fonte oficial**, seja a ANTT, uma agência estadual ou a concessionária. O que entra e o que não entra está em [CONTRIBUTING.md](CONTRIBUTING.md), e o histórico de mudanças em [CHANGELOG.md](CHANGELOG.md).

---

## Fontes oficiais

Estas são as fontes primárias deste repositório. Em caso de divergência, **elas prevalecem sobre o que está aqui**.

| Fonte | O que traz |
|---|---|
| [ANTT, Free Flow](https://www.gov.br/antt/pt-br/free-flow) | Painel oficial das rodovias **federais** concedidas, com localizador de pórticos |
| [Resolução ANTT nº 6.079/2026](https://anttlegis.antt.gov.br/) | Regulamenta o sistema de livre passagem nas rodovias federais, publicada em 27/03/2026 |
| [CNH do Brasil](https://www.gov.br/transportes/pt-br/cnh-do-brasil) | Consulta oficial de passagens de Free Flow por veículo |
| [Portal de Serviços Senatran](https://portalservicos.senatran.serpro.gov.br) | Consulta detalhada e obrigatória para frotas |
| [Siga Fácil, Governo de SP e ARTESP](https://www.sigafacil.sp.gov.br) | Free Flow nas rodovias **estaduais paulistas** |
| [RS Parcerias, Free Flow](https://parcerias.rs.gov.br/free-flow) | Free Flow nas rodovias **estaduais gaúchas** |
| Sites das concessionárias | Pórticos, prazos, tarifas e canais de pagamento de cada trecho |

---

## Metodologia e limites

**Como os dados são levantados.** Sem Parar parte do painel oficial da ANTT para as rodovias federais e dos portais das agências estaduais, entre elas ARTESP, AGERGS e DER-MG, para as estaduais, e confere cada trecho no site da concessionária responsável. Cada linha das bases carrega a coluna `fonte` e a coluna `atualizado_em`.

**Divergências.** Quando a ANTT e a concessionária publicam quilometragens diferentes para o mesmo pórtico, e isso acontece, registramos o valor da ANTT e sinalizamos a divergência no campo de trecho. Nenhum dado foi inferido ou preenchido por dedução: o que não foi confirmado aparece como `n/d`.

**O que este repositório não faz.** Não guardamos valores de tarifa, mensalidade ou percentual de desconto, porque esses números mudam com frequência e envelhecem mal. Guardamos o link da tabela tarifária oficial de cada concessionária, que está sempre atualizada na origem.

**Frequência de atualização.** Inaugurações, adiamentos e mudanças de status entram em até 72 horas após o fato. As bases passam por revisão completa mensal, com tudo registrado no [CHANGELOG](CHANGELOG.md).

**Isenção.** Este material é informativo e não substitui os canais oficiais para consulta de débitos, contestação de cobrança ou defesa de infração.

---

<div align="center">

### Resolva de uma vez com a Tag Sem Parar

Com uma tag ativa, a tarifa do Free Flow é debitada automaticamente, entra nos descontos do trecho e some da sua lista de preocupações.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=readme&utm_campaign=sem-parar-free-flow)**

Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

<br>

| Você quer | Vá para |
|---|---|
| Quitar uma passagem sem ser cliente | [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=readme&utm_campaign=sem-parar-free-flow) |
| Gestão de frota e soluções para empresas | [sempararempresas.com.br](https://www.sempararempresas.com.br?utm_source=github&utm_medium=readme&utm_campaign=sem-parar-free-flow) |

<br>

<sub>Repositório oficial mantido pelo <strong>Sem Parar</strong>. Conteúdo e dados sob <a href="LICENSE">CC BY 4.0</a>. Última revisão dos dados em 25 de agosto de 2026.</sub>

<sub><strong>Você com mais tempo para o que importa.</strong> #TudoProSeuCarro</sub>

</div>
