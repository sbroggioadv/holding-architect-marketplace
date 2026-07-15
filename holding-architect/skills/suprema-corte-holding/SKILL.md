---
name: suprema-corte-holding
description: Gate de qualidade final (R1-R4) de toda estrutura, contrato, parecer ou peça de holding antes da entrega. R1 confere estrutura/sócios/patrimônio e sequência das 4 células; R2 confere fundamentação vigente (nunca lei revogada); R3 confere tributário/sucessório correto (Lei 15.270, ITCMD-SP 4% fixo, Tema 796); R4 confere forma/registro JUCESP. Use SEMPRE antes de entregar qualquer produto de holding, quando pedirem "revisão final", `/revisao-final-holding`, ou ao fechar uma trilha do `holding-master`. Emite veredito APROVADO / AJUSTAR / REPROVADO com a correção.
---

# suprema-corte-holding — auditoria de excelência R1-R4

Última barreira antes da entrega. Auditor cético: nada passa por elogio, só por prova. Roda em 4 rounds; cada round pode devolver **AJUSTAR** (com a correção exata) ou **REPROVADO**. Só sai com **APROVADO** nos quatro.

## Quando ativa
Ao final de qualquer skill que produz peça, estrutura, cálculo ou parecer. É o fechamento obrigatório do `holding-master`. Também roda sob demanda ("revisa isso", `/revisao-final-holding`).

## R1 — Estrutura, sócios e patrimônio
- As 4 células estão coerentes com o objetivo? Cofre = guarda; ADM = renda ativa; Participações = controle; Gestora = back-office.
- **Quotas:** Cofre = 98% patrimonial + 2% operacional **PF direto**. ADM = 98% patrimonial + 2% **Participações (PJ)**. Participações e Gestora unipessoais. Errou a natureza dos 2% da ADM (PF em vez de PJ)? **AJUSTAR** — quebra a isenção inter-PJ.
- **Golden Share** com o sócio **patrimonial** (não o operacional). **Administração conjunta** — quem opera assina, quem protege veta (senão: administrador de fato + simulação art. 167 CC).
- **Inalienabilidade:** 15a Cofre/ADM · 5a Participações/Gestora. Recaiu sobre a legítima? Exige justa causa declarada (**CC 1.848**) — senão nulidade.
- **Sequência de produção** respeitada: Gestora → Cofre → Participações → ADM (por alteração). Ver `metodologia-4-celulas.md`.

## R2 — Fundamentação vigente (nunca lei revogada)
- Todo dispositivo/súmula/tema citado existe e está **vigente em 2026** e ancorado no `context/`? Sem âncora → volta ao `validador-holding`.
- **Súmula 49 STF é a CURTA** — "A cláusula de inalienabilidade inclui a incomunicabilidade dos bens." A versão inflada ("justa causa... impenhorabilidade e incomunicabilidade") é **fabricada** → REPROVADO. Ligação inalienabilidade→impenhorabilidade vem do **CC art. 1.911**, não da súmula.
- **Registro de capital estrangeiro = Lei 14.286/2021** (+ Res. BCB 278/2022) — **não** a 4.131/62 nesse ponto. Citou 4.131 como vigente? AJUSTAR.
- Reforma 2027 apareceu como **vigente**? REPROVADO — ela só sinaliza (`reforma-2027-watch`).

## R3 — Tributário e sucessório corretos
- **Dividendos:** o texto ainda diz "100% isento, sempre"? REPROVADO. Regra 2026 = **Lei 15.270/2025**: IRRF 10% sobre dividendos de uma mesma PJ a uma mesma PF **> R$ 50.000/mês** (sobre o total) + IRPFM para renda **> R$ 600.000/ano**. Isenção **inter-PJ** (art. 10) segue intacta.
- **ITCMD-SP = 4% FIXO** (não progressivo em SP hoje). Doação com reserva de usufruto: nua-propriedade **2/3**, usufruto **1/3** (base patrimonial na holding fechada). Consolidação: isenção do art. 6º, I, "f" **não** cobre o caso típico (nu-proprietário não foi o instituidor).
- **ITBI integralização — Tema 796 (RE 796.376/SC):** imunidade **não alcança o valor que exceder o capital social a integralizar**; o excedente pode ser tributado. Holding de **locação** tipicamente não goza da imunidade (atividade preponderante imobiliária). Postura honesta obrigatória.
- **Integralização a custo histórico** (art. 23 L.9.249/95) = sem ganho de capital; a mercado = ganho de capital PF 15–22,5%.
- **Lucro presumido locação:** presunção **32%** (não 8%) → carga efetiva ~11,33–14,53%. **Limite do presumido = receita ≤ R$ 78.000.000/ano.**

## R4 — Forma, registro e sequência
- **JUCESP** aceita? Sem quadro-resumo na abertura de LTDA; sem regime tributário no contrato; sem reserva de lucro com cap; sem auditoria externa obrigatória; §§ no padrão. Ver `societario-jucesp-sa.md`.
- **Gestora** tem a **vedação BCB expressa** no objeto? Ausente → AJUSTAR.
- Documento certo para o ato: constituição × **alteração** (entrada da Participações na ADM é alteração). DBE/Redesim/viabilidade coerentes.
- Qualificação completa dos sócios (PF e PJ); CNAE correto por célula (6462-0/00 · 6619-3/99 Gestora).

## Veredito (formato de saída)
```
R1 estrutura ...... APROVADO | AJUSTAR: <o quê> | REPROVADO: <por quê>
R2 fundamentação .. ...
R3 tributário ..... ...
R4 forma/registro . ...
VEREDITO FINAL: APROVADO / AJUSTAR / REPROVADO
```
Qualquer AJUSTAR/REPROVADO volta à skill de origem com a correção precisa. Divergência de número não resolvida → `validador-holding`. Não invente jurisprudência para "salvar" a peça — marque "a confirmar".
