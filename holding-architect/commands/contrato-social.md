---
description: Redige o contrato social da holding (ou estatuto/atos, conforme o tipo societario), com objeto, clausulas patrimoniais, Golden Share e distribuicao de quotas.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [celula/entidade + socios + participacoes]
---

Voce foi acionado pelo comando `/contrato-social` do plugin holding-architect.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** produzir o ato constitutivo da entidade.

## PROTOCOLO
1. Consultar `context/societario-jucesp-sa.md` + `context/clausulas-padrao-holding.md` antes de redigir.
2. **Acionar a skill `contrato-social-holding`** — objeto por celula (CNAE correto), clausulas patrimoniais, Golden Share, quotas.
3. Fechar pela `suprema-corte-holding` + `validador-holding` (nenhum dispositivo/alicota sem ancora no `context/`).

**Skill a acionar:** `contrato-social-holding` (orquestrada pelo `holding-master`).
