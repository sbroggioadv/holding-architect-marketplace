---
name: base-tributaria-2026
description: Fundação tributária da holding pela lei VIGENTE em 2026 — integralização de bens (custo × mercado), dividendos pós-Lei 15.270/2025, Lei 14.973/2024, lucro presumido 32% na locação e os limites do planejamento (propósito negocial). Use ao calcular carga da holding, comparar PF × PJ, decidir valor de integralização, avaliar distribuição de lucros/dividendos, ou quando o cliente disser "deixo na PJ e saco isento" / "aluguel na holding paga quanto?" / "vale a pena passar os imóveis pra empresa?".
---

# Base Tributária da Holding — Lei Vigente 2026

## 1. Quando ativa
Sempre que houver conta tributária: integralização de bens, dividendos/distribuição de lucros, carga da locação, PF × PJ, limites do planejamento. Lei **vigente de 2026 manda**; a Reforma 2027 só sinaliza (→ `reforma-2027-watch`). Alimenta `planejamento-tributario-holding`, `comparativo-pf-pj`, `integralizacao-de-imoveis`.

## 2. Base legal ancorada (`tributario-holding-2026.md`)

**Integralização — art. 23 Lei 9.249/95:** a PF transfere bens à PJ a **custo histórico (valor da DIRPF)** OU a **valor de mercado**, à sua opção.
- Custo histórico → **zero imposto na entrada** (difere o ganho) = rota padrão da holding.
- Mercado → diferença (mercado − custo) é **ganho de capital na PF** (art. 23, §1º), alíquotas progressivas do **art. 21 Lei 8.981/95 (red. Lei 13.259/2016): 15% até R$ 5 mi · 17,5% até R$ 10 mi · 20% até R$ 30 mi · 22,5% acima**.
- ITBI na integralização: imunidade CF 156 §2º I, **exceto atividade preponderante imobiliária** (holding de locação normalmente não goza) e **Tema 796 STF** (imune só até o capital integralizado; excedente tributa) → detalhe em `itbi-integralizacao`.

**Lei 14.973/2024 — atualização de imóvel a mercado (JANELA ENCERRADA 16/12/2024):** RAB-PF **4%** · RAB-PJ **6% IRPJ + 4% CSLL = 10%**. Carência do **art. 8º: 15 anos** — vender antes de 3 anos = dupla tributação; benefício só amadurece 100% em 180 meses. Em 2026 vale como **referência histórica** (quem aderiu carrega a carência).

**Dividendos — Lei 15.270/2025 (vigente 01/01/2026), a maior mudança:**
1. **IRRF 10%** sobre dividendos de uma mesma PJ a uma mesma PF residente **> R$ 50.000/mês** (sobre o total, sem dedução — art. 6º-A). **Não** incide na distribuição **PJ→PJ** (art. 10 Lei 9.249 intacto inter-PJ).
2. **IRPFM** (mínimo) para renda total **> R$ 600.000/ano** — cresce de 0% a 10% entre R$ 600 mil e R$ 1,2 mi; 10% acima (art. 16-A).
3. **Redutor anti-bitributação** se IRPJ+CSLL efetivo + IRPFM ultrapassar o teto (34/40/45%).
4. **10% IRRF** sobre dividendos ao exterior (§4º art. 10).
5. **Transição:** lucros aprovados/acumulados **até 31/12/2025** ficam isentos se distribuídos conforme o ato até **2028** → janela para deliberar lucros antigos.

**Lucro presumido — locação de imóveis próprios:** presunção **32%** (não 8%). Carga efetiva ≈ **11,33%** (IRPJ 4,80 + CSLL 2,88 + PIS 0,65 + COFINS 3,00), subindo até **≈ 14,53%** com o adicional de IRPJ 10% (lucro presumido > R$ 20 mil/mês). Compra e venda de imóveis = presunção **8%**. Locação **não** pode Simples. Limite do presumido: receita ≤ R$ 78 mi/ano. Objeto social deve trazer **locação de imóveis próprios expressa**.

**Limites — art. 116, §ú, CTN (norma antielisiva, LC 104/2001):** em vigor, mas **nunca regulamentado** federalmente → sozinho não embasa autuação (corrente majoritária). RFB/CARF desconsideram por **simulação (CTN 149, VII) + propósito negocial + substância sobre forma**.

## 3. O que produzir
- Cálculo com a lei de hoje, **somando a saída** (dividendo pós-15.270) — nunca só a carga na PJ.
- Escolha de valor de integralização (custo × mercado) com o trade-off ITBI × ganho de capital explícito.
- Regra de ouro do produto: a holding tem que **fazer algo** (administrar, contratar, ter contabilidade e fluxo real) e ter **propósito documentado** — sem isso é envelope vazio = autuação.

## 4. Postura honesta (verdades duras)
- **VERDADE #1 — dividendo não é mais 100% isento p/ valor alto** (Lei 15.270/2025). A tese "deixa na PJ e saca isento" **morreu** para alto valor. Planejamento lícito: distribuir ≤ R$ 50k/mês por PJ/sócio evita o IRRF mensal, **mas** o IRPFM anual captura quem passa de R$ 600 mil/ano somando tudo.
- Migrar locação para a holding no presumido derruba a carga de até 27,5% (PF) para ~11,33–14,53% — **ainda vantajoso**, mas some o dividendo na saída e sinalize o IBS/CBS futuro (`reforma-2027-watch`).
- **Riscos:** distribuição desproporcional sem causa → doação disfarçada/ITCMD; confusão patrimonial → desconsideração (CC 50); pejotização → requalificação. Regulamentação infralegal do IRRF/IRPFM **ainda em consolidação** → confirmar atos vigentes; o que não confirmar vira "a confirmar" → `validador-holding`.

## 5. Cross-link
`tributario-holding-2026.md` (fonte) · `itcmd-itbi-sucessao.md` (ITBI/ITCMD) · `reforma-2027-watch` (2027) · `planejamento-tributario-holding` · `comparativo-pf-pj` · plugin `tributario-societario-adv-os`.

## 6. Fechamento
Peça tributária fecha por **`suprema-corte-holding`** (R3 tributário correto: Lei 15.270, Tema 796, presumido 32%) + **`validador-holding`**.
