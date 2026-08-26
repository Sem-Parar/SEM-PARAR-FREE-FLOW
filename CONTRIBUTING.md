# Como contribuir

Este repositório é mantido pelo Sem Parar e existe porque a informação sobre Free Flow no Brasil está espalhada e muda rápido. **Toda correção é bem-vinda**, inclusive as pequenas: um km errado, um link que quebrou, um pórtico que inaugurou ontem.

## A regra que vale para tudo: fonte oficial

Toda contribuição precisa vir acompanhada de uma **fonte oficial**, seja a ANTT, uma agência reguladora estadual (ARTESP, AGERGS, DER-MG e congêneres) ou o site da própria concessionária. Notícia de imprensa serve como sinal para investigarmos, mas o dado só entra com confirmação oficial.

Se a fonte oficial ainda não publicou, avise assim mesmo. Registramos como pendência e acompanhamos.

## O jeito mais rápido: abrir uma issue

Você não precisa saber Git. [Abra uma issue](../../issues/new) dizendo o que está errado ou o que mudou, e cole o link da fonte oficial. Serve para pórtico novo, inauguração, adiamento, km errado, concessionária errada, link quebrado ou canal suspeito.

## Se preferir mandar um pull request

1. Faça um fork e crie um branch descritivo, por exemplo `dados/portico-br101-km600`.
2. Edite **o CSV**, nunca só o JSON. Os arquivos em `dados/json/` são gerados a partir dos CSVs.
3. Atualize a coluna `atualizado_em` da linha que você mexeu, no formato `AAAA-MM-DD`, e preencha a coluna `fonte` com a URL oficial.
4. Some uma linha ao [CHANGELOG.md](CHANGELOG.md), na seção `[Não publicado]`.
5. Abra o PR explicando o que mudou e por quê.

Não é preciso regenerar os JSONs. A manutenção faz isso na revisão.

## Convenções das bases

**Nada de valores.** Não registramos tarifa em reais nem percentual de desconto, porque eles mudam com frequência e envelhecem mal. Registramos o link da tabela tarifária oficial, que fica sempre atualizada na origem.

**`n/d` em vez de chute.** Campo não confirmado é `n/d`. Nenhum dado deste repositório pode ser inferido, deduzido ou preenchido por analogia.

**Divergência se registra, não se resolve no escuro.** Quando ANTT e concessionária publicam quilometragens diferentes para o mesmo pórtico, adotamos o valor da ANTT e anotamos a divergência no campo de trecho.

**Pórtico de monitoramento não é pórtico de cobrança.** Estruturas que só monitoram tráfego não entram na contagem de `n_porticos`. Mencione-as no campo de trecho.

**Datas em ISO** (`AAAA-MM-DD`), sempre.

**Separador de listas dentro de célula:** ponto e vírgula.

O significado de cada coluna está em [`dados/README.md`](dados/README.md).

## Ritmo de atualização

| Evento | Prazo |
|---|---|
| Inauguração, adiamento ou mudança de status | até 72 horas após o fato confirmado |
| Revisão completa das bases | mensal |
| Revisão editorial dos textos | trimestral |

## O que não entra

- Valores de tarifa, mensalidade ou percentual de desconto.
- Dados sem fonte oficial verificável.
- Links de canais não oficiais de pagamento apresentados como oficiais.
- Conteúdo promocional de terceiros.

## Achou um golpe?

Se você encontrou um site, app ou mensagem se passando por canal oficial de pagamento de pedágio, [abra uma issue](../../issues/new) com o endereço e, se possível, uma captura de tela. Quanto mais rápido a lista verificada em [`dados/canais-oficiais-pagamento.csv`](dados/canais-oficiais-pagamento.csv) refletir a realidade, menos gente cai.

**Nunca inclua dados pessoais**, como placa, CPF, número de cartão ou print de fatura. Este repositório é público.

## Código de conduta

Ao participar, você concorda com o [Código de Conduta](CODE_OF_CONDUCT.md).
