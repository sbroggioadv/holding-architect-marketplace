---
name: triagem-holding
description: Diagnóstico de entrada de um caso de holding — levanta patrimônio, identifica sócios (operacional × patrimonial), mapeia setor de risco e fixa o objetivo (proteção/organização, sucessão, eficiência tributária ou offshore), e grava tudo em `memoria-de-caso-holding`. Use no início de qualquer caso novo, quando o usuário disser "novo caso", "quero montar uma holding", "analisa esse patrimônio", `/diagnostico-holding`, ou quando o `holding-master` precisar dos dados antes de desenhar a estrutura. Conduz por botões (AskUserQuestion) nas escolhas fechadas.
---

# triagem-holding — diagnóstico de entrada do caso

Converte "quero uma holding" em dados estruturados que alimentam `diagnostico-estrutura` e as skills de documento. Não desenha a estrutura ainda — **coleta e classifica**. Uma decisão por vez, por botões.

## Quando ativa
Caso novo, ou quando `memoria-de-caso-holding` está vazio de dados do caso. Também sob demanda: "faz a triagem", `/diagnostico-holding`.

## Como conduzir (botões nas escolhas fechadas)
Use **AskUserQuestion** para os blocos de opção fechada, um de cada vez, com a opção mais provável marcada como recomendada. Patrimônio e nomes são digitados.

### 1. Patrimônio a estruturar (dispara `mapa-patrimonial` se for complexo)
- Tipos de bem: imóveis (quantos, valor aproximado, se geram aluguel), participações societárias, aplicações financeiras, veículos/outros.
- Valor global aproximado — define o **capital** da Cofre/ADM e a exposição a ganho de capital/ITBI.
- Origem/prova do valor (DIRPF) — base da integralização a custo histórico (**art. 23 L.9.249/95**).

### 2. Sócios — operacional × patrimonial (AskUserQuestion)
Distinção que estrutura tudo:
- **Sócio patrimonial** — detém o patrimônio (imóveis/financeiro); fica com 98% da Cofre/ADM e a Golden Share.
- **Sócio operacional** — opera as empresas de risco; fica com a Participações e os 2% da Cofre.
- **Sócio único** (acumula os dois papéis) — variação com testamento/doação com usufruto.
- **Família ampla** (vários patrimoniais) — 98% dividido; Golden Share no patriarca/matriarca.
Pergunte o **regime de bens** do sócio patrimonial (incomunicabilidade).

### 3. Setor de risco das operacionais (AskUserQuestion)
Define as vedações do objeto e se cabe camada extra:
- **Risco padrão** — estrutura de 4 células basta.
- **Alto risco** (trabalhista/ambiental/regulatório pesado) — avaliar sub-holding setorial (Participações → sub-holding → operacional).
- **Sem operacionais** (só patrimônio) — pode dispensar Participações/Gestora; foco Cofre/ADM.

### 4. Objetivo principal (AskUserQuestion — pode marcar mais de um)
- **Proteção/organização patrimonial** — segregação art. 1.024 CC (não é blindagem absoluta).
- **Sucessão** — doação de quotas com usufruto, testamento, legítima (CC 1.846/1.848).
- **Eficiência tributária** — aluguel na PJ (presumido 32%) × PF; recalcular pós-Lei 15.270.
- **Offshore** — privacidade/proteção/sucessão (não isenção — Lei 14.754/2023).

### 5. Situação de partida (AskUserQuestion)
- **Do zero** — constituir as células.
- **Já tem sociedades** — avaliar alteração/reorganização em vez de constituir.
- Sede: SP (JUCESP) ou outro estado.

## O que gravar
Persista em `memoria-de-caso-holding` (chave do **caso**): patrimônio, papéis dos sócios, regime de bens, setor de risco, objetivo(s), situação de partida, praça de registro, herdeiros necessários (dispara legítima/colação).

## Postura honesta (dizer na triagem, antes de prometer)
- Se o objetivo declarado for "blindar de credor que já existe", **alerte**: fraude contra credores / fraude à execução / desconsideração (CC 158/167/50) derrubam a estrutura montada tarde demais. Holding protege quem se organiza **antes** do passivo.
- Se o objetivo for "sacar dividendo isento", **alerte**: acabou para valor alto (Lei 15.270/2025).
- Se for offshore por "não pagar imposto", **corrija**: o gatilho de 15%/ano pega até em Delaware.

## Próximo passo
Devolva ao **`holding-master`**, que aciona `diagnostico-estrutura` para desenhar quantas células e a variação. O produto final fecha por `suprema-corte-holding`.
