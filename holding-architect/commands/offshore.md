---
description: Estrutura a camada offshore da holding — diagnostico fiscal (Lei 14.754/2023), entidade estrangeira como socia da ponta BR, registro de capital estrangeiro no BCB (Lei 14.286/2021) e regularizacao.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [objetivo offshore + patrimonio + jurisdicao]
---

Voce foi acionado pelo comando `/offshore` do plugin holding-architect.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** desenhar a ponta offshore ancorada na realidade fiscal brasileira.

## VERDADE DURA (nao vender folclore)
Offshore patrimonial de renda passiva **cai no gatilho de 15%/ano** (Lei 14.754/2023 art. 5), ate em Delaware. Offshore = privacidade/protecao/sucessao, **nunca isencao**. Foco na ponta BR ate o talo.

## PROTOCOLO
1. Consultar `context/offshore-ponta-br.md` antes.
2. **Acionar as skills da camada offshore via `holding-master`:** `offshore-diagnostico-fiscal`, `estrangeira-como-socia`, `registro-investimento-bcb` (Lei 14.286/2021 — nao a 4.131/62 revogada nesse ponto), `regularizacao-entidade-estrangeira-br`.
3. Fechar pela `suprema-corte-holding` + `validador-holding`.

**Skills a acionar:** `offshore-diagnostico-fiscal` + `estrangeira-como-socia` + `registro-investimento-bcb` + `regularizacao-entidade-estrangeira-br` (dirimidas pelo `holding-master`).
