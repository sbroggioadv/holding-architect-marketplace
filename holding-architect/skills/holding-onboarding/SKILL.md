---
name: holding-onboarding
description: Configura o perfil do escritório do usuário na primeira sessão do plugin (nome/marca, OAB, foro, estilo de peça, praça de registro predominante) e grava em `memoria-de-caso-holding`. Use quando o usuário digitar `/start-holding`, na primeira vez que abrir o plugin, quando disser "configurar meu escritório", "onboarding", "começar do zero", ou quando o `holding-master` detectar que o escritório ainda não foi configurado. Conduz por botões (AskUserQuestion), nunca por texto aberto em escolha fechada.
---

# holding-onboarding — configuração do escritório

Primeira porta do plugin. O produto é **despersonalizado** (autoria IA Combativa, método das 4 células); o escritório de **quem usa** é configurado aqui, uma vez, e reaproveitado em todas as peças. Nada de dado de cliente vive no plugin — só o perfil do operador.

## Quando ativa
`/start-holding`, primeira sessão, "configurar escritório", ou disparo do `holding-master` quando o perfil está vazio.

## Como conduzir (regra de ouro: botões)
Toda pergunta de escolha fechada usa **AskUserQuestion** (botões clicáveis), uma decisão por vez, com uma opção recomendada marcada. Campos livres (nome, número da OAB, cidade) são digitados. Nunca despeje um formulário gigante — pergunte em blocos curtos.

### Bloco 1 — Identidade do escritório (campos livres)
- Nome/marca do escritório ou do advogado (como assina a peça).
- Número da OAB e seccional (para o rodapé/assinatura das peças).
- Cidade/UF da sede.

### Bloco 2 — Praça de registro predominante (AskUserQuestion)
Onde a maioria das holdings será registrada?
- **JUCESP (São Paulo)** — recomendado se a sede é SP; o `context/` está calibrado para a JUCESP.
- **Outra junta comercial** — o método é o mesmo; confirmar exigências locais na junta.
- **Misto / a definir por caso** — decide na `triagem-holding`.

### Bloco 3 — Estilo de peça (AskUserQuestion)
- **Enxuto e objetivo** — cláusulas diretas, sem prolixidade (recomendado; alinha com a JUCESP).
- **Detalhado e fundamentado** — mais notas de fundamento no corpo.

### Bloco 4 — Postura sobre a Reforma 2027 (AskUserQuestion)
- **Sinalizar sempre** — toda peça/parecer traz um aviso forward-look sobre IBS/CBS, ITCMD progressivo e split payment (recomendado — transparência).
- **Só quando eu pedir** — mantém o foco na lei vigente 2026.

## O que gravar
Persista em `memoria-de-caso-holding` sob a chave do **perfil do escritório** (não do caso): nome/marca, OAB+seccional, cidade/UF, praça de registro, estilo de peça, postura Reforma 2027. Marque `perfil_configurado: sim`.

## Postura honesta (dizer no fecho do onboarding)
- O plugin entrega o **método** (as 4 células, cláusulas, sequência, tributário/sucessório vigente) — a **responsabilidade técnica e a adaptação ao caso concreto são do advogado**.
- O plugin **não** vende blindagem absoluta nem promessa de isenção: holding é organização/sucessão/eficiência com fundamento (ver `anti-alucinacao-holding`).
- Lei vigente 2026 é a autoritativa; a Reforma 2027 só sinaliza.

## Próximo passo
Ao concluir, devolva o controle ao **`holding-master`** e ofereça iniciar um caso pela **`triagem-holding`**. Peças produzidas depois continuam fechando por `suprema-corte-holding`.
