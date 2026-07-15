---
name: parecer-viabilidade-holding
description: Emite o parecer consultivo de ENTRADA — "vale a pena montar holding? qual estrutura?" — cruzando patrimônio, sócios, risco e objetivo do cliente com o método das 4 células e devolvendo um veredito HONESTO (holding não é blindagem — não afasta legítima CC 1.846/1.848, fraude CC 158/167, desconsideração CC 50; dividendos não são mais isentos p/ alto valor, Lei 15.270/2025). Precifica o trade-off (economia real × custo de manutenção × substância exigida) e recomenda estrutura mínima × completa. Use quando o operador disser "vale a pena holding?", "faz sentido pro meu cliente?", "qual estrutura pra esse caso", "holding resolve?", "parecer de viabilidade", "diagnóstico de entrada", "montar holding ou não", "/parecer-holding".
---

# PARECER DE VIABILIDADE DA HOLDING

> Camada Consultivo/diferencial. O parecer de ENTRADA — antes de qualquer célula ou documento. Responde "vale a pena e qual estrutura" com honestidade, não com folclore de venda. Consome o `mapa-patrimonial`; alimenta `diagnostico-estrutura` e `holding-master`.

## Anexos obrigatórios (context/)
- `context/metodologia-4-celulas.md` — estrutura das 4 células, variações (sócio único / família ampla / alto risco), sequência, §8 checklist de adaptação.
- `context/itcmd-itbi-sucessao.md` — **§6 (LIMITES — o que a holding NÃO faz)**: legítima (CC 549/1.846/1.789), colação (CC 544/2.002), fraude contra credores (CC 158-165), fraude à execução (CPC 792 IV), desconsideração (CC 50), simulação (CC 167).
- `context/tributario-holding-2026.md` — **§6** (lícito × abusivo, propósito negocial/substância, CTN 116 §ú) + **§4** (dividendos Lei 15.270/2025) + **§5** (holding de aluguel ~11,33-14,53%).
- `context/reforma-2027-watch.md` — **§5** (decisões que envelhecem bem × mal) — sinalizar, não aplicar.

## Quando ativar
Cliente pergunta se deve montar holding; advogado precisa de parecer fundamentado de entrada; há dúvida entre estrutura mínima e completa, ou entre PF e PJ.

## O que apurar primeiro (lista fechada → use AskUserQuestion, botões)
1. **Objetivo dominante:** proteção patrimonial · sucessão / antecipação de herança · eficiência tributária (renda/aluguel) · governança familiar · internacionalização.
2. **Perfil de sócios:** sócio único · casal · família ampla · há sócio operacional (risco) separado do patrimonial?
3. **Setor de risco** das operacionais (define camadas e vedações de objeto).
4. **Há herdeiros necessários?** Doação será igual ou desigual? (dispara legítima/colação.)
> Sem esses dados, rode `mapa-patrimonial` antes.

## Metodologia do parecer
1. **Aderência ao método das 4 células:** mapear se o caso pede estrutura completa (Gestora → Cofre → Participações → ADM) ou variação (sócio único 98-100%; família ampla com 98% dividido + Golden Share no patriarca; alto risco com sub-holding setorial). Justificar cada célula pela função (guarda × renda ativa × controle × back-office).
2. **Teste dos LIMITES (itcmd-itbi §6) — antes de recomendar:**
   - **Tempestividade:** há dívida/litígio/execução preexistente? Se sim, integralizar agora pode ser **fraude contra credores (CC 158-165)** ou **fraude à execução (CPC 792, IV)** → holding não resolve, agrava. Sinalizar em vermelho.
   - **Legítima:** planejamento sucessório respeita a metade indisponível (CC 1.846/1.789)? Doação que invade a legítima é **nula no excedente (CC 549)**.
   - **Substância:** o cliente vai dar função real (contrato, contabilidade, conta própria, receita)? Sem isso é **envelope vazio → desconsideração (CC 50) / simulação (CC 167)**.
3. **Economia REAL pós-Lei 15.270 (tributario §4-§5):** se o objetivo é tributário, dizer a verdade — a conta "11% na PJ e saca isento" **morreu para alto valor** (IRRF 10% > R$ 50k/mês + IRPFM > R$ 600k/ano). A vantagem da holding de aluguel (presumido ~11,33-14,53% × PF até 27,5%) **persiste**, mas some com a saída ao sócio PF em alto volume. Delegar o número ao `comparativo-pf-pj`.
4. **Trade-off explícito:** economia/proteção esperada × custo de constituição e manutenção (4 CNPJs, contabilidade, obrigações) × substância exigida. Recomendar estrutura **mínima viável** quando o patrimônio/risco não justificar as 4 células.
5. **Forward-look (reforma-2027 §5):** o que envelhece bem (montar agora, antecipar doação enquanto ITCMD-SP é 4% fixo, integralização imune Tema 796) × o que envelhece mal (prometer "aluguel isento pra sempre", adiar sucessão apostando que nada muda).

## Estrutura do parecer (o que produzir)
- **I. Objetivo e perfil** (dados apurados). **II. Diagnóstico do patrimônio/risco/sócios.** **III. Recomendação de estrutura** (quais células, por quê, variação aplicável). **IV. Ganho esperado × custo × substância exigida.** **V. LIMITES e riscos honestos** (o que a holding não faz no caso). **VI. Forward-look 2027.** **VII. Conclusão** (vale a pena? estrutura mínima × completa? próximos passos).

## Postura honesta (inegociável)
- **Holding NÃO é blindagem** — dizer com todas as letras: não afasta legítima, fraude nem desconsideração.
- **Dividendos não são mais sempre isentos** (Lei 15.270/2025) — recalcular a economia; nunca vender a tese antiga.
- **Se o caso não justifica**, o parecer recomenda **não** montar (ou montar mínimo). Melhor perder a venda que entregar envelope vazio autuável.
- Números só via `comparativo-pf-pj`/operador — nunca inventar valor.

## Cross-link soft
Insumo → `mapa-patrimonial` · desenho da estrutura → `diagnostico-estrutura` · números → `comparativo-pf-pj` · sucessão → `planejamento-sucessorio` · offshore → `offshore-diagnostico-fiscal` · execução → `holding-master`.

## Guard
Nenhum dispositivo/alíquota sem `validador-holding` (cruzar `context/`). ITCMD-SP = **4% fixo**; art. 294 LSA = receita ≤ **R$ 78 mi**; Súmula 49 STF é a **curta**. Fecha pela `suprema-corte-holding` (R1-R4).
