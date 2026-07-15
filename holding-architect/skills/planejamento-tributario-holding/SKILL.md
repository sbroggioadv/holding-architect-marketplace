---
name: planejamento-tributario-holding
description: "Calcula a economia tributaria REAL de uma holding patrimonial em 2026, pos-Lei 15.270/2025 — sem promessa de isencao. Compara PF x PJ com honestidade (locacao no lucro presumido, presuncao 32%, carga efetiva ~11,33-14,53% x PF ate 27,5%), soma o custo dos dividendos na saida (IRRF 10% acima de R$50k/mes + IRPFM acima de R$600k/ano), a integralizacao a custo x mercado (art. 23 Lei 9.249/95), a Lei 14.973/2024 e os limites do planejamento (proposito negocial/substancia, CARF, CTN 116). Use quando o operador pedir 'vale a pena a holding no imposto', 'quanto economizo', 'planejamento tributario da holding', 'holding paga menos imposto', 'dividendo isento ainda vale', 'lucro presumido da holding de aluguel', 'JCP na holding', 'integralizar a custo ou a mercado', 'holding paga imposto de renda'."
---

# Planejamento Tributario da Holding (economia REAL pos-Lei 15.270/2025)

> A holding continua vantajosa em 2026 — mas NAO pela lenda "deixa na PJ e saca isento", que **morreu para valor alto**. O produto vende a conta correta, somando a carga na entrada, na operacao E na saida. Sem promessa de isencao.

## Anexo obrigatorio (context/)
- `context/tributario-holding-2026.md` — **§1 integralizacao custo x mercado (art. 23 L.9.249) · §2 Lei 14.973/2024 · §4 dividendos Lei 15.270/2025 · §5 lucro presumido locacao (32%, carga efetiva) · §6 limites (proposito negocial/CARF)**. Localizar por `grep -niE "15.270|presuncao|32%|integraliza|14.973|CARF"`.

## Quando ativa
- Operador quer saber se a holding economiza imposto, quanto, e sob quais condicoes.
- Gatilhos: "vale a pena no imposto", "quanto economizo", "dividendo ainda e isento", "lucro presumido da holding de aluguel", "integralizar a custo ou a mercado", "JCP".

## Base tecnica ancorada (lei vigente 2026)

### 1. Locacao na holding — lucro presumido (o motor classico)
- **Locacao de imoveis proprios → presuncao de 32%** (nao 8%) para IRPJ e CSLL. Compra e venda de imoveis proprios → 8%. *(§5)*
- Carga efetiva sobre a **receita** de aluguel (base 32%): IRPJ 15%→**4,80%** · CSLL 9%→**2,88%** · PIS **0,65%** · COFINS **3,00%** = **≈ 11,33%**.
- **Adicional de IRPJ 10%** sobre lucro presumido que exceder R$ 20.000/mes → aluguel **> ~R$ 62.500/mes** eleva a carga a **≈ 14,53%**. **Faixa tipica: 11,33% a 14,53%.**
- PF: carne-leao / tabela progressiva ate **27,5%**. Migrar a locacao para a holding no presumido tipicamente derruba de ~27,5% para ~11,33-14,53%.
- **Limite do presumido: receita bruta anual R$ 78.000.000** — acima, Lucro Real. Locacao de proprios **nao** pode Simples. O objeto social deve trazer a locacao expressamente.

### 2. Dividendos — a maior mudanca (Lei 15.270/2025, vigente 01/01/2026) *(§4)*
A isencao do art. 10 da Lei 9.249/95 **segue no caput**, mas foi subordinada aos novos arts. 6º-A e 16-A da Lei 9.250/95:
- **IRRF de 10%** sobre dividendos a PF residente **acima de R$ 50.000/mes** por PJ (retem sobre o total, sem deducao). **NAO** se aplica a distribuicao PJ→PJ (isencao inter-PJ intacta — art. 10; e a base da celula 2% da ADM de Bens).
- **IRPFM** (renda total **> R$ 600.000/ano**): aliquota cresce linearmente de 0% a 10% entre R$ 600 mil e R$ 1,2 milhao (aliquota% = renda/60.000 − 10) e e 10% acima de R$ 1,2 mi/ano. Considera dividendos.
- **Redutor anti-bitributacao:** se [aliquota efetiva IRPJ+CSLL] + [IRPFM] passar do teto efetivo da PJ (34/40/45%), ha fator redutor do IRPFM.
- **Transicao:** lucros aprovados/acumulados **ate 31/12/2025** ficam isentos se distribuidos conforme o ato de aprovacao **ate 2028**. Janela de planejamento: deliberar a distribuicao dos lucros antigos antes do prazo.
> **Planejamento licito:** distribuir ≤ R$ 50k/mes por PJ/por socio mantem a isencao do art. 10 e evita o IRRF mensal (escalonamento / multiplas PJs / multiplos socios). **Mas** o IRPFM anual pode capturar quem passa de R$ 600 mil/ano somando tudo. (Regulamentacao infralegal em consolidacao — marcar "a confirmar".)

