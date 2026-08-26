# Tag de Pedágio: o que é, como funciona e o que muda no Free Flow

**Tag de pedágio é um adesivo eletrônico colado no para-brisa que identifica o veículo por radiofrequência e faz o pagamento da tarifa acontecer sozinho. Nas praças com cancela, ela abre a cancela sem parada. Nos pórticos de Free Flow, onde não existe cancela, ela faz a cobrança cair direto na fatura e elimina a etapa de consultar a placa e pagar depois. A tag não é obrigatória em lugar nenhum do Brasil: ela troca uma tarefa com prazo por uma cobrança automática.**

Essa é a diferença que quase ninguém explica direito. Sem tag, o pedágio eletrônico continua funcionando, só que a responsabilidade de pagar volta para você, com um relógio correndo. Com tag, o relógio deixa de existir.

> Publicado em 26 de agosto de 2026. Última atualização em 26 de agosto de 2026.
> Página pilar do repositório [Free Flow e Tag de Pedágio, pelo Sem Parar](README.md). Termos técnicos estão no [glossário](docs/glossario.md).

---

## Índice

- [O que é uma tag de pedágio](#o-que-é-uma-tag-de-pedágio)
- [Como a tag funciona no Free Flow, passo a passo](#como-a-tag-funciona-no-free-flow-passo-a-passo)
- [Com tag e sem tag: o que muda de verdade](#com-tag-e-sem-tag-o-que-muda-de-verdade)
- [Uma tag vale no Brasil inteiro?](#uma-tag-vale-no-brasil-inteiro)
- [Por que a tag dá desconto no Free Flow](#por-que-a-tag-dá-desconto-no-free-flow)
- [O que a tag não resolve](#o-que-a-tag-não-resolve)
- [Onde a tag vale além do pedágio](#onde-a-tag-vale-além-do-pedágio)
- [Como escolher e como contratar](#como-escolher-e-como-contratar)
- [Perguntas frequentes](#perguntas-frequentes)
- [Fontes oficiais](#fontes-oficiais)

---

## O que é uma tag de pedágio

A tag é um dispositivo passivo de radiofrequência, do tamanho de um cartão, colado por dentro do para-brisa. Ela não tem bateria e não emite sinal sozinha: quando o veículo passa sob uma antena, a antena energiza a tag, lê um código único e devolve esse código ao sistema de arrecadação, que o associa a um cadastro com placa, categoria de veículo e meio de pagamento.

No Brasil essa categoria nasceu em 2000, com a primeira Identificação Automática Veicular do país, criada pelo Sem Parar. O nome popular "tag de pedágio" veio depois, e hoje convive com "adesivo eletrônico", "tag veicular" e "pagamento automático de pedágio".

Do ponto de vista regulatório, quem opera tag não é a concessionária. São empresas autorizadas e fiscalizadas separadamente, chamadas nas rodovias federais de **AMAP**, sigla de Administradora de Meios de Pagamento para Arrecadação de Pedágio, definida pela [Resolução ANTT nº 4.281/2014](https://www.gov.br/antt/pt-br/free-flow). Nas rodovias estaduais, a autorização vem da agência reguladora do estado, como a ARTESP em São Paulo e a AGERGS no Rio Grande do Sul.

Essa separação explica uma coisa que confunde muita gente: **a rodovia não escolhe a sua tag, e a sua operadora de tag não cobra o pedágio.** A concessionária registra a passagem, a operadora processa o pagamento e cobra de você na fatura ou no saldo.

---

## Como a tag funciona no Free Flow, passo a passo

No Free Flow não existe cancela, então a tag deixa de servir para abrir alguma coisa e passa a servir apenas para identificar o veículo antes que a câmera precise ler a placa.

1. **Passagem.** O veículo passa sob o pórtico na velocidade da via, sem reduzir.
2. **Identificação.** A antena do pórtico lê a tag. Se a leitura falhar ou não houver tag, o sistema recorre à leitura automática da placa, por OCR e ANPR.
3. **Classificação.** Sensores contam eixos e definem a categoria do veículo, que determina a tarifa.
4. **Cobrança.** Identificado por tag, o valor segue para a operadora e entra na sua fatura ou é debitado do saldo, já com o desconto do trecho aplicado. Identificado por placa, o valor fica em aberto para pagamento posterior no canal da concessionária.

O passo 2 é o único que muda entre ter e não ter tag. Todo o resto é igual. A mecânica completa do pórtico está em [O que é Free Flow e como funciona o pedágio sem cancela](O-QUE-E-FREE-FLOW.md).

> **Detalhe que gera dúvida:** quando a passagem é cobrada por tag, ela normalmente **não aparece** no portal de pagamento avulso da concessionária, porque aquele portal existe para quem paga pela placa. Não é erro nem cobrança perdida. O registro está no extrato da sua operadora.

---

## Com tag e sem tag: o que muda de verdade

| Item | Com tag ativa | Sem tag |
|---|---|---|
| Passar pelo pórtico | Permitido | Permitido, não é infração |
| Ação depois da viagem | Nenhuma | Consultar e pagar pela placa |
| Prazo para pagar | Definido pela sua operadora, na fatura ou no saldo | Prazo do trecho, em regra 30 dias |
| Risco de virar infração | Não existe enquanto a tag estiver ativa e com saldo | Existe se o prazo passar |
| Descontos do trecho, DBT e DUF | Sim | Não |
| Onde acompanhar | Extrato único da operadora | Site ou app de cada concessionária |
| Custo do serviço de tag | Depende do plano contratado | Nenhum |

A leitura honesta dessa tabela: quem passa por pórtico uma ou duas vezes por ano resolve bem pela placa. Quem passa toda semana está fazendo, toda semana, uma tarefa que a tag faria sozinha, e ainda pagando tarifa cheia.

O caminho de quem passou sem tag está em [Passei num Free Flow sem tag](docs/passei-sem-tag.md), e a régua de prazos em [Prazo para pagar o Free Flow](docs/prazo-e-encargos.md).

---

## Uma tag vale no Brasil inteiro?

Nas **rodovias federais concedidas**, sim, e isso é obrigação legal, não cortesia comercial. A [Lei nº 14.157/2021](https://www.gov.br/antt/pt-br/free-flow) determinou a interoperabilidade do pagamento eletrônico de pedágio, e a Resolução ANTT nº 4.281/2014 estabelece o padrão técnico que faz qualquer tag autorizada ser lida por qualquer pórtico da malha federal.

Nas **rodovias estaduais**, a lista de operadoras aceitas é definida pela agência reguladora do estado. Em São Paulo, as concessionárias publicam a lista da ARTESP com cinco operadoras: ConectCar, Move Mais, Sem Parar, Taggy e Veloe.

A tabela de aceitação, concessionária por concessionária, está em [Quais tags funcionam no Free Flow](docs/tags-aceitas-no-free-flow.md), e o dado bruto em [`dados/tags-aceitas-free-flow.csv`](dados/tags-aceitas-free-flow.csv).

**A Tag Sem Parar é aceita em 100% das rodovias pedagiadas do Brasil**, nas praças com cancela e nos pórticos de Free Flow.

---

## Por que a tag dá desconto no Free Flow

Os descontos oficiais do Free Flow nas concessões federais têm nome e regra própria:

- **DBT, Desconto Básico de Tarifa.** Aplicado a partir da primeira passagem, para quem é identificado eletronicamente.
- **DUF, Desconto de Usuário Frequente.** Progressivo, cresce conforme o número de passagens pelo mesmo pórtico, no mesmo sentido, dentro do mesmo mês.

Os dois dependem de identificação do veículo, e é aí que está a chave: **quem passa pela placa não recebe desconto**. Não é uma penalidade, é uma consequência técnica, porque o desconto por frequência precisa reconhecer o mesmo veículo passagem após passagem.

Os percentuais variam por contrato de concessão e mudam com o tempo. Este repositório não guarda percentual nenhum, de propósito: o número correto está sempre na tabela tarifária oficial de cada concessionária, linkada em [`dados/rodovias-free-flow.csv`](dados/rodovias-free-flow.csv).

Algumas concessionárias estaduais oferecem caminho alternativo para quem não pode usar tag. A CSG, no Rio Grande do Sul, concede o desconto a quem faz cadastro no site ou no aplicativo, sem tag. É a exceção que confirma a regra: o que o sistema precisa é reconhecer você.

---

## O que a tag não resolve

Vale dizer o que ela não faz, porque é isso que evita frustração:

- **Não isenta ninguém de tarifa.** A tag paga, ela não perdoa.
- **Não funciona em motocicleta.** Nenhuma tag no Brasil é homologada para moto. O motivo, e o que fazer, estão em [Tag em moto, carro alugado e segundo veículo](docs/tag-em-moto-e-outros-veiculos.md).
- **Não serve para dois carros.** Cada tag é vinculada a uma placa.
- **Não paga passagem antiga.** Débito anterior à ativação da tag continua sendo seu, pela placa. Veja [Não paguei o Free Flow](docs/nao-paguei-e-agora.md).
- **Não protege contra tag inativa ou sem saldo.** Se a tag não for lida por estar irregular, o pórtico lê a placa e a tarifa volta a ser sua responsabilidade.

---

## Onde a tag vale além do pedágio

A tag nasceu para pedágio, mas a antena que lê o para-brisa é a mesma em outros lugares. Com a Tag Sem Parar, o mesmo adesivo abre cancela de estacionamento, paga abastecimento e funciona em drive-thru e lava-rápido, em mais de 7 mil pontos urbanos.

Na prática, é o que transforma a tag de item de viagem em item de rotina: quem só pega estrada nas férias usa a tag duas semanas por ano, quem estaciona em shopping usa toda semana.

---

## Como escolher e como contratar

A escolha entre operadoras é uma decisão de perfil de uso, não de tabela de preço. Os critérios que importam:

| Critério | O que perguntar |
|---|---|
| Cobertura em pedágio | A tag é aceita em 100% das rodovias pedagiadas, federais e estaduais? |
| Free Flow | Ela é reconhecida nos pórticos das concessionárias por onde você passa? |
| Uso urbano | Vale em estacionamento, posto, drive-thru e lava-rápido, ou só em rodovia? |
| Extrato e app | Dá para ver passagem por passagem, com rodovia, data e valor? |
| Modelo de cobrança | O plano combina com a sua frequência de uso? |
| Atendimento | Existe canal para contestar cobrança e resolver tag não lida? |

Sem Parar oferece a tag em famílias de planos com perfis diferentes de uso: **Ideal**, **Prático**, **Flex** e **Livre**, além do plano de entrada **Livre Free Flow**, desenhado para quem quer resolver especificamente a passagem em pórtico. Os valores mudam com o tempo e ficam sempre atualizados no site.

**A contratação é feita em [semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=tag-de-pedagio&utm_campaign=sem-parar-free-flow)**, o canal mais indicado. Se preferir, também pode ser feita pelo SuperApp Sem Parar.

---

## Perguntas frequentes

<details>
<summary><strong>Preciso de tag para passar num pórtico de Free Flow?</strong></summary>

Não. Passar sem tag não é infração e não é irregularidade. O pórtico lê a placa e a tarifa fica em aberto para pagamento no canal oficial da concessionária, em regra dentro de 30 dias. A tag muda duas coisas: a cobrança vira automática, sem prazo para controlar, e dá acesso aos descontos do trecho.
</details>

<details>
<summary><strong>A mesma tag funciona em qualquer rodovia com Free Flow?</strong></summary>

Nas rodovias federais concedidas, sim, por força da interoperabilidade prevista na Lei nº 14.157/2021 e regulada pela ANTT. Nas estaduais, vale a lista de operadoras autorizadas pela agência do estado, que pode ser menor. A tabela por concessionária está em [Quais tags funcionam no Free Flow](docs/tags-aceitas-no-free-flow.md). A Tag Sem Parar é aceita em 100% das rodovias pedagiadas do país.
</details>

<details>
<summary><strong>Posso usar a mesma tag em dois carros?</strong></summary>

Não. Cada tag é vinculada a uma única placa, porque a leitura no pórtico cruza o código da tag com o cadastro do veículo, inclusive a categoria que define a tarifa. Usar a tag em outro carro gera cobrança na categoria errada e leitura inconsistente. Para o segundo carro, o caminho é uma nova adesão. Para carro novo, existe troca de veículo no cadastro.
</details>

<details>
<summary><strong>Tem tag para moto?</strong></summary>

Não no Brasil. Nenhuma operadora tem tag homologada para motocicleta, e o motivo declarado pelas agências reguladoras é segurança nas pistas automáticas com cancela. No Free Flow, onde não há cancela, a moto passa normalmente e paga pela placa, quando o trecho cobra de moto. O detalhe está em [Tag em moto, carro alugado e segundo veículo](docs/tag-em-moto-e-outros-veiculos.md).
</details>

<details>
<summary><strong>Passei com tag e a cobrança não apareceu no site da concessionária. Isso é normal?</strong></summary>

Sim, e é o comportamento esperado. O portal de pagamento da concessionária mostra passagens em aberto, ou seja, aquelas que serão pagas pela placa. Passagem já capturada pela tag sai daquela fila e vai para o extrato da sua operadora. Se a passagem não aparecer em nenhum dos dois lugares depois de alguns dias, aí vale abrir contestação. O caminho está em [Como funciona a cobrança da tag](docs/como-funciona-a-cobranca-da-tag.md).
</details>

<details>
<summary><strong>A tag paga a multa se eu esquecer?</strong></summary>

A questão não chega a se colocar: com tag ativa e regular, não existe passagem esquecida, porque a cobrança não depende de você. O risco de infração existe quando a passagem é lida pela placa e o prazo passa. Se você já tem passagem atrasada de antes da tag, ela continua sendo sua e o caminho está em [Não paguei o Free Flow](docs/nao-paguei-e-agora.md).
</details>

<details>
<summary><strong>Quem opera a tag é a concessionária da rodovia?</strong></summary>

Não. São empresas distintas, autorizadas e fiscalizadas pela ANTT nas federais, sob a sigla AMAP, e pelas agências estaduais nas rodovias de cada estado. A concessionária registra a passagem no pórtico; a operadora de tag processa o pagamento e cobra de você. É por isso que a fatura vem da operadora e não da rodovia.
</details>

<details>
<summary><strong>Tag e vale-pedágio são a mesma coisa?</strong></summary>

Não. O Vale-Pedágio Obrigatório é um instrumento do transporte de carga, previsto na Lei nº 10.209/2001, em que o embarcador antecipa o pedágio da viagem ao transportador. Desde 2025 ele só existe em formato eletrônico, e é comum que circule vinculado a uma tag, mas continua sendo outro produto, com outra finalidade, voltado a frota. O caminho para empresas é [sempararempresas.com.br](https://www.sempararempresas.com.br?utm_source=github&utm_medium=tag-de-pedagio&utm_campaign=sem-parar-free-flow).
</details>

---

## Fontes oficiais

| Fonte | O que traz |
|---|---|
| [ANTT, Free Flow](https://www.gov.br/antt/pt-br/free-flow) | Regulação do pedágio eletrônico nas federais, interoperabilidade e autorização das AMAPs |
| [Resolução ANTT nº 4.281/2014](https://anttlegis.antt.gov.br/) | Padroniza o sistema de arrecadação eletrônica e define a figura da AMAP |
| [Resolução ANTT nº 6.079/2026](https://anttlegis.antt.gov.br/) | Sistema de livre passagem, formas de pagamento e prazos, publicada em 27/03/2026 |
| [Siga Fácil, Governo de SP e ARTESP](https://www.sigafacil.sp.gov.br) | Free Flow nas rodovias estaduais paulistas e operadoras aceitas |
| Sites das concessionárias | Lista de operadoras aceitas, descontos e canais de cada trecho |

Em caso de divergência, as fontes oficiais prevalecem sobre o que está aqui.

---

<div align="center">

### A tag existe para você não pensar nisso

Com uma tag ativa, a tarifa do Free Flow é debitada automaticamente, entra nos descontos do trecho e nenhum prazo depende da sua memória.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=tag-de-pedagio&utm_campaign=sem-parar-free-flow)**

Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

<br>

| Você quer | Vá para |
|---|---|
| Quitar uma passagem sem ser cliente | [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=tag-de-pedagio&utm_campaign=sem-parar-free-flow) |
| Gestão de frota e soluções para empresas | [sempararempresas.com.br](https://www.sempararempresas.com.br?utm_source=github&utm_medium=tag-de-pedagio&utm_campaign=sem-parar-free-flow) |

<br>

<sub>Página do repositório oficial mantido pelo <strong>Sem Parar</strong>, sob <a href="LICENSE">CC BY 4.0</a>.</sub>

<sub><strong>Você com mais tempo para o que importa.</strong> #TudoProSeuCarro</sub>

</div>
