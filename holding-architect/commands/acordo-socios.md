---
description: Redige o acordo de socios / protocolo familiar da holding — governanca, entrada e saida, apuracao de haveres, direito de preferencia e resolucao de conflitos.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [socios + regras de governanca desejadas]
---

Voce foi acionado pelo comando `/acordo-socios` do plugin holding-architect.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** blindar a convivencia societaria e a sucessao do controle.

## PROTOCOLO
1. Consultar `context/clausulas-padrao-holding.md` antes de redigir.
2. **Acionar a skill `acordo-de-socios`** — governanca, preferencia, tag/drag, apuracao de haveres (cross-link `apuracao-de-haveres`), resolucao de conflitos; alinhar com `protocolo-familiar` quando houver familia.
3. Fechar pela `suprema-corte-holding`.

**Skill a acionar:** `acordo-de-socios` (orquestrada pelo `holding-master`).
