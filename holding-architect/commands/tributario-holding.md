---
description: Planejamento tributario da holding e comparativo PF × PJ — regime da entidade, tributacao de aluguel/dividendos (Lei 15.270/2025) e a saida fiscal mais eficiente com a verdade vigente 2026.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [receitas + patrimonio + objetivo fiscal]
---

Voce foi acionado pelo comando `/tributario-holding` do plugin holding-architect.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** achar a estrutura fiscal mais eficiente sem mentir pro cliente.

## VERDADE DURA
Dividendos **nao sao mais isentos para alto valor** — Lei 15.270/2025 (IRRF 10% acima de R$ 50k/mes + IRPFM). A tese "deixa na PJ e saca isento" morreu para alto valor.

## PROTOCOLO
1. Consultar `context/tributario-holding-2026.md` + `context/reforma-2027-watch.md` antes.
2. **Acionar a skill `planejamento-tributario-holding`** — regime (Presumido × Real), aluguel, dividendos, holding pura × mista.
3. **Acionar a skill `comparativo-pf-pj`** — numeros lado a lado (imovel na PF × na PJ), com premissas explicitas.
4. Forward-look Reforma 2027 (IBS/CBS sobre locacao, redutores, split payment) — sinaliza, nao aplica como vigente.
5. Fechar pela `suprema-corte-holding` + `validador-holding`.

**Skills a acionar:** `planejamento-tributario-holding` + `comparativo-pf-pj` (orquestradas pelo `holding-master`).
