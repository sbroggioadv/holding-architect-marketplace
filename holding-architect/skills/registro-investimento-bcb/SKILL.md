---
name: registro-investimento-bcb
description: Registra o investimento estrangeiro direto no Banco Central pelo SCE-IED — base legal Lei 14.286/2021 (Novo Marco Cambial, NUNCA a 4.131/62 revogada nesse ponto) + Res. BCB 278/2022, com prazos e quem declara (o receptor = holding BR, em até 30 dias da movimentação ≥ US$ 100 mil), mais o representante/procurador no Brasil (IN RFB 2.119/2022 art. 6º §1º, CC 1.134, art. 119 Lei 6.404/76). Sem registro, trava a repatriação de capital e a remessa de lucros. Use quando o operador disser "registro no BCB", "SCE-IED", "RDE-IED", "capital estrangeiro", "remeter lucro pro exterior", "declaração de investimento estrangeiro", "repatriar capital", "/offshore bcb".
---

# REGISTRO DO INVESTIMENTO ESTRANGEIRO NO BCB — SCE-IED

> Camada 5 (Offshore — ponta BR). Registra o capital que a entidade estrangeira ingressa na holding BR e garante o direito de repatriar capital e remeter lucros. Depende de `regularizacao-entidade-estrangeira-br` (CNPJ 221-6) feito.

## Anexos obrigatórios (context/)
- `context/offshore-ponta-br.md` — **§3** (SCE-IED, base legal, normas BCB, quem declara e prazos) e **§4** (representante/procurador no Brasil). `grep -n "14.286\|278/2022\|SCE-IED\|US\$ 100\|1.134\|art. 119\|CDNR" context/offshore-ponta-br.md`.

## Quando ativar
A entidade estrangeira vai aportar capital (moeda ou conferência de bens/quotas) na holding BR; o grupo vai distribuir lucros/dividendos ao sócio no exterior; ou é preciso assegurar a via cambial de saída de recursos.

## Base legal ancorada (context/offshore-ponta-br §3-§4) — o marco MUDOU
- **Lei 14.286/2021 (Novo Marco Legal Cambial)**, em vigor desde 31/12/2022, é a **base legal central do IED**. **Revogou** a disciplina de registro de capitais estrangeiros/remessas/reinvestimentos da **Lei 4.131/1962** (que sobrou residual). **Citar sempre a 14.286/2021 — nunca a 4.131/62 como base vigente do registro.**
- Normas BCB: **Res. BCB 278/2022** (núcleo do SCE-IED — crédito externo + IED + prestação de informações) · Res. CMN 5.042/2022 (câmbio) · Res. BCB 279 (capital BR no exterior) · 280 (residente/não residente) · 281 (Censo) · 131/2021 (penalidades).
- O **SCE-IED** (Sistema de Prestação de Informação de Capital Estrangeiro – Investimento Estrangeiro Direto) **substituiu o RDE-IED**.

## Quem declara e prazos (Res. BCB 278/2022)
- **Quem declara é o RECEPTOR** do investimento — a **holding BR**, não a estrangeira.
- **Por movimentação:** declarar quando houver transferência **≥ US$ 100.000** (ou equivalente) relativa ao investidor estrangeiro (conferência de quotas/ações, aquisição/alienação de participação, distribuição de lucros/dividendos, JCP, restituição de capital, capitalização). **Prazo: até 30 dias da ocorrência.**
- **Declarações periódicas** (por ativos totais na data-base): **Quinquenal** (ativos ≥ R$ 100 mil) · **Anual** (≥ R$ 100 milhões) · **Trimestral** (≥ R$ 300 milhões).
- **Penalidades (Res. BCB 131/2021):** fora do prazo, informação incorreta/incompleta/falsa, com tetos por faixa — **confirmar os valores no texto vigente antes de citar em peça** (marcar "a confirmar" → `validador-holding`).

> **Por que registrar:** o registro garante ao não residente o direito de **repatriar capital** e **remeter lucros/dividendos** pela via cambial regular. **Sem registro, trava a saída de recursos.**

## Representante / procurador no Brasil (§4)
- **Distinção crítica:** LLC que é **apenas sócia** da holding BR (não abre filial, não "funciona" no país) **não** precisa da autorização do Executivo do **art. 1.134 CC** (regime de filial/sucursal). A lógica de representante persiste por força da **IN RFB 2.119/2022 (art. 6º, §1º)** e do BCB.
- **Art. 119 da Lei 6.404/76:** o acionista domiciliado no exterior deve manter no Brasil representante com poderes para receber citação em ações societárias — **aplica-se quando a holding BR é S.A.**. Na **LTDA** não há dispositivo idêntico, mas o representante do CNPJ existe e o contrato social deve exigir representante no Brasil para o sócio estrangeiro.
- **Poderes mínimos da procuração** (apostilada + traduzida): (1) administrar bens/direitos no Brasil + representar perante a RFB; (2) receber citações/notificações; (3) representar perante o BCB (CDNR, registro no SCE-IED, declarações); (4) poderes societários (votar/representar em assembleias/reuniões); (5) manutenção sem lacuna de representação.

## Sequência operacional (o que produzir)
1. **Confirmar pré-requisitos:** CNPJ da estrangeira (NJ 221-6) obtido; cadastro de não residente no **CDNR** (pode ser pré-requisito/automático do CNPJ).
2. **Identificar o fato gerador do registro:** ingresso de capital (câmbio de moeda) **ou** conferência de bens/quotas → ambos disparam registro.
3. **Registrar o IED no SCE-IED** em **até 30 dias** da ocorrência (declarante = holding BR receptora).
4. **Agendar as declarações periódicas** conforme a faixa de ativos (quinquenal/anual/trimestral).
5. **Verificar a procuração** do representante contempla os poderes perante o BCB (item 3 acima); se não, ajustar via `estrangeira-como-socia`.
6. **Entregar** o checklist (fato gerador · valor · data · prazo de 30 dias · declarante · periodicidade) + alerta de penalidade por atraso.

## Postura honesta
- O registro **não é opcional** para quem quer remeter lucro/repatriar — é o que destrava a via cambial.
- **Valores de penalidade e terminologia (CDNR/CADEMP)**: só citar após conferir o manual SCE-IED e a Res. BCB 131/2021 vigentes.
- Registro ≠ economia de imposto: o beneficiário residente segue na Lei 14.754 (`offshore-diagnostico-fiscal`).

## Cross-link soft
Documentos + CNPJ da estrangeira → `regularizacao-entidade-estrangeira-br` · procuração e admissão no quadro → `estrangeira-como-socia` · jurisdição → `offshore-diagnostico-fiscal` · câmbio/tributação da remessa → `tributario-societario-adv-os`.

## Guard
Base do registro = **Lei 14.286/2021 + Res. BCB 278/2022** — **jamais a 4.131/62**. Nenhum valor/prazo/penalidade sem `validador-holding` (cruzar `context/offshore-ponta-br.md`). Fecha pela `suprema-corte-holding` (R1-R4).
