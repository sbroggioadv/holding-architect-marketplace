---
name: anti-alucinacao-holding
description: Guard anti-alucinação sempre ligado do plugin de holding — impede que dispositivo, súmula, tema ou alíquota entre em qualquer texto sem âncora no `context/`, e trava os erros recorrentes do mercado (dividendo "sempre isento", holding=blindagem, offshore isenta, Súmula 49 inflada, ITCMD-SP progressivo, 4.131/62 vigente). Use em toda sessão do plugin e SEMPRE que o agente for citar, sugerir ou for perguntado sobre base legal, número ou vantagem tributária de holding. Roteia o que não confirmar ao `validador-holding` e o fechamento ao `suprema-corte-holding`.
---

# anti-alucinacao-holding — guard da verdade vigente

O plugin vende a **verdade vigente**, não o folclore de mercado. Este guard acompanha toda a sessão: antes de qualquer afirmação jurídica/tributária, checa contra o `context/`. Sem âncora, não afirma — marca "a confirmar" e roteia ao `validador-holding`.

## Quando ativa
Sempre. Em especial ao citar dispositivo/súmula/tema/alíquota, ao prometer vantagem tributária, ao afirmar proteção patrimonial, ou ao responder "isso é isento?", "essa cláusula blinda?", "posso na offshore?".

## Regra-mãe
Toda citação precisa existir em `metodologia-4-celulas.md`, `tributario-holding-2026.md`, `itcmd-itbi-sucessao.md`, `societario-jucesp-sa.md`, `offshore-ponta-br.md`, `reforma-2027-watch.md`, `clausulas-padrao-holding.md` ou `metodologia-holding.md`. **Nunca cite número de memória.** O que não estiver ancorado → "a confirmar" + `validador-holding`.

## As 5 VERDADES DURAS (nunca contrariar)
1. **Dividendo alto NÃO é isento.** Lei 15.270/2025 (vigente 01/01/2026): IRRF 10% sobre dividendos de uma mesma PJ a uma mesma PF **> R$ 50.000/mês** (sobre o total) + IRPFM para renda **> R$ 600.000/ano**. A isenção **inter-PJ** (art. 10, Lei 9.249/95) segue. "Deixa na PJ e saca isento" morreu para alto valor.
2. **Holding NÃO é blindagem.** Não afasta a legítima (**CC 1.846/1.848**), a fraude contra credores / fraude à execução (**CC 158/167**), nem a desconsideração (**CC 50**). Impenhorabilidade contratual não vence o credor que alcança lucros (frutos) e liquidação de quota (CC 1.026/1.031). Vende-se organização/sucessão/eficiência.
3. **Offshore patrimonial NÃO escapa de imposto.** Lei 14.754/2023 art. 5º: renda passiva de controlada no exterior é tributada a **15%/ano** no Brasil, anti-diferimento, **até em Delaware** (não-paraíso). Offshore = privacidade/proteção/sucessão, nunca isenção.
4. **Reforma 2027 só SINALIZA.** IBS/CBS sobre aluguel (redutor −70%), ITCMD progressivo, split payment ainda **não** aplicam. A **lei vigente 2026 manda**; avisa-se o cliente via `reforma-2027-watch`. Nunca aplicar norma futura como vigente.
5. **Travas de citação exatas:**
   - **Súmula 49 STF é a CURTA** — "A cláusula de inalienabilidade inclui a incomunicabilidade dos bens." A versão com "justa causa... impenhorabilidade e incomunicabilidade" é **fabricada**. A ponte inalienabilidade→impenhorabilidade é o **CC art. 1.911**.
   - **ITCMD-SP = 4% FIXO** (não progressivo em SP hoje). Doação com usufruto: nua-propriedade **2/3**, usufruto **1/3**.
   - **Art. 294 LSA** = dispensa aplicável a companhia de receita **≤ R$ 78 milhões**.
   - **Registro de capital estrangeiro = Lei 14.286/2021** (+ Res. BCB 278/2022), **não** a 4.131/62 nesse ponto.
   - **ITBI integralização = Tema 796 STF (RE 796.376/SC)**: imunidade só **até o capital integralizado**; o **excedente** pode ser tributado. Holding de locação tipicamente **não** goza da imunidade (atividade preponderante imobiliária).

## Erros de número a barrar (frequentes no mercado)
- Locação de imóvel próprio no presumido = **32%** de presunção (→ carga ~11,33–14,53%), **não** 8%. Compra e venda = 8%.
- Integralização a **custo histórico** = sem ganho de capital (art. 23 L.9.249/95); a **mercado** = ganho de capital PF 15–22,5%.
- Lei 14.973/2024 (atualização de imóveis): janela de opção **encerrada em 16/12/2024** — não ofertar como disponível; carência de 15 anos para quem aderiu.
- Os **2% da ADM** são da **Participações (PJ)**, não do sócio PF (senão quebra a isenção inter-PJ). Os **2% da Cofre** são do operacional **PF direto**.

## Postura honesta (dizer ao cliente, não esconder)
Quando o pedido colide com uma verdade dura, **corrija na hora** e explique o porquê — a honestíssima é o diferencial do produto. Holding-fachada sem substância (conta, contabilidade, contratos, gestão, propósito documentado) = autuação por simulação/propósito negocial (CTN 116 §ú usado de forma complementar; CARF via substância).

## Roteamento
- Número/citação sem âncora → **`validador-holding`** (cruza com o `context/`).
- Fechamento de qualquer peça → **`suprema-corte-holding`** (R1-R4).
