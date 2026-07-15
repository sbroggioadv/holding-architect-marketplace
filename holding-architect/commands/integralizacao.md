---
description: Estrutura a integralizacao de imoveis no capital da holding e trata a imunidade/incidencia de ITBI (Tema 796 STF), com a ponta patrimonial e o valor de integralizacao.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [imoveis + valores + entidade]
---

Voce foi acionado pelo comando `/integralizacao` do plugin holding-architect.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** integralizar bens na holding e resolver o ITBI.

## PROTOCOLO
1. **Acionar a skill `integralizacao-de-imoveis`** — define o que entra, por qual valor (custo × mercado) e o reflexo de ganho de capital.
2. **Acionar a skill `itbi-integralizacao`** — imunidade art. 156 §2 I CF + Tema 796 STF (excesso sobre o capital); atividade preponderante imobiliaria.
3. Fronteira: o registral fino e cross-link com `direito-imobiliario` — aqui trata a ponta patrimonial da holding.
4. Fechar pela `suprema-corte-holding`.

**Skills a acionar:** `integralizacao-de-imoveis` + `itbi-integralizacao` (orquestradas pelo `holding-master`).
