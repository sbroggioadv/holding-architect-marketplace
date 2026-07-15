---
name: apuracao-de-haveres
description: "Trata a saida, exclusao ou falecimento de socio na holding e a apuracao dos haveres devidos: criterio de avaliacao (CC 1.031 — balanco especialmente levantado, 'salvo disposicao contratual em contrario'), procedimento de dissolucao parcial (CPC 599-609 — data da resolucao, criterio a vista do contrato, balanco de determinacao), a jurisprudencia do STJ 2025 (criterio patrimonial, fluxo de caixa descontado afastado) e a forca (e o limite) da clausula de valor contabil na holding pura x mista. Use quando o operador disser 'apuracao de haveres', 'saida de socio', 'exclusao de socio', 'falecimento de socio', 'dissolucao parcial', 'quanto vale a quota', 'balanco de determinacao', 'como calcular a quota do socio que sai', 'fluxo de caixa descontado', 'credor do socio quer a quota'."
---

# Apuracao de Haveres (saida · exclusao · falecimento)

> Quando um socio sai, e excluido ou falece, a sociedade se **resolve em relacao a ele** e paga os haveres. Na holding, a clausula de criterio bem redigida **protege o planejamento tributario da integralizacao** — mas tem limites. Esta skill calibra o criterio e instrui a dissolucao parcial.

## Anexo obrigatorio (context/)
- `context/itcmd-itbi-sucessao.md` — **§5 apuracao de haveres: CC 1.031, CPC 599/604/605/606/608, STJ 2025 (REsp 2.174.631/SP e 1.900.838/SP), holding pura x mista, CC 1.026**. `grep -niE "1.031|599|604|605|606|608|2.174.631|1.900.838|balanco|1.026"`.
- `context/clausulas-padrao-holding.md` — §5 (clausula de apuracao: valor contabil, pagamento, retencao, criterio de imoveis pela DIRPF).

## Quando ativa
- Ha saida/exclusao/morte de socio e a discussao e o valor devido ou o procedimento.
- Gatilhos: "apuracao de haveres", "saida/exclusao/falecimento de socio", "dissolucao parcial", "quanto vale a quota", "balanco de determinacao", "fluxo de caixa descontado".

## Base tecnica ancorada

### 1. Criterio de avaliacao (CC 1.031, verbatim) *(§5.1)*
> "Nos casos em que a sociedade se resolver em relacao a um socio, o valor da sua quota (...) liquidar-se-a, **salvo disposicao contratual em contrario**, com base na situacao patrimonial da sociedade, a data da resolucao, verificada em **balanco especialmente levantado**. §1º o capital social sofrera a correspondente reducao, salvo se os demais suprirem o valor. §2º a quota liquidada sera paga em dinheiro, no prazo de **90 dias**, salvo acordo ou estipulacao contratual em contrario."
- A expressao **"salvo disposicao contratual em contrario"** e o que valida a clausula de criterio da holding (valor patrimonial contabil pela DIRPF, vedada reavaliacao a mercado) — a autonomia da vontade prevalece.

### 2. Procedimento — dissolucao parcial (CPC 599-609) *(§5.2)*
> **CPC 599:** objeto = resolucao quanto ao socio falecido/excluido/retirante (I), apuracao de haveres (II) ou so uma delas (III); §1º inicial instruida com o **contrato social consolidado**; §2º cabe contra **S.A. fechada** quando acionista(s) com **5% ou mais** demonstrem que ela nao pode preencher seu fim.
> **CPC 604:** o juiz fixa a **data da resolucao**, **define o criterio de apuracao a vista do disposto no contrato social** (II) e nomeia o perito.
> **CPC 605 (data da resolucao):** falecimento = **data do obito** (I); retirada imotivada = **60º dia** da notificacao (II); recesso = recebimento da notificacao (III); retirada por justa causa e exclusao judicial = **transito em julgado** (IV); exclusao extrajudicial = **data da assembleia** (V).
> **CPC 606:** **na omissao do contrato**, o juiz adota o **valor patrimonial apurado em balanco de determinacao**, avaliando ativos tangiveis e intangiveis a **preco de saida**.
> **CPC 608:** lucros/JCP/remuneracao integram os haveres **ate** a data da resolucao; depois, so correcao monetaria + juros.

