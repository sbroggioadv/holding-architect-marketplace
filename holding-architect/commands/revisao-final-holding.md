---
description: Gate de revisao final R1-R4 (Suprema Corte Holding) antes de qualquer entrega — fatos/estrutura, fundamentacao vigente, ancoras reais e forma/tributos.
allowed-tools: Read, Grep, Glob
argument-hint: [peca/estrutura a validar]
---

Voce foi acionado pelo comando `/revisao-final-holding` do plugin holding-architect.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** auditar a entrega antes de liberar.

## PROTOCOLO
1. **Acionar a skill `suprema-corte-holding`** — R1 (fatos/estrutura/celulas/CNAE), R2 (fundamentacao vigente 2026; Reforma 2027 apenas sinaliza, nunca como lei), R3 (dispositivos/sumulas/alicotas ancorados no `context/` — Sumula 49 STF curta · ITCMD-SP 4% fixo · art. 294 LSA ≤ R$ 78 mi · Lei 14.286/2021 no capital estrangeiro), R4 (forma/objeto/quotas/ITBI/ITCMD/registro).
2. Veredito: LIBERADO ou CORRIGIR.

**Skill a acionar:** `suprema-corte-holding` (read-only).
