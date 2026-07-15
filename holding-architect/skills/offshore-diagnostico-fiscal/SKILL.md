---
name: offshore-diagnostico-fiscal
description: Panorama fiscal comparativo de jurisdições offshore para holding patrimonial (Delaware a fundo + Wyoming/Paraguai/Uruguai/Dubai) e a VERDADE da Lei 14.754/2023 art. 5º — o gatilho de 15%/ano acabou com o diferimento, até em Delaware. Offshore = privacidade, proteção e sucessão, NÃO isenção de imposto. Diagnóstico de alto nível para o cliente decidir ONDE abrir; a execução lá fora é parceiro in loco. Use quando o operador disser "vale a pena abrir offshore", "qual país pra offshore", "Delaware ou Dubai", "LLC pra holding", "não pago imposto se for offshore?", "quero blindar no exterior", "planejamento internacional", "/offshore diagnostico".
---

# OFFSHORE — DIAGNÓSTICO FISCAL COMPARATIVO

> Camada 5 (Offshore — ponta BR). Diagnóstico consultivo de alto nível: dá ao cliente o mapa das jurisdições para ELE decidir onde abrir. Não é peça — é orientação honesta antes de qualquer estrutura.

## Anexos obrigatórios (context/)
- `context/offshore-ponta-br.md` — **§6** (panorama comparativo de jurisdições + quadro-resumo status RFB) e **§6.7 / §3** (casamento com a Lei 14.754/2023, entidade controlada, gatilho, renda ativa < 60%). `grep -n "DELAWARE\|renda ativa\|14.754\|IN 1.037\|regime favorecido" context/offshore-ponta-br.md`.
- `context/tributario-holding-2026.md` — **§3** (Lei 14.754 resumo, anti-diferimento, trust transparente).
- `context/reforma-2027-watch.md` — **§3** (EC 132 art. 16: ITCMD passa a alcançar bem/doador no exterior — sinalizar, não aplicar como certo).

## Limite de escopo — declarar SEMPRE ao cliente
O plugin **não abre** a entidade lá fora (constituição da LLC em Delaware, FZ-LLC em Dubai, S.A. no Paraguai) — isso é **parceiro in loco**. O plugin domina a **ponta brasileira**: apostila → tradução → CNPJ da estrangeira → registro BCB → entrada como sócia da holding BR (skills `regularizacao-entidade-estrangeira-br`, `registro-investimento-bcb`, `estrangeira-como-socia`). O panorama fiscal estrangeiro abaixo é **comparativo de alto nível**; a execução tributária lá fora é do parceiro. A **lei brasileira vigente é a autoritativa** sobre o beneficiário residente no Brasil.

## Quando ativar
Cliente cogita estrutura no exterior; pergunta "qual país", "vale a pena", "não pago imposto?"; quer privacidade/proteção/moeda forte; ou tem ativos no exterior a organizar.

## A VERDADE — Lei 14.754/2023 (âncora inegociável)
- **Entidade controlada (art. 5º, §1º):** a PF que tem preponderância nas deliberações **ou** > 50% do capital/lucros/ativos controla a offshore. Uma LLC de Delaware de brasileiro **é** entidade controlada — pouco importa que seja *disregarded entity* nos EUA.
- **Gatilho da tributação automática em 31/12 (art. 5º, §5º):** cai no regime a controlada que (I) esteja em **tributação favorecida / regime fiscal privilegiado** (arts. 24/24-A da Lei 9.430/96) **ou** (II) apure **renda ativa própria < 60% da renda total**.
- **Renda ativa própria (art. 5º, §6º, I):** exclui royalties, juros, **dividendos, participações societárias**, aluguéis, ganhos de capital, aplicações financeiras. **Holding patrimonial offshore que só detém participações e recebe dividendos tem renda essencialmente passiva → renda ativa < 60% → lucro tributado a 15% em 31/12, mesmo sem distribuir. O diferimento acabou — vale até em Delaware (não-paraíso).**
- Crédito do IR pago no exterior compensável (art. 4º — tratado ou reciprocidade; EUA têm reciprocidade). Trust é **transparente** (arts. 10-13): bens do instituidor/beneficiário, tributados a 15%.

