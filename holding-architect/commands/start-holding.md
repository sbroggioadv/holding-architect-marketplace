---
description: Inicia o wizard de configuracao do plugin holding-architect — cria a pasta holding/ com identidade do escritorio, area de atuacao, perfil de cliente-alvo e modo de fluxo.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [--update para reconfigurar]
---

Voce foi acionado pelo comando `/start-holding` do plugin holding-architect (Arquiteto de Holding — metodo das 4 celulas).

Argumento recebido: `$ARGUMENTS`

**Objetivo:** configurar o plugin de holding patrimonial/sucessoria ao perfil do escritorio.

## PROTOCOLO
1. **Acionar a skill `holding-onboarding`** (wizard com botoes via AskUserQuestion nas escolhas de lista fechada).
2. Cria `<cwd>/holding/perfil.md` (identidade do escritorio, area, cliente-alvo, modo).
3. Se ja existir, oferecer continuar / atualizar / recriar.

**Skill a acionar:** `holding-onboarding`.
