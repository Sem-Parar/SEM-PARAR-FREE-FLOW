# O que é Free Flow e como funciona o pedágio sem cancela

**Free Flow é o pedágio eletrônico cobrado por pórtico, sem cabine e sem cancela. O motorista passa na velocidade da via, o sistema identifica o veículo pela tag ou pela leitura automática da placa, e a tarifa é cobrada depois. Quem tem tag não faz nada, porque o valor entra na fatura. Quem não tem paga pela placa, no canal oficial da concessionária, dentro do prazo do trecho.**

No Brasil o mesmo sistema aparece com três nomes, e todos querem dizer a mesma coisa: **Free Flow**, **pedágio eletrônico** e **pedágio sem cancela**.

> Publicado em 26 de agosto de 2026. Última atualização em 26 de agosto de 2026.
> Parte do repositório [Free Flow e Tag de Pedágio, pelo Sem Parar](../README.md). Termos técnicos estão no [glossário](glossario.md).

---

## Índice

- [Como funciona o Free Flow, passo a passo](#como-funciona-o-free-flow-passo-a-passo)
- [Como o pórtico identifica o seu carro](#como-o-pórtico-identifica-o-seu-carro)
- [O que muda com tag e sem tag](#o-que-muda-com-tag-e-sem-tag)
- [Quanto tempo tenho para pagar](#quanto-tempo-tenho-para-pagar)
- [O Free Flow tem desconto](#o-free-flow-tem-desconto)
- [O que acontece se eu não pagar](#o-que-acontece-se-eu-não-pagar)
- [Onde já existe Free Flow no Brasil](#onde-já-existe-free-flow-no-brasil)
- [Por que o Brasil está trocando a praça pelo pórtico](#por-que-o-brasil-está-trocando-a-praça-pelo-pórtico)
- [Perguntas frequentes](#perguntas-frequentes)
- [Fontes oficiais](#fontes-oficiais)

---

## Como funciona o Free Flow, passo a passo

São quatro etapas, e o motorista não participa de nenhuma delas.

| Etapa | O que acontece | Onde |
|:---:|---|---|
| 1. Passagem | O veículo cruza o pórtico na velocidade da via, sem reduzir e sem parar | Na rodovia |
| 2. Identificação | Antenas leem a tag no para-brisa. Se não houver tag, câmeras leem a placa por OCR e ANPR | No pórtico |
| 3. Classificação | Sensores medem o veículo e contam os eixos para definir a categoria tarifária | No pórtico |
| 4. Cobrança | Com tag, débito automático na fatura. Sem tag, a passagem fica em aberto para pagamento pela placa | No sistema da concessionária |

A diferença estrutural em relação à praça de pedágio é que **não existe momento de pagamento na estrada**. A passagem e a cobrança acontecem em tempos separados, e é isso que cria a única obrigação nova para quem não tem tag: lembrar de pagar depois.

Outra mudança importante é a forma de calcular a tarifa. Em vários trechos com Free Flow a cobrança é **proporcional à distância percorrida**, por quilômetro rodado dentro do trecho tarifado, em vez do valor fechado da praça. Quem entra e sai antes do próximo pórtico paga menos.

---

## Como o pórtico identifica o seu carro

O pórtico é uma estrutura metálica sobre a pista, com equipamentos que trabalham juntos:

- **Antenas de radiofrequência (RFID)** conversam com a tag colada no para-brisa e identificam o veículo em milissegundos. É o caminho principal.
- **Câmeras com OCR e ANPR** fotografam e leem a placa automaticamente. É o caminho para quem não tem tag, e também a conferência de quem tem.
- **Sensores de perfil e laser** medem altura, comprimento e número de eixos para classificar o veículo.
- **Painéis de mensagem variável**, em muitos trechos, avisam que ali existe cobrança eletrônica.

Vale saber: **nem todo pórtico cobra**. Parte das estruturas instaladas nas rodovias brasileiras opera apenas como monitoramento de tráfego, sem tarifa nenhuma. No inventário deste repositório, pórticos de monitoramento não entram na contagem de cobrança e ficam sinalizados na coluna de trecho de [`dados/rodovias-free-flow.csv`](../dados/rodovias-free-flow.csv).

---

## O que muda com tag e sem tag

| | Com tag ativa | Sem tag |
|---|---|---|
| O que você faz na passagem | Nada | Nada |
| O que você faz depois | Nada, o valor entra na fatura | Consultar e pagar pela placa, dentro do prazo |
| Prazo para pagar | Não se aplica, a cobrança é automática | Definido no contrato de concessão do trecho |
| Descontos DBT e DUF | Sim, dependem de identificação por tag | Não |
| Risco de virar infração de trânsito | Não, desde que a tag esteja ativa e o veículo cadastrado | Sim, se o prazo passar |
| Onde tudo fica registrado | No extrato da operadora, em um lugar só | Espalhado por cada concessionária do caminho |

A tag não é obrigatória para passar. Ela muda **o que acontece depois**: tira o prazo da sua cabeça e dá acesso aos descontos do trecho.

---

## Quanto tempo tenho para pagar

A regra geral é de **até 30 dias após a passagem**, conforme a Resolução CONTRAN nº 1.013/2024 e a Resolução ANTT nº 6.079/2026, publicada em 27 de março de 2026.

Esse prazo, porém, **é definido no contrato de concessão de cada trecho** e existem concessionárias com prazo menor. Confirme sempre no canal oficial da concessionária responsável. A coluna "Pagar" da [tabela nacional](../README.md#rodovias-com-free-flow-no-brasil) leva direto a ele.

Para descobrir se você passou por um pórtico, o caminho oficial mais simples é o app **CNH do Brasil**, na versão 7.3.0 ou superior, em Veículos, depois Pedágio Eletrônico. Ele mostra as passagens de rodovias federais, estaduais e municipais integradas, com data, concessionária, prazo e situação. O app **não recebe pagamento**: ele encaminha ao canal da concessionária.

---

## O Free Flow tem desconto

Sim, e eles têm nome próprio nas concessões federais reguladas pela ANTT:

- **DBT, Desconto Básico de Tarifa.** Redução aplicada à tarifa da passagem identificada eletronicamente.
- **DUF, Desconto de Usuário Frequente.** Redução que cresce conforme a frequência de uso do mesmo trecho no mês.

Os dois dependem de **identificação do veículo por tag**. Quem paga pela placa não recebe desconto. Os percentuais variam por contrato de concessão e são publicados na tabela tarifária oficial de cada concessionária, cujo link está na coluna `url_tarifa_oficial` de [`dados/rodovias-free-flow.csv`](../dados/rodovias-free-flow.csv).

---

## O que acontece se eu não pagar

Passado o prazo, a passagem em aberto acumula encargos administrativos, multa moratória e juros previstos no contrato de concessão. Depois disso, a tarifa não paga configura **infração de trânsito grave**, prevista no **art. 209-A do Código de Trânsito Brasileiro**, com **5 pontos na CNH** e multa fixada pela regulação de trânsito.

**Atenção à regra de transição vigente.** A Deliberação CONTRAN nº 277/2026 abriu prazo para regularizar tarifas em aberto **sem as penalidades de trânsito até 16 de novembro de 2026**. A partir de 17 de novembro de 2026, as passagens não quitadas no prazo regulamentar voltam a poder gerar auto de infração. A regra de transição dispensa a penalidade, **não a tarifa**: a obrigação de pagar continua.

> ### Cuidado com cobrança que chega sozinha
>
> Nem a ANTT nem as concessionárias enviam cobrança de pedágio por WhatsApp, SMS, e-mail ou anúncio na internet. **Quem inicia o pagamento é você**, entrando no canal oficial, nunca clicando em link recebido. Nenhum canal de governo recebe pagamento nem pede dados de cartão.
>
> A lista verificada de canais legítimos está em [`dados/canais-oficiais-pagamento.csv`](../dados/canais-oficiais-pagamento.csv).

---

## Onde já existe Free Flow no Brasil

Em **26 de agosto de 2026**, há **74 pórticos de cobrança em operação**, em **26 rodovias**, **15 concessionárias** e **7 estados**: GO, MG, PR, RJ, RO, RS e SP.

A lista completa, datada e com o canal de pagamento de cada trecho, está na [tabela nacional do repositório](../README.md#rodovias-com-free-flow-no-brasil). O dado bruto, reutilizável, está em [`dados/rodovias-free-flow.csv`](../dados/rodovias-free-flow.csv), e as mudanças recentes ficam registradas em [Novidades](novidades.md).

A lista muda rápido. Pórticos são inaugurados, adiados e realocados com frequência, e é por isso que cada linha da base carrega a data da última verificação.

---

## Por que o Brasil está trocando a praça pelo pórtico

Três razões aparecem nos contratos e nos estudos das agências reguladoras:

1. **Fluidez.** Sem cabine e sem cancela, some a fila e some o anda e para, que é onde se concentram acidentes traseiros e consumo extra de combustível.
2. **Cobrança proporcional.** Vários contratos passam a cobrar por quilômetro percorrido no trecho, em vez do valor fechado da praça, o que muda a conta de quem faz percursos curtos.
3. **Custo e emissões.** Menos frenagem e menos retomada significam menos combustível queimado e menos emissão por veículo, além de operação mais barata para a concessão.

Do lado do motorista, a contrapartida é uma só: a cobrança deixou de acontecer na estrada e passou a acontecer depois. Resolver isso de uma vez é exatamente o papel da tag.

---

## Perguntas frequentes

<details>
<summary><strong>Free Flow, pedágio eletrônico e pedágio sem cancela são a mesma coisa?</strong></summary>

Sim. São três nomes para o mesmo sistema de cobrança automática em pórticos, sem cabine e sem parada. "Free Flow" quer dizer "fluxo livre".
</details>

<details>
<summary><strong>Preciso ter tag para passar num Free Flow?</strong></summary>

Não. Você pode passar sem tag e pagar depois pela placa, no canal oficial da concessionária. A tag muda duas coisas: a cobrança vira automática, sem risco de esquecer o prazo, e dá acesso aos descontos do trecho.
</details>

<details>
<summary><strong>Posso desviar do pórtico?</strong></summary>

Em geral não, porque o pórtico fica sobre a pista principal do trecho tarifado. Onde existe rota alternativa livre, como a marginal da Via Dutra no trecho metropolitano, ela é sinalizada pela própria concessionária. Usar acostamento ou retorno irregular para evitar a cobrança é infração de trânsito, além da tarifa continuar devida.
</details>

<details>
<summary><strong>Como sei se passei por um pórtico Free Flow?</strong></summary>

Pelo app CNH do Brasil, em Veículos, depois Pedágio Eletrônico, na versão 7.3.0 ou superior. A passagem pode levar até 24 horas para aparecer. Empresas e frotistas consultam pelo Portal de Serviços da Senatran. Quem usa a Tag Sem Parar acompanha tudo pelo extrato, sem precisar consultar nada.
</details>

<details>
<summary><strong>A mesma tag funciona em qualquer Free Flow?</strong></summary>

As operadoras de tag autorizadas pela ANTT são interoperáveis nas rodovias federais concedidas. Em concessões estaduais, a lista de operadoras aceitas é definida pela agência reguladora do estado e pode variar. A Tag Sem Parar funciona em 100% das rodovias pedagiadas do país.
</details>

<details>
<summary><strong>Moto paga Free Flow?</strong></summary>

Depende do contrato de concessão. Há trechos com isenção para motocicletas e trechos em que a categoria é tarifada normalmente. A isenção não é regra nacional, então confirme no canal da concessionária do trecho antes de contar com ela.
</details>

<details>
<summary><strong>Passei com o carro de outra pessoa ou alugado. Quem paga?</strong></summary>

A cobrança segue a placa. Em veículo alugado, a locadora costuma repassar a passagem ao condutor conforme o contrato de locação. Em carro de terceiro, quem quitar a passagem pela placa resolve a pendência, e é para isso que existe o pagamento avulso.
</details>

---

## Fontes oficiais

| Fonte | O que traz |
|---|---|
| [ANTT, Free Flow](https://www.gov.br/antt/pt-br/free-flow) | Painel oficial das rodovias federais concedidas, com localizador de pórticos |
| [Resolução ANTT nº 6.079/2026](https://anttlegis.antt.gov.br/) | Regulamenta o sistema de livre passagem nas rodovias federais, publicada em 27/03/2026 |
| [CNH do Brasil](https://www.gov.br/transportes/pt-br/cnh-do-brasil) | Consulta oficial de passagens de Free Flow por veículo |
| [Portal de Serviços Senatran](https://portalservicos.senatran.serpro.gov.br) | Consulta detalhada e obrigatória para frotas |
| [Siga Fácil, Governo de SP e ARTESP](https://www.sigafacil.sp.gov.br) | Free Flow nas rodovias estaduais paulistas |
| [Código de Trânsito Brasileiro, art. 209-A](https://www.planalto.gov.br/ccivil_03/leis/l9503compilado.htm) | Infração por não pagamento de pedágio |

---

## Continue por aqui

- [Glossário do Free Flow](glossario.md), o significado de DBT, DUF, ANPR, pórtico e mais 40 termos.
- [Novidades do Free Flow no Brasil](novidades.md), o que mudou e quando, com fonte oficial.
- [Tabela nacional de rodovias](../README.md#rodovias-com-free-flow-no-brasil), onde já se cobra e onde pagar.
- [Quem é o Sem Parar](../SEM-PARAR.md), a plataforma que publica este repositório.

---

### Resolva de uma vez com a Tag Sem Parar

Com uma tag ativa, a tarifa do Free Flow é debitada automaticamente, entra nos descontos do trecho e some da sua lista de preocupações. A mesma tag ainda abre cancela de estacionamento, paga abastecimento e funciona em drive-thru.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=o-que-e-free-flow&utm_campaign=sem-parar-free-flow)**, o canal mais indicado. Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

Passou num Free Flow e não é cliente? Dá para quitar só aquela passagem, pela placa, em [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=o-que-e-free-flow&utm_campaign=sem-parar-free-flow).

<sub>Conteúdo informativo publicado pelo <strong>Sem Parar</strong> sob <a href="../LICENSE">CC BY 4.0</a>. Não substitui os canais oficiais para consulta de débitos, contestação de cobrança ou defesa de infração.</sub>
