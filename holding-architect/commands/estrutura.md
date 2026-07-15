---
description: Desenha a estrutura da holding pelo metodo das 4 celulas (Cofre · ADM de Bens · Participacoes · Gestora), na sequencia de producao correta por dependencia de CNPJ.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [caso ja diagnosticado]
---

Voce foi acionado pelo comando `/estrutura` do plugin holding-architect.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** montar a arquitetura das celulas.

## PROTOCOLO
1. `diagnostico-estrutura` define quantas celulas e a variacao antes de desenhar.
2. **Acionar as skills das 4 celulas via `holding-master`:** `celula-empresa-cofre`, `celula-adm-de-bens`, `celula-holding-participacoes`, `celula-gestora-pagamentos`.
3. `sequencia-de-producao` orquestra a ordem (Gestora → Cofre → Participacoes → ADM — dependencia de CNPJ).
4. Fechar pela `suprema-corte-holding`.

**Skills a acionar:** `celula-empresa-cofre` + `celula-adm-de-bens` + `celula-holding-participacoes` + `celula-gestora-pagamentos` (dirimidas pelo `holding-master`).
