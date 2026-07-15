---
name: mapa-patrimonial
description: Levanta e organiza o INVENTÁRIO do patrimônio e dos sócios a estruturar — imóveis (matrícula, valor DIRPF × mercado, situação registral e ITBI), participações societárias, aplicações, veículos; papéis (sócio patrimonial × operacional), regime de bens, herdeiros necessários e setor de risco. É o INSUMO estruturado que alimenta as demais skills (diagnóstico, células, integralização, sucessão, comparativo). Use quando o operador disser "levanta o patrimônio", "mapa patrimonial", "o que o cliente tem pra colocar na holding", "inventário de bens do cliente", "organiza os ativos", "quais imóveis integralizar", "levantamento patrimonial", "/mapa-patrimonial".
---

# MAPA PATRIMONIAL

> Camada Consultivo/diferencial. O levantamento estruturado que TODA holding precisa antes de desenhar célula ou redigir documento. Sem mapa, o diagnóstico chuta. É insumo, não peça: organiza os dados brutos do caso num formato reutilizável.

## Anexos obrigatórios (context/)
- `context/metodologia-4-celulas.md` — **§8** (checklist de adaptação para novo caso) + §1-§2 (papéis sócio patrimonial × operacional; qual patrimônio vai à Cofre × ADM).
- `context/itcmd-itbi-sucessao.md` — **§1** (imóveis: matrícula, continuidade registral LRP 195/237, valor DIRPF × mercado, ITBI Tema 796) + **§4.2** (herdeiros necessários/legítima — dado que muda a sucessão).
- `context/tributario-holding-2026.md` — **§1** (custo histórico × valor de mercado — capturar os dois para cada bem).

## Quando ativar
Início de qualquer caso de holding; antes de `parecer-viabilidade-holding`, `diagnostico-estrutura`, `comparativo-pf-pj`; quando o operador tem os documentos do cliente e precisa organizá-los.

## O que levantar (checklist estruturado — metodologia §8)
**A. Sócios e papéis:**
- Quem é o **sócio patrimonial** (detém o patrimônio) × quem é o **sócio operacional** (opera empresas de risco). Podem ser a mesma pessoa (sócio único).
- Estado civil e **regime de bens** (define incomunicabilidade / anuência conjugal).
- **Herdeiros necessários** (descendentes, ascendentes, cônjuge — CC 1.845)? Quantos? Doação pretendida **igual ou desigual**? (dispara legítima/colação — `doacao-quotas-usufruto`.)

**B. Imóveis (o núcleo — usar tabela):**
| Imóvel | Matrícula/CRI | Titular atual | Valor DIRPF | Valor de mercado | Gera aluguel? | Destino (Cofre/ADM) |
|---|---|---|---|---|---|---|
- Anotar **valor DIRPF (custo histórico)** E **valor de mercado** de cada um (base do trade-off integralização — tributario §1).
- **Situação registral:** o titular consta como proprietário na matrícula (continuidade, LRP 195/237)? Há ônus/gravame/financiamento?
- **Gera renda ativa (aluguel)?** → candidato à **ADM de Bens**. Guarda pura, sem renda → **Cofre**.

**C. Participações societárias:** empresas operacionais (setor/risco), % detido, quem controla → definem a **Holding de Participações** e eventuais sub-holdings.

**D. Aplicações financeiras, veículos e outros ativos** relevantes.

**E. Setor de risco** das operacionais (define vedações de objeto e nº de camadas).

**F. Passivos e contingências:** há **dívida, execução ou litígio preexistente**? (crítico — dispara alerta de fraude contra credores/à execução no `parecer-viabilidade-holding`; integralizar sobre dívida preexistente é anulável).

**G. Ativos no exterior?** → aciona a camada offshore (`offshore-diagnostico-fiscal`) e o ITCMD forward-look (EC 132 art. 16).

## Como conduzir
- Perguntas de **lista fechada** (papel do sócio, regime de bens, doação igual/desigual, sede SP × outro estado) → usar **AskUserQuestion** (botões).
- Dados abertos (matrículas, valores) → pedir os documentos; **nunca inventar valor ou número de matrícula**.
- Consolidar tudo num **mapa reutilizável** que as demais skills consomem (e o `memoria-de-caso-holding` guarda).

## O que produzir
1. **Quadro de sócios e papéis** (patrimonial × operacional, regime de bens, herdeiros).
2. **Tabela de imóveis** (matrícula · DIRPF · mercado · aluguel? · destino Cofre/ADM · situação registral).
3. **Lista de participações e demais ativos.**
4. **Bandeiras de risco** (passivo/litígio preexistente; ativos no exterior; herdeiros/legítima; imóvel sem continuidade registral).
5. **Encaminhamentos:** o que alimenta o diagnóstico de estrutura, o comparativo PF×PJ e a integralização.

## Postura honesta
- O mapa **só registra o que o operador informa** — dado faltante fica marcado "a obter", não estimado.
- **Sinalizar cedo** o passivo/litígio preexistente: é o que pode inviabilizar a holding (fraude) antes de qualquer economia.
- Valor de mercado sem laudo é premissa, não fato — marcar como tal.

## Cross-link soft
Parecer de entrada → `parecer-viabilidade-holding` · desenho da estrutura → `diagnostico-estrutura` · números → `comparativo-pf-pj` · integralização → `integralizacao-de-imoveis` / `itbi-integralizacao` · estado do caso → `memoria-de-caso-holding` · sucessão → `planejamento-sucessorio`.

## Guard
Nenhum valor/matrícula/dado inventado. Dispositivos (LRP, CC herdeiros, Tema 796) só via `validador-holding`. Fecha (quando vira insumo de peça) pela `suprema-corte-holding` (R1-R4).
