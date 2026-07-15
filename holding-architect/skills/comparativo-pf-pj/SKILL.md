---
name: comparativo-pf-pj
description: Monta o comparativo quantitativo de carga tributária PESSOA FÍSICA (aluguel no carnê-leão até 27,5%) × PJ HOLDING no lucro presumido (locação presunção 32% → ~11,33% a 14,53%), SEMPRE somando a saída pós-Lei 15.270/2025 (IRRF 10% sobre dividendos > R$ 50k/mês + IRPFM > R$ 600k/ano) e sinalizando o IVA dual sobre locação (−70%, forward-look 2027). Usa os NÚMEROS do operador — nunca inventa valor. Use quando o operador disser "compara PF e PJ", "quanto economizo com a holding", "vale a pena tributariamente", "aluguel na pessoa física ou na empresa", "carga do aluguel", "simula a economia", "holding compensa no imposto?", "/comparativo-pf-pj".
---

# COMPARATIVO PF × PJ (HOLDING)

> Camada Consultivo/diferencial. Traduz a decisão "pessoa física ou holding" em números — honestos, com a saída pós-Lei 15.270 embutida. Alimenta `parecer-viabilidade-holding` e `planejamento-tributario-holding`. NÃO inventa valor: opera sobre os dados do operador.

## Anexos obrigatórios (context/)
- `context/tributario-holding-2026.md` — **§5** (holding de aluguel no presumido: presunção 32%, carga ~11,33-14,53%, adicional IRPJ, limite R$ 78 mi, PF até 27,5%) + **§4** (dividendos Lei 15.270/2025) + **§1** (integralização custo × mercado, ganho de capital 15-22,5%). `grep -n "32%\|11,33\|14,53\|27,5\|50.000\|600.000\|78.000.000" context/tributario-holding-2026.md`.
- `context/reforma-2027-watch.md` — **§2** (IVA dual sobre locação: −70% art. 261, redutor social art. 260, filtro PF art. 251; forward-look). Sinalizar, não aplicar.

## Quando ativar
Cliente quer saber quanto economiza; comparação PF × holding para renda de aluguel; dúvida se a holding compensa tributariamente.

## Dados que o operador precisa fornecer (nunca presumir)
Receita de aluguel mensal/anual · nº de imóveis · valor DIRPF × valor de mercado dos imóveis · rendimento anual total do sócio (para o teste do IRPFM) · quanto o sócio pretende sacar por mês da PJ · outras rendas do sócio. **Faltando dados, pedir — não estimar.**

## Base de cálculo ancorada (tributario-holding §5)
**PJ holding — locação de imóveis próprios no lucro presumido (presunção 32%):**
| Tributo | Cálculo | % sobre a receita |
|---|---|---|
| IRPJ 15% | 15% × 32% | 4,80% |
| CSLL 9% | 9% × 32% | 2,88% |
| PIS (cumulativo) | sobre receita | 0,65% |
| COFINS (cumulativo) | sobre receita | 3,00% |
| **Total (sem adicional)** | | **≈ 11,33%** |
- **Adicional de IRPJ (10%)** sobre lucro presumido que exceder R$ 20.000/mês (R$ 60.000/trimestre) → receita de aluguel **> ~R$ 62.500/mês** começa a gerar adicional → carga pode chegar a **≈ 14,53%**. **Faixa efetiva típica: 11,33% a 14,53%.**
- **Limite do presumido:** receita bruta anual **R$ 78.000.000**; acima, Lucro Real. Locação de imóveis próprios **não** pode optar pelo Simples. Objeto social deve prever locação expressamente. Presunção de **8%** é só para **compra e venda** de imóveis, não para locação.

**PF — aluguel:** carnê-leão / tabela progressiva **até 27,5%** (sem PIS/COFINS, deduções limitadas).

## A SAÍDA — Lei 15.270/2025 (o que quase todo comparativo esquece — tributario §4)
Somar SEMPRE a carga na **distribuição da PJ ao sócio PF**:
1. **IRRF 10%** se a mesma PJ paga à mesma PF **> R$ 50.000/mês** — 10% sobre o **total**, sem dedução.
2. **IRPFM** (mínimo) se o sócio recebe **> R$ 600.000/ano** — alíquota cresce de 0% a 10% entre R$ 600 mil e R$ 1,2 mi, 10% acima de R$ 1,2 mi/ano; considera dividendos.
3. **Redutor anti-bitributação:** se [IRPJ+CSLL efetivo] + IRPFM ultrapassar o teto (34/40/45%), há fator redutor.
4. **Transição:** lucros acumulados até 31/12/2025 isentos se distribuídos conforme o ato até 2028 — janela de planejamento.
> **A conta "11% na PJ e saca isento" morreu para alto valor.** O comparativo só é honesto se somar a saída.

## Metodologia (o que produzir)
1. **Cenário PF:** receita anual × alíquota efetiva do carnê-leão (com deduções informadas).
2. **Cenário PJ — dentro da holding:** receita × 11,33% (ou 14,53% se estourar o adicional).
3. **Cenário PJ — na saída ao sócio:** aplicar IRRF 10% (se saque > R$ 50k/mês) + IRPFM (se renda anual > R$ 600k), com o redutor.
4. **Carga total PJ = tributação da holding + tributação da saída.** Comparar com a PF.
5. **Integralização (one-off):** lembrar do ganho de capital se a mercado (15-22,5%, tributario §1) e do ITBI (Tema 796 — `itbi-integralizacao`); a custo histórico não há ganho na entrada.
6. **Forward-look:** sinalizar que o IVA dual (−70% na locação, art. 261) tende a estreitar a vantagem da PJ na transição 2027-2033 — **sem prometer percentual fechado** (alíquota de referência não é oficial).
7. **Devolver a tabela** (PF × PJ-só-holding × PJ-com-saída) + o veredito: em que faixa de saque/renda a holding ainda compensa.

## Postura honesta
- **Nunca inventar número.** Faltou dado, pediu.
- **Nunca vender "isento pra sempre"** — a saída pós-15.270 entra sempre.
- Percentuais do IVA 2027 = forward-look, não definitivo.
- O comparativo é tributário; a decisão final pondera também proteção/sucessão/custo de manutenção (`parecer-viabilidade-holding`).

## Cross-link soft
Parecer de entrada → `parecer-viabilidade-holding` · planejamento completo → `planejamento-tributario-holding` · integralização/ITBI → `itbi-integralizacao` · cálculo fino → `calculosjudiciais-adv-os` · IVA/reforma → `reforma-2027-watch`.

## Guard
Alíquotas/faixas só do `context/tributario-holding-2026.md` via `validador-holding`. Presunção locação = **32%** (nunca 8%); limite presumido = **R$ 78 mi**; gatilhos 15.270 = **R$ 50k/mês** e **R$ 600k/ano**. Fecha pela `suprema-corte-holding` (R1-R4).
