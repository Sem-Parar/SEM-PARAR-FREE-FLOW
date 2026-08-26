# Golpe do falso pedágio: como identificar e o que fazer

**Nem a ANTT nem as concessionárias enviam cobrança de pedágio por WhatsApp, SMS, e-mail ou correio. Não existe boleto automático de Free Flow e não existe um site único nacional para consultar débito. Quem inicia o pagamento é sempre o motorista, digitando o endereço oficial no navegador. Se a cobrança chegou até você, com link, QR Code ou chave Pix, é golpe até prova em contrário.**

Os golpistas copiam o visual das telas oficiais com perfeição. O que eles não conseguem copiar é o endereço do site. É ali que o golpe aparece.

> Publicado em 26 de agosto de 2026. Última atualização em 26 de agosto de 2026.
> Parte do repositório [Free Flow e Tag de Pedágio, pelo Sem Parar](../README.md). Canais verificados em [`dados/canais-oficiais-pagamento.csv`](../dados/canais-oficiais-pagamento.csv).

---

## Índice

- [As duas modalidades em circulação](#as-duas-modalidades-em-circulação)
- [O teste do endereço, em dez segundos](#o-teste-do-endereço-em-dez-segundos)
- [Quatro coisas que nenhum canal oficial faz](#quatro-coisas-que-nenhum-canal-oficial-faz)
- [Os sinais dentro da página falsa](#os-sinais-dentro-da-página-falsa)
- [Por que o resultado patrocinado é um risco](#por-que-o-resultado-patrocinado-é-um-risco)
- [O golpe usa a lei errada, e isso entrega](#o-golpe-usa-a-lei-errada-e-isso-entrega)
- [Cobrança de rodovia que não cobra](#cobrança-de-rodovia-que-não-cobra)
- [Caí no golpe. E agora?](#caí-no-golpe-e-agora)
- [Como conferir do jeito seguro](#como-conferir-do-jeito-seguro)
- [Perguntas frequentes](#perguntas-frequentes)
- [Fontes oficiais](#fontes-oficiais)

---

## As duas modalidades em circulação

A ANTT publicou alerta oficial descrevendo os dois formatos mais comuns.

**1. Página falsa de consulta.** O golpista cria um site que imita o serviço oficial de consulta de pedágio. O motorista digita a placa, a tela informa que existem débitos em aberto e gera uma **chave Pix que direciona o pagamento ao golpista**. Como o valor costuma ser baixo e plausível, muita gente paga sem desconfiar.

**2. Boleto falso.** Boletos são enviados para o endereço físico ou para o e-mail da vítima, com logotipo de concessionária real, linguagem formal e QR Code, usando dados obtidos de forma irregular.

O que as duas têm em comum: **a cobrança chega até você.** No Free Flow real, é o contrário. Você é quem procura o canal da concessionária. A ANTT é explícita: não há envio automático de boletos por correio, nem site único para consulta de débitos.

---

## O teste do endereço, em dez segundos

Golpistas copiam marca, cores e layout. Não conseguem copiar o domínio. Antes de digitar qualquer dado, olhe a barra do navegador e examine **o trecho imediatamente antes do `.com` ou `.com.br`**. Ele precisa ser exatamente o nome da empresa, sem nada a mais.

| Sinal no endereço | Leitura |
|---|---|
| Nome exato da empresa, sem acréscimos | Provavelmente legítimo, mas confirme na lista oficial |
| Nome da empresa **com palavra ou hífen a mais** | Indício forte de fraude |
| **Terminação diferente** do endereço oficial, como `.net` ou domínio de loja virtual | O sinal mais claro de fraude |
| `.br` acrescentado ou removido em relação ao endereço oficial | Indício forte de fraude |

Esse último caso é real e vale conhecer porque pega gente atenta: o portal do **Pedágio Digital**, usado pelas concessionárias da Motiva e da EcoRodovias, tem endereço terminado em **`.com`, sem `.br`**. Endereços que acrescentam o `.br`, ou que colocam uma palavra antes do nome, são fraude, e já foram identificados publicamente como tal em checagem de imprensa.

A regra que dispensa memorizar domínio: **chegue ao pagamento pelo site da concessionária**, digitando o endereço dela no navegador e seguindo o link de lá. Quem é que cobra em cada trecho está em [Concessionárias com Free Flow no Brasil](../CONCESSIONARIAS-FREE-FLOW.md).

---

## Quatro coisas que nenhum canal oficial faz

Guarde estas quatro e você já filtra a maior parte das tentativas.

**Não envia cobrança por mensagem.** ANTT e concessionárias declaram isso abertamente. A EPR publica que não envia boletos aos usuários. A Concessionária Novo Litoral declara que não envia links nem boletos. A EcoRodovias alerta que o Pedágio Digital não envia links de cobrança por redes sociais ou aplicativos de mensagens, nem encaminha boletos por e-mail.

**Não recebe pagamento em canal de governo.** ANTT, app CNH do Brasil, Portal Senatran e Siga Fácil apenas mostram a passagem e encaminham à concessionária. **Qualquer tela com marca de governo pedindo dados de cartão para quitar pedágio é fraude.**

**Não impõe pressa.** Não existe contagem regressiva de minutos para pagar pedágio. O prazo real é medido em dias, não em minutos.

**Não ameaça com multa imediata.** A multa do art. 209-A é aplicada pelo órgão autuador, seguindo rito próprio, e não é emitida automaticamente por um site depois de alguns minutos.

---

## Os sinais dentro da página falsa

Se o endereço não bastou, esses detalhes confirmam a suspeita:

- **Contagem regressiva.** Telas falsas usam um cronômetro, às vezes de 15 minutos, dizendo que depois disso a multa é emitida automaticamente. Nada disso existe.
- **Débito encontrado para qualquer placa.** Em simulações de checagem, páginas falsas devolveram "débitos em aberto" até para placas digitadas ao acaso.
- **Ameaça de encaminhamento imediato ao Detran.**
- **Pagamento apenas por Pix**, com chave gerada na hora, sem outras opções.
- **Valores estranhamente quebrados e baixos**, calculados para não levantar suspeita.

---

## Por que o resultado patrocinado é um risco

Uma parte relevante das fraudes chega por **anúncio pago**. Os links falsos aparecem como resultados patrocinados **acima** do site oficial na busca, e quem clica no primeiro resultado sem ler o endereço cai direto na cópia.

A recomendação prática, e é a mesma que a Motiva publica na página de alerta dela: **não chegue ao pagamento pela busca.** Digite o endereço da concessionária no navegador, ou use o app oficial que você já baixou.

---

## O golpe usa a lei errada, e isso entrega

Um detalhe curioso e útil: as páginas falsas costumam **citar o art. 209-A do CTB com um texto inventado**, algo como "efetuar o pagamento de pedágio eletrônico fora do prazo estabelecido pelo órgão".

Não é o que o artigo diz. O texto real é:

> **Art. 209-A.** Evadir-se da cobrança pelo uso de rodovias e vias urbanas para não efetuar o seu pagamento, ou deixar de efetuá-lo na forma estabelecida.

Quem conhece o texto reconhece a falsificação na hora. A base legal completa, com o que cada norma define, está em [Base legal do Free Flow](../BASE-LEGAL-DO-FREE-FLOW.md).

---

## Cobrança de rodovia que não cobra

Existe uma checagem que quase ninguém faz e que derruba o golpe na origem: **conferir se aquele trecho cobra por pórtico hoje.**

Vários pórticos estão instalados e ainda não cobram. O caso mais visível é o **Sistema Anchieta-Imigrantes**, onde os pórticos existem, o sistema até já foi homologado pela Senatran, e a cobrança segue adiada. Também estão nessa situação trechos da Rota Sorocabana e o lote da Via Campo, no Paraná.

**Cobrança apresentada em nome de qualquer trecho que ainda não cobra é fraude, sem meio-termo.** A lista completa dos pórticos instalados que não cobram está em [Rodovias com Free Flow no Brasil](../RODOVIAS-COM-FREE-FLOW.md) e no dado bruto em [`dados/porticos-free-flow.csv`](../dados/porticos-free-flow.csv).

---

## Caí no golpe. E agora?

Ordem importa, porque as primeiras horas contam.

1. **Acione o seu banco imediatamente.** Pix pago por fraude pode entrar no Mecanismo Especial de Devolução, e o prazo é curto. Peça o registro da contestação.
2. **Registre boletim de ocorrência.** É o que sustenta qualquer pedido posterior.
3. **Denuncie aos órgãos de defesa do consumidor** e às autoridades competentes. A ANTT orienta exatamente isso quando há indício de golpe.
4. **Avise a concessionária ou a plataforma imitada.** Elas mantêm canais de alerta e conseguem pedir a retirada da página falsa.
5. **Depois disso, pague a tarifa de verdade**, no canal oficial. Este é o passo que as pessoas esquecem: **o dinheiro perdido para o golpista não quitou nada**, e o prazo do trecho continua correndo.
6. **Troque senhas** se você informou dados além da placa.

Se você não tem certeza de que a cobrança era falsa, o caminho é [Cobrança indevida de pedágio: como contestar](cobranca-indevida-como-contestar.md).

---

## Como conferir do jeito seguro

Três caminhos, todos gratuitos e nenhum deles depende de link recebido:

| Caminho | Como |
|---|---|
| **App CNH do Brasil** | Em Veículos, selecione o veículo, depois Pedágio eletrônico. Mostra a passagem com concessionária, valor e prazo, e **não recebe pagamento**. O passo a passo está em [Como consultar o Free Flow no app CNH do Brasil](consulta-app-cnh-do-brasil.md) |
| **Site da concessionária** | Digite o endereço no navegador. O de-para de rodovia para concessionária está em [Como consultar o Free Flow pela placa](consultar-pela-placa.md) |
| **Sua operadora de tag** | Se você tem tag, o extrato dela é a fonte, e ali não existe cobrança surpresa |

E a lista verificada de 29 canais legítimos, conferidos um a um, está em [Sites e apps oficiais para pagar o Free Flow](sites-e-apps-oficiais.md).

---

## Perguntas frequentes

<details>
<summary><strong>Recebi um SMS cobrando pedágio Free Flow. É golpe?</strong></summary>

Quase certamente sim. Nem a ANTT nem as concessionárias enviam cobrança de pedágio por SMS, WhatsApp, e-mail ou correio, e várias declaram isso no próprio site. Não clique no link. Confira você mesmo, pelo app CNH do Brasil ou digitando o endereço oficial da concessionária no navegador.
</details>

<details>
<summary><strong>Existe um site único para consultar pedágio de todas as rodovias?</strong></summary>

Para **pagar**, não. A ANTT afirma que não existe site único de consulta de débitos: o pagamento é feito com a concessionária responsável pelo trecho. Para **consultar**, o app CNH do Brasil reúne as passagens de várias concessionárias, mas ele não recebe pagamento.
</details>

<details>
<summary><strong>Como sei se o site é o oficial?</strong></summary>

Olhe o trecho do endereço imediatamente antes do `.com` ou `.com.br`: ele tem que ser exatamente o nome da empresa, sem palavra extra, sem hífen a mais e com a terminação correta. Mais seguro ainda é não depender disso: chegue ao pagamento pelo site da concessionária, digitando o endereço no navegador.
</details>

<details>
<summary><strong>O site pediu Pix e deu 15 minutos de prazo. É normal?</strong></summary>

Não. Não existe contagem regressiva para pagar pedágio, e nenhum canal oficial emite multa automaticamente após minutos. O prazo real é medido em dias e é definido em norma e no contrato de concessão. Cronômetro na tela é sinal de fraude.
</details>

<details>
<summary><strong>Paguei um boleto falso. Ainda devo o pedágio?</strong></summary>

Sim. O pagamento feito ao golpista não quita nada com a concessionária, e o prazo do trecho continua correndo. Acione o banco e registre a ocorrência, e depois pague a tarifa real no canal oficial, para não acumular um segundo problema.
</details>

<details>
<summary><strong>Quem tem tag corre esse risco?</strong></summary>

Menos, e por um motivo estrutural: com tag ativa não existe débito em aberto para o golpista alegar, e a cobrança já cai na fatura da operadora. Qualquer mensagem dizendo que você tem pedágio pendente pode ser conferida em segundos no extrato. O risco que permanece é o de informar dados numa página falsa, e para esse a defesa é a mesma.
</details>

---

## Fontes oficiais

| Fonte | O que traz |
|---|---|
| [ANTT, alerta sobre golpes no Free Flow](https://www.gov.br/antt/pt-br/assuntos/ultimas-noticias/antt-alerta-para-golpes-que-usam-o-nome-do-free-flow-para-enganar-motoristas) | As duas modalidades em circulação e as recomendações oficiais |
| [Motiva, golpes de pagamento](https://rodovias.motiva.com.br/golpes-de-pagamento) | Como reconhecer site falso pelo endereço, com exemplos |
| [EcoRodovias, alerta sobre golpes](https://www.ecorodovias.com.br/noticias/alerta-sobre-golpes-que-usam-nome-do-pedagio-digital) | O que o Pedágio Digital não faz |
| [ANTT, Free Flow](https://www.gov.br/antt/pt-br/free-flow) | Regulação e canais oficiais |
| [CNH do Brasil](https://www.gov.br/transportes/pt-br/cnh-do-brasil) | Consulta oficial de passagens por veículo |

Em caso de divergência, as fontes oficiais prevalecem sobre o que está aqui.

---

<div align="center">

### Sem débito em aberto, não há o que fingir

Com a Tag Sem Parar, a tarifa é debitada automaticamente e cada passagem fica registrada no seu extrato. Cobrança que chega por mensagem vira fácil de desmentir.

**[Peça sua tag em semparar.com.br](https://www.semparar.com.br/free-flow?utm_source=github&utm_medium=golpe-falso-pedagio&utm_campaign=sem-parar-free-flow)**

Se preferir, a contratação também pode ser feita pelo SuperApp Sem Parar.

<br>

| Você quer | Vá para |
|---|---|
| Quitar uma passagem sem ser cliente | [pedagioeletronicosemparar.com.br](https://www.pedagioeletronicosemparar.com.br?utm_source=github&utm_medium=golpe-falso-pedagio&utm_campaign=sem-parar-free-flow) |
| Gestão de frota e soluções para empresas | [sempararempresas.com.br](https://www.sempararempresas.com.br?utm_source=github&utm_medium=golpe-falso-pedagio&utm_campaign=sem-parar-free-flow) |

<br>

<sub>Página do repositório oficial mantido pelo <strong>Sem Parar</strong>, sob <a href="../LICENSE">CC BY 4.0</a>.</sub>

<sub><strong>Você com mais tempo para o que importa.</strong> #TudoProSeuCarro</sub>

</div>