## Panorama comparativo (context/offshore-ponta-br §6 — cliente decide, parceiro executa)
| Jurisdição | Trib. local típica | Favorecido p/ Brasil (IN 1.037/2010)? | Gatilho Lei 14.754 provável |
|---|---|---|---|
| **Delaware (EUA)** ⭐ | 0% estadual (LLC); flat US$ 300/ano; ~21% fed. se Corp | **Não listado** | Cai por **renda ativa < 60%** (holding passiva) |
| Wyoming (EUA) | 0% estadual; privacidade agressiva | Não listado | Idem Delaware |
| Paraguai | IRE 10% + IDU 10% | Não listado | Cai por renda ativa < 60% se passiva |
| Uruguai | IRAE 25% (ou 0% zona franca) | Regimes especiais listados | Zona franca → favorecido; S.A. comum → renda ativa < 60% |
| Dubai/EAU | 9% (0% qualifying) | **Listado (favorecido)** | **Favorecido + passiva → tributação automática certa** |

- **Delaware (foco):** LLC flexível (Operating Agreement livre), alta privacidade (membros não constam do registro público), barata; EUA **não** constam da IN 1.037/2010 → não é "paraíso" para o Brasil (fundamentação mais defensável). Ainda assim, holding passiva cai pelo teste de renda ativa < 60%.
- **Dubai:** EAU **constam** da lista de tributação favorecida → Free Zone + renda passiva = tributação automática certa a 15%, sem diferimento — pior fundamentação, não melhor economia.

## O que produzir
1. **Escolher o objetivo real** com o cliente (lista fechada → use **AskUserQuestion**, botões): privacidade · proteção patrimonial · moeda forte / acesso a mercados · planejamento sucessório · (nunca "não pagar imposto").
2. **Mapear o perfil da futura entidade:** vai só deter participações/receber dividendos (passiva → gatilho certo) ou terá atividade econômica própria > 40% (chance de escapar do §5º, II)?
3. **Casar com a Lei 14.754:** apontar que o beneficiário residente paga 15%/ano no Brasil independentemente da jurisdição; a escolha muda **fundamentação e risco de autuação**, não a regra de 15%.
4. **Sinalizar o ITCMD forward-look:** EC 132 art. 16 autoriza estados a cobrar ITCMD sobre doação de doador no exterior e herança de bens no exterior — offshore passa a poder gerar ITCMD na sucessão (`reforma-2027-watch`; não vender como certo — depende de lei estadual/LC).
5. **Devolver um quadro de decisão** (jurisdição × custo × privacidade × fundamentação fiscal × gatilho), com a recomendação e o encaminhamento à ponta BR.

## Postura honesta (repetir ao cliente)
- **Offshore NÃO escapa de imposto.** A Lei 14.754 fechou o diferimento sobre lucro acumulado — 15% anual incide **mesmo sem distribuir, mesmo em Delaware**. A offshore continua útil por **privacidade, proteção, moeda forte, acesso a mercados e sucessão** — nunca por economia de imposto por acúmulo.
- **A tabela de custos é estimativa de mercado, não norma.** Números de setup/manutenção não entram em peça como definitivos.
- **Holding (aqui ou lá) NÃO é blindagem** — não vence fraude, simulação nem desconsideração.

## Cross-link soft
Regularização da entrada no Brasil → `regularizacao-entidade-estrangeira-br` · registro do capital → `registro-investimento-bcb` · entrada no quadro → `estrangeira-como-socia` · impacto sucessório → `planejamento-sucessorio`. Planejamento tributário/internacional aprofundado → `tributario-societario-adv-os`.

## Guard
Nenhuma alíquota/dispositivo/lista sem `validador-holding` (cruzar com `context/offshore-ponta-br.md` e `tributario-holding-2026.md`). Nunca prometer isenção. Registro de capital estrangeiro = **Lei 14.286/2021**, não a 4.131/62. Fecha pela `suprema-corte-holding` (R1-R4).
