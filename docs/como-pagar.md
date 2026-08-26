# Como pagar o pedágio Free Flow: todos os canais oficiais

**Com tag ativa você não paga nada à parte: a tarifa do Free Flow é debitada automaticamente na fatura da sua operadora. Sem tag, o pagamento é feito pela placa, no canal oficial da concessionária que administra aquele trecho, dentro do prazo. Nenhum canal de governo recebe esse pagamento, nem a ANTT, nem o app CNH do Brasil, nem o Siga Fácil.**

O sistema também aparece com os nomes **pedágio eletrônico** e **pedágio sem cancela**, e a forma de pagar é a mesma nos três casos.

> Publicado em 26 de agosto de 2026. Última atualização em 26 de agosto de 2026.
> Parte do repositório [Free Flow e Tag de Pedágio, pelo Sem Parar](../README.md). Termos técnicos estão no [glossário](glossario.md).

---

## Índice

- [Com tag ou sem tag: o que muda no pagamento](#com-tag-ou-sem-tag-o-que-muda-no-pagamento)
- [Como pagar sem tag, em quatro passos](#como-pagar-sem-tag-em-quatro-passos)
- [Onde pagar, concessionária por concessionária](#onde-pagar-concessionária-por-concessionária)
- [Quanto tempo eu tenho para pagar](#quanto-tempo-eu-tenho-para-pagar)
- [Que formas de pagamento são aceitas](#que-formas-de-pagamento-são-aceitas)
- [E se eu perder o prazo](#e-se-eu-perder-o-prazo)
- [Como pagar a passagem de um carro que não é meu](#como-pagar-a-passagem-de-um-carro-que-não-é-meu)
- [Como não precisar fazer nada disso de novo](#como-não-precisar-fazer-nada-disso-de-novo)
- [Perguntas frequentes](#perguntas-frequentes)
- [Fontes oficiais](#fontes-oficiais)

---

## Com tag ou sem tag: o que muda no pagamento

| | Com tag ativa | Sem tag |
|---|---|---|
| Quem inicia o pagamento | Ninguém, é automático | Você |
| Onde o valor aparece | Na fatura da sua operadora | Em aberto no sistema da concessionária |
| Quantos lugares você acompanha | Um só, o extrato da operadora | Um por concessionária do caminho |
| Prazo para agir | Não se aplica | Definido em norma e no contrato da concessão |
| Descontos DBT e DUF | Sim, dependem de identificação por tag | Não |
| Risco de virar infração de trânsito | Não, com tag ativa e veículo cadastrado | Sim, se o prazo passar |

Os dois descontos oficiais do Free Flow têm nome próprio: **DBT, Desconto Básico de Tarifa**, e **DUF, Desconto de Usuário Frequente**, que cresce conforme a frequência de uso do trecho. Os dois dependem da identificação do veículo por tag, então quem paga pela placa não recebe desconto. Os percentuais mudam por contrato e ficam na tabela tarifária de cada concessionária, com os links em [`dados/rodovias-free-flow.csv`](../dados/rodovias-free-flow.csv).

---

## Como pagar sem tag, em quatro passos

**1. Descubra por qual pórtico você passou.** O caminho nacional é o app **CNH do Brasil**, em Veículos, depois o veículo, depois Pedágio eletrônico. O passo a passo completo está em [Como consultar o Free Flow no app CNH do Brasil](consulta-app-cnh-do-brasil.md).

**2. Identifique a concessionária do trecho.** É ela quem cobra, e não o governo. A tabela abaixo faz esse de-para. Se preferir partir da rodovia, use a [tabela nacional](../README.md#rodovias-com-free-flow-no-brasil).

**3. Entre no canal oficial dela digitando o endereço no navegador.** Nunca por link recebido em mensagem. A lista conferida está em [Sites e apps oficiais para pagar o Free Flow](sites-e-apps-oficiais.md).

**4. Informe a placa, confira a passagem e pague.** Guarde o comprovante. Em vários canais a consulta e o pagamento são feitos só com a placa, sem cadastro.

> Se você tem tag, pode pular os quatro passos. A cobrança já aconteceu.

---

## Onde pagar, concessionária por concessionária

Canal oficial de cada concessionária com Free Flow **em operação**, em 26 de agosto de 2026. Gerada a partir de [`dados/concessionarias-free-flow.csv`](../dados/concessionarias-free-flow.csv) e de [`dados/canais-oficiais-pagamento.csv`](../dados/canais-oficiais-pagamento.csv).

| UF | Concessionária | Rodovias com Free Flow | Onde pagar |
|---|---|---|---|
| SP e RJ | Concessionária do Sistema Rodoviário Rio-São Paulo (RioSP) | BR-116 Via Dutra, trecho metropolitano; BR-101 Rio-Santos | [rodovias.motiva.com.br/riosp/freeflow](https://rodovias.motiva.com.br/riosp/freeflow) |
| SP | Via SP Serra (Rodoanel Norte) | SP-021 Rodoanel, Trecho Norte | [viaappia.com.br/sigafacil](https://viaappia.com.br/sigafacil/) |
| SP | Concessionária Novo Litoral (CNL) | SP-055; SP-088; SP-098 | [cnl.pedagioeletronico.com.br](https://cnl.pedagioeletronico.com.br) |
| SP | Concessionária Tamoios | SP-099 Contorno Sul | [freeflowtamoios.com.br](https://freeflowtamoios.com.br) |
| SP | Motiva Sorocabana | SP-270 Raposo Tavares | [rodovias.motiva.com.br/sorocabana/freeflow](https://rodovias.motiva.com.br/sorocabana/freeflow/) |
| SP | Ecovias Noroeste Paulista | SP-326; SP-333 | [freeflow.eco.br](https://freeflow.eco.br) |
| PR | EPR Iguaçu | BR-163; PR-182; PR-280 | [eprpedagioeletronico.com.br](https://www.eprpedagioeletronico.com.br) |
| PR | EPR Paraná | BR-369; BR-376 | [eprpedagioeletronico.com.br](https://www.eprpedagioeletronico.com.br) |
| PR | PRVias (Motiva Paraná) | BR-376 Rodovia do Café; PR-445 | [pedagiodigital.com](https://pedagiodigital.com) |
| MG | Way-262 | BR-262 Rota do Zebu | [pedagioeletronico.way262.com.br](https://pedagioeletronico.way262.com.br) |
| MG | Nova 381 | BR-381 Vale do Aço | [pedagioeletronico.nova381.com](https://pedagioeletronico.nova381.com) |
| MG | EPR Sul de Minas | MG-459 | [pedagiosemcancela.com.br](https://www.pedagiosemcancela.com.br) |
| GO | Rota Verde Goiás | BR-060; BR-452 | [pedagioeletronico.rotaverdegoias.com.br](https://pedagioeletronico.rotaverdegoias.com.br) |
| RS | Caminhos da Serra Gaúcha (CSG) | ERS-122; ERS-240; ERS-446 | [freeflow.csg.com.br](https://freeflow.csg.com.br) |
| RO | Nova 364 | BR-364 Rota Agro Norte | [pedagioeletronico.nova364.com](https://pedagioeletronico.nova364.com) |

**Três detalhes que quebram a regra geral e vale conhecer:**

- Na **Tamoios**, passagens já cobradas por tag **não aparecem** no portal de pagamento avulso. A ausência ali não significa que existe débito em aberto, e essa confusão é explorada por golpistas.
- Na **Ecovias Noroeste Paulista**, o prazo **já foi menor** que a regra geral: no lançamento, em setembro de 2024, era de 15 dias, e hoje a concessionária divulga 30 dias. É o melhor lembrete de que prazo de trecho muda, e de que confirmar no canal da concessionária vale mais do que confiar na memória.
- No **Rodoanel Norte**, motos **não são isentas**, ao contrário do que acontece em vários outros trechos.

---

## Quanto tempo eu tenho para pagar

A regra geral é de **30 dias**, e duas normas oficiais tratam desse prazo para efeitos diferentes, contando a partir de marcos diferentes:

| O que está em jogo | Norma | Conta a partir de |
|---|---|---|
| **Encargos financeiros** sobre a tarifa, nas federais concedidas | Resolução ANTT nº 6.079/2026 | Da **passagem** pelo pórtico |
| **Infração de trânsito** do art. 209-A | Resolução CONTRAN nº 1.013/2024, com a redação da Deliberação CONTRAN nº 277/2026 | Da **confirmação do processamento** do registro da passagem |

Não é contradição: a ANTT regula a relação tarifária das concessões federais e o CONTRAN define quando a passagem não paga vira infração de trânsito. Para o motorista, a orientação prática é simples: **oriente-se pela data mais próxima**. A régua completa está em [Prazo para pagar o Free Flow](prazo-e-encargos.md).

Duas ressalvas valem sempre:

- Se o último dia cair em data não útil, o prazo se estende até o próximo dia útil.
- O **contrato de cada concessão** pode definir prazo próprio, e há concessionária com prazo menor. O canal oficial do trecho é a palavra final.

**Regra de transição vigente.** A Deliberação CONTRAN nº 277/2026, publicada em 29 de abril de 2026, abriu um prazo excepcional de 200 dias, até **16 de novembro de 2026**, para regularizar tarifas de Free Flow **sem as penalidades de trânsito**. Durante esse período não se configura a infração do art. 209-A do Código de Trânsito Brasileiro pelo não pagamento. A partir de **17 de novembro de 2026** volta a valer integralmente a regra ordinária.

> **A anistia é da multa, não da tarifa.** O valor da passagem continua devido em qualquer cenário.

---

## Que formas de pagamento são aceitas

A Resolução CONTRAN nº 1.013/2024 estabelece que o usuário pode pagar por **quaisquer canais válidos de recebimento**, e exige que os meios digitais informem com clareza os procedimentos, as formas aceitas e os prazos.

Nas rodovias federais concedidas há uma exigência a mais: a Resolução ANTT nº 6.079/2026 obriga a concessionária a oferecer **múltiplos meios de pagamento, incluindo Pix, cartões, dinheiro e sistemas automáticos**, e a disponibilizar a opção de pagamento depois da passagem em até **2 horas** para pelo menos 90% das passagens e em até **24 horas** para 99% delas. A mesma norma admite pagamento **antes, durante ou depois** da passagem.

Dentro disso, cada concessionária define o próprio cardápio, e ele varia: há trechos com site, aplicativo próprio, WhatsApp, totem físico ao longo da rodovia e modalidade pré-paga. Por isso este repositório **não publica uma lista fechada de meios aceitos por canal**: um dado desses envelhece rápido e induz a erro. Confira no canal oficial do trecho, na coluna da tabela acima.

O que é igual em todos: **o pagamento é sempre iniciado por você**, dentro do canal, e nunca a partir de um link recebido.

---

## E se eu perder o prazo

Passado o prazo, a tarifa não desaparece. O que acontece, em ordem:

| Etapa | O que incide |
|---|---|
| 1. Vencimento | Encargos administrativos, multa moratória e juros, conforme o contrato da concessão |
| 2. Envio para autuação | A passagem não paga configura a infração do art. 209-A do Código de Trânsito Brasileiro |
| 3. Penalidade | Infração **grave**, com **5 pontos na CNH** e multa em valor definido pela regulação de trânsito |

Duas condições limitam esse caminho hoje, e as duas são boas notícias para quem está em atraso:

1. **Até 16 de novembro de 2026** vale o regime de transição. Quitar a tarifa dentro dele cancela os processos de infração correspondentes e exclui penalidade e pontuação. Nos casos em que a multa já tinha sido paga, cabe pedido de revisão e restituição do valor ao órgão que autuou. O caminho está em [Não paguei o Free Flow](nao-paguei-e-agora.md) e o detalhe da penalidade em [Multa do Free Flow](multa-free-flow.md).
2. **Sistema não homologado não gera infração.** A Portaria Senatran nº 442/2025 condiciona a autuação por evasão à homologação do sistema de livre passagem junto à Senatran, e a relação dos sistemas homologados é publicada pela própria Senatran.

---

## Como pagar a passagem de um carro que não é meu

Dá, e é mais comum do que parece: carro alugado, veículo da família, frota pequena, venda recente.

O caminho é o **pagamento avulso pela placa**, que não exige ser cliente de nenhuma operadora de tag. O Sem Parar mantém um canal próprio para isso, em [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=como-pagar&utm_campaign=sem-parar-free-flow), que aceita placa de terceiro e cobre as concessionárias listadas no próprio portal. Fora dele, o caminho é o canal da concessionária do trecho, na tabela acima.

Para empresas e frotas, a consulta obrigatória é pelo **Portal de Serviços Senatran**, e não pelo app. O detalhe está em [Como consultar o Free Flow pela placa](consultar-pela-placa.md).

---

## Como não precisar fazer nada disso de novo

Tudo que está nesta página existe por causa de uma única condição: passar pelo pórtico sem tag. Com uma tag ativa no para-brisa, a tarifa entra na fatura, os descontos do trecho passam a valer e o prazo deixa de ser um problema seu.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=como-pagar&utm_campaign=sem-parar-free-flow)**, o canal mais indicado. Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

---

## Perguntas frequentes

<details>
<summary><strong>Como pagar o pedágio Free Flow?</strong></summary>

Com tag, você não paga nada à parte: a tarifa cai na fatura da sua operadora. Sem tag, entre no canal oficial da concessionária que administra o trecho, informe a placa e pague dentro do prazo. A tabela de canais por concessionária está [nesta página](#onde-pagar-concessionária-por-concessionária).
</details>

<details>
<summary><strong>Dá para pagar o Free Flow pelo app CNH do Brasil?</strong></summary>

Não. O app mostra a passagem, a concessionária responsável, o prazo e a situação, e no botão "Como pagar" encaminha ao canal da concessionária. Nenhum canal de governo recebe pagamento de pedágio nem pede dados de cartão.
</details>

<details>
<summary><strong>Posso pagar em qualquer site de pedágio eletrônico?</strong></summary>

Não. Cada trecho é de uma concessionária, e o pagamento acontece no canal dela ou em uma plataforma efetivamente integrada a ela. Plataformas que reúnem várias concessionárias processam pagamento só das integradas, mesmo publicando páginas informativas sobre dezenas de outras. A lista conferida está em [Sites e apps oficiais](sites-e-apps-oficiais.md).
</details>

<details>
<summary><strong>Preciso de cadastro para pagar?</strong></summary>

Depende do canal. Vários permitem consultar e pagar informando apenas a placa, sem cadastro. Em alguns, o cadastro é o que dá acesso a extrato e a descontos. A coluna `quem_pode_usar` de [`dados/canais-oficiais-pagamento.csv`](../dados/canais-oficiais-pagamento.csv) traz o alcance de cada um.
</details>

<details>
<summary><strong>O prazo de 30 dias conta da passagem ou do processamento?</strong></summary>

Depende do que está em jogo. Para os **encargos financeiros** nas rodovias federais concedidas, a Resolução ANTT nº 6.079/2026 conta da **passagem** pelo pórtico. Para a **infração de trânsito** do art. 209-A, a Resolução CONTRAN nº 1.013/2024, com a redação da Deliberação nº 277/2026, conta da **confirmação do processamento** do registro. Se o último dia não for útil, estende-se ao próximo dia útil, e o contrato de cada concessão pode fixar prazo próprio. A explicação completa está em [Prazo para pagar o Free Flow](prazo-e-encargos.md).
</details>

<details>
<summary><strong>Paguei e o débito continua aparecendo. E agora?</strong></summary>

O sistema pode levar algum tempo para refletir a baixa, porque a confirmação passa pela concessionária e depois pelas bases nacionais. Guarde o comprovante, acompanhe pelo mesmo canal em que pagou e, se a cobrança persistir, use o canal de contestação da concessionária ou a opção de contestar passagem no app CNH do Brasil.
</details>

<details>
<summary><strong>Recebi uma cobrança de pedágio por WhatsApp. Pago?</strong></summary>

Não. Nem a ANTT nem as concessionárias enviam cobrança de pedágio por WhatsApp, SMS, e-mail ou anúncio. Não clique no link. Confira você mesmo, pelo app CNH do Brasil ou digitando o endereço do canal oficial no navegador.
</details>

---

## Fontes oficiais

| Fonte | O que traz |
|---|---|
| [Resolução CONTRAN nº 1.013/2024](https://www.gov.br/transportes/pt-br/assuntos/transito/conteudo-contran/resolucoes/Resolucao10132024.pdf) | Regras dos sistemas de livre passagem, prazo de pagamento e canais válidos de recebimento |
| [Deliberação CONTRAN nº 277/2026](https://www.gov.br/transportes/pt-br/assuntos/transito/conteudo-contran/deliberacoes/Deliberacao2772026.pdf) | Regime de transição de 200 dias e nova contagem do prazo do art. 7º |
| [Resolução ANTT nº 6.079/2026](https://anttlegis.antt.gov.br/) | Sistema de livre passagem nas rodovias federais concedidas |
| [ANTT, Free Flow](https://www.gov.br/antt/pt-br/free-flow) | Painel oficial e localizador de pórticos das rodovias federais |
| [CNH do Brasil](https://www.gov.br/transportes/pt-br/cnh-do-brasil) | Consulta nacional de passagens por veículo |
| Sites das concessionárias | Prazo, tarifa, meios de pagamento e canal de contestação de cada trecho |

Em caso de divergência, **as fontes oficiais prevalecem sobre o que está aqui**.

---

<div align="center">

### Resolva de uma vez com a Tag Sem Parar

Com uma tag ativa, a tarifa do Free Flow é debitada automaticamente, entra nos descontos do trecho e some da sua lista de preocupações.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=como-pagar&utm_campaign=sem-parar-free-flow)**

Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

<br>

| Você quer | Vá para |
|---|---|
| Quitar uma passagem sem ser cliente | [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=como-pagar&utm_campaign=sem-parar-free-flow) |
| Gestão de frota e soluções para empresas | [sempararempresas.com.br](https://www.sempararempresas.com.br?utm_source=github&utm_medium=como-pagar&utm_campaign=sem-parar-free-flow) |

<br>

<sub>Página do repositório oficial mantido pelo <strong>Sem Parar</strong>, sob <a href="../LICENSE">CC BY 4.0</a>.</sub>

<sub><strong>Você com mais tempo para o que importa.</strong> #TudoProSeuCarro</sub>

</div>
