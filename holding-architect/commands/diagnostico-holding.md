---
description: Diagnostico inicial da holding — classifica o caso, mapeia o patrimonio e desenha quantas celulas e qual variacao de estrutura o cliente precisa.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [perfil do cliente + patrimonio + objetivo]
---

Voce foi acionado pelo comando `/diagnostico-holding` do plugin holding-architect.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** entender o caso antes de estruturar.

## PROTOCOLO
1. **Acionar a skill `triagem-holding`** (botoes) — fixa patrimonio, socios (operacional × patrimonial), setor de risco e objetivo.
2. **Acionar a skill `mapa-patrimonial`** — inventaria imoveis, participacoes, aplicacoes e a titularidade atual.
3. **Acionar a skill `diagnostico-estrutura`** — decide quantas celulas e a variacao (socio unico / familia ampla / alto risco com sub-holding).
4. Encaminhar ao `holding-master` para conduzir a montagem.

**Skills a acionar:** `triagem-holding` + `mapa-patrimonial` + `diagnostico-estrutura` (orquestradas pelo `holding-master`).