### 3. Jurisprudencia STJ 2025 *(§5.3)*
- **REsp 2.174.631/SP** (3ª T., Rel. Min. Moura Ribeiro, j. 17/03/2025): fundo de comercio/aviamento/goodwill e elemento do **balanco de determinacao**; **incabivel o fluxo de caixa descontado (FCD)** — usa-se o **criterio patrimonial** (CPC 606 / CC 1.031).
- **REsp 1.900.838/SP** (Rel. Min. Humberto Martins, j. 28/04/2025): na **omissao do contrato**, a quota e avaliada pelo **criterio patrimonial mediante balanco de determinacao**; afastar o FCD **nao contraria** a jurisprudencia (Sum. 83/STJ).
> Sintese: criterio **patrimonial** (balanco de determinacao, preco de saida, com intangiveis) e o padrao **na omissao**; o **FCD** e em regra **afastado**. Clausula contratual clara **prevalece** (CC 1.031), mas pode ser **revista** se conduzir a valor manifestamente aviltante (CC 884/187 — enriquecimento sem causa, abuso de direito).

### 4. Na holding — pura x mista *(§5.4)*
- **Holding patrimonial pura:** o valor concentra-se na reavaliacao dos ativos (imoveis, participacoes, aplicacoes) menos passivo; **goodwill autonomo tende a ser marginal/inexistente** (sem clientela/marca/atividade operacional). Por isso a **clausula de valor contabil e mais segura** aqui — nao ha goodwill a discutir e a previsibilidade protege a integralizacao pela DIRPF.
- **Holding mista/operacional** (ADM de Bens com gestao ativa): o risco de revisao **sobe** — reforcar a clausula com **racional/justa causa declarada**.
- **CC 1.026:** o credor particular do socio pode, na insuficiencia de outros bens, fazer a execucao recair sobre os **lucros** e requerer a **liquidacao da quota** (apurada na forma do 1.031). E o lastro — e o limite — da clausula de "frutos civis".

## O que produzir
1. **Enquadrar o evento** (saida voluntaria/exclusao/falecimento) e a **data da resolucao** (CPC 605).
2. **Redigir/auditar a clausula de apuracao** (§5 do anexo de clausulas): balanco de determinacao por contador independente, **valor patrimonial contabil como criterio EXCLUSIVO** (CC 1.031), afastada reavaliacao a mercado/FCD, imoveis pelo **valor da DIRPF** do integralizador (§3º critico), pagamento parcelado (ex.: 24x IPCA+6% a.a.), retencao para contingencias.
3. Se contencioso: **acao de dissolucao parcial** (CPC 599) instruida com o contrato consolidado; requerer a fixacao da data e do criterio; sinalizar a orientacao STJ 2025.
4. Alertar sobre o **teste de aviltamento**: em holding com ativo quase todo imobiliario e mercado muito acima do contabil, a clausula pode ser atacada — reforcar racional.

## Postura honesta
- A clausula de valor contabil **organiza e protege**, mas **nao e absoluta**: pode ser revista se aviltante (CC 884/187) e o credor alcanca lucros + liquidacao (CC 1.026).
- Na **omissao** do contrato, o juiz vai ao **criterio patrimonial/balanco de determinacao** (CPC 606 + STJ) — nao ao valor contabil historico; por isso a **clausula expressa** e o que trava o criterio favoravel.

## Cross-link
`contrato-social-holding`/`acordo-de-socios` (redacao da clausula) · `celula-adm-de-bens`/`celula-empresa-cofre` (pura x mista) · `planejamento-sucessorio` (falecimento) · plugins `civel-adv-os` (dissolucao parcial) e `calculosjudiciais-adv-os` (memoria de calculo dos haveres).

## Guard
CC 1.031 "salvo disposicao contratual" valida a clausula; FCD em regra afastado (STJ 2025). Data da resolucao pelo CPC 605. Clausula contabil pode cair se aviltante (CC 884/187). REsp so com numero/data conferidos — nenhum dado sem `validador-holding`. Entrega fecha pela `suprema-corte-holding`.