### 3. Integralizacao — a entrada (art. 23 Lei 9.249/95) *(§1)*
- **A custo historico (DIRPF):** sem ganho de capital no ato — **rota padrao** (zero imposto na entrada; difere a valorizacao).
- **A valor de mercado:** a diferenca (mercado − custo) e ganho de capital tributavel na PF: **15%** (ate R$ 5 mi) · **17,5%** · **20%** · **22,5%** (acima de R$ 30 mi). So quando ha razao (step-up para reduzir ITBI/ganho futuro).
- ITBI da integralizacao → cross-link `itbi-integralizacao` (Tema 796 + preponderancia).

### 4. Lei 14.973/2024 — atualizacao de imoveis a mercado *(§2)*
Regime optativo: **PF 4% / PJ 6%+4% = 10%** sobre a diferenca custo x mercado. **Janela encerrada em 16/12/2024** — em 2026 vale so como referencia historica para quem aderiu (carencia de 15 anos; vender antes de 3 anos = dupla tributacao). Nao oferecer como opcao vigente salvo reabertura legislativa (a confirmar).

### 5. JCP
Juros sobre capital proprio: dedutivel na PJ, tributado a **15% de IRRF** na PF. Aplicavel a holding com PL relevante — confirmar limites TJLP/PL e o impacto pos-15.270 no caso concreto.

## O que produzir
1. **Recorte da situacao:** natureza da receita (aluguel/participacoes/venda), volume mensal e anual, patrimonio, numero de socios.
2. **Conta dos 3 tempos** (com os numeros do operador, **nunca inventados**): entrada (integralizacao custo x mercado + ITBI) · operacao (presumido 32% x PF 27,5%) · **saida** (dividendo: ≤ R$50k/mes isento; acima, IRRF 10%; IRPFM se renda anual > R$600k).
3. **Estrategia licita:** escalonar distribuicao, usar a celula 2% PJ→PJ (isencao art. 10), deliberar lucros pre-2025 ate 2028.
4. **Veredito honesto:** onde a holding ganha, onde empata, onde perde — sem "isencao total".

## Postura honesta (as verdades duras)
- **Dividendo alto NAO e mais isento** (Lei 15.270/2025). Recalcular toda economia da PJ **na saida**.
- **Holding nao e blindagem nem passe livre fiscal** — precisa de **substancia** (conta propria, contabilidade, contratos de locacao a mercado, administracao efetiva) e **proposito documentado**. Sem isso e envelope vazio = autuacao. *(§6)*
- **Limites (CTN 116, §ú, LC 104/2001):** a norma antielisiva **nao foi regulamentada** em ambito federal; RFB/CARF desconsideram estruturas por **simulacao (CTN 149, VII) + proposito negocial + substancia sobre forma**. Elisao (opcoes legais antes do fato gerador) x evasao/simulacao (pode ser crime — Lei 8.137/1990).
- **Riscos da holding familiar:** distribuicao desproporcional sem causa → requalificacao como doacao disfarcada (ITCMD + multa); confusao patrimonial → desconsideracao (CC 50); pejotizacao → requalificacao (IRPF + previdenciario + multa).
- **Reforma 2027 so sinaliza** (IBS/CBS sobre locacao com redutor de 70%): a lei vigente de 2026 manda; avisar o cliente → `reforma-2027-watch`.

## Cross-link
`comparativo-pf-pj` (numeros lado a lado) · `base-tributaria-2026` (fundacao) · `itbi-integralizacao` e `integralizacao-de-imoveis` (entrada) · `celula-adm-de-bens` (isencao 2% PJ→PJ) · plugins `tributario-societario-adv-os`/`cfo-combativo-os` (modelagem pesada).

## Guard
Nenhum numero/aliquota/dispositivo sem confirmar em `context/tributario-holding-2026.md` → `validador-holding`. Nunca prometer isencao de dividendo alto. Regulamentacao infralegal do IRRF/IRPFM = "a confirmar". Janela 14.973 encerrada. Entrega fecha pela `suprema-corte-holding` (R3 tributario correto).
