---
name: estrangeira-como-socia
description: Admite a entidade estrangeira já regularizada (CNPJ 221-6 + registro BCB) como sócia/acionista da holding brasileira — qualificação no ato societário, sequência operacional completa da ponta BR e a procuração com poderes mínimos (societários + citação + RFB + BCB), com as travas por tipo societário (art. 119 Lei 6.404/76 na S.A.; representante exigido no contrato na LTDA; art. 1.134 CC não se aplica a mera sócia). Use quando o operador disser "colocar a LLC como sócia", "estrangeira no quadro societário", "admitir empresa do exterior na holding", "alteração pra entrar sócio estrangeiro", "acionista no exterior na S.A.", "qualificação do sócio estrangeiro", "/offshore socia".
---

# ESTRANGEIRA COMO SÓCIA/ACIONISTA DA HOLDING BR

> Camada 5 (Offshore — ponta BR). Fecha a ponta brasileira: coloca a entidade estrangeira dentro da holding. Consolida `regularizacao-entidade-estrangeira-br` (CNPJ) + `registro-investimento-bcb` (SCE-IED) num único ato societário.

## Anexos obrigatórios (context/)
- `context/offshore-ponta-br.md` — **§5** (entrada da estrangeira como sócia/acionista + qualificação + sequência operacional completa) e **§4** (representante/procurador, poderes mínimos, art. 119 LSA × LTDA). `grep -n "§ 5\|221-6\|art. 119\|1.134\|procuração\|qualificação" context/offshore-ponta-br.md`.
- `context/societario-jucesp-sa.md` — roteiro de **alteração contratual** (LTDA) / atos da **S.A.**, DBE de alteração de QSA, exigências da junta.

## Quando ativar
A entidade estrangeira já tem CNPJ (NJ 221-6) e representante no Brasil, e vai entrar como quotista da holding LTDA ou acionista da S.A. — na constituição ou por alteração.

## Base legal ancorada (context/offshore-ponta-br §4-§5)
- **Qualificação no ato societário:** razão social da estrangeira · endereço no exterior · **CNPJ da estrangeira (NJ 221-6)** · nome + CPF do representante/procurador no Brasil · referência à **procuração arquivada**.
- **LTDA:** entra como **quotista** (constituição ou alteração que a admite). Não há art. 119; o **contrato social deve exigir representante no Brasil** para o sócio estrangeiro (poderes de voto, alteração contratual, citação).
- **S.A.:** entra como **acionista** — observar **art. 119 da Lei 6.404/76** (acionista domiciliado no exterior mantém representante no Brasil com poderes para receber citação em ações societárias) + registro no **livro de ações**.
- **Art. 1.134 CC NÃO se aplica** a estrangeira que é **apenas sócia** (não abre filial/sucursal) — não precisa de autorização do Executivo. Não confundir com o regime de filial.
- **Procuração — poderes mínimos** (apostilada + traduzida): (1) administrar bens/direitos no Brasil + RFB; (2) receber citações/notificações; (3) representar perante o BCB (CDNR/SCE-IED); (4) votar e representar em assembleias (S.A.) / reuniões de sócios e alterações contratuais (LTDA); (5) sem lacuna de representação enquanto durar o investimento.

## Sequência operacional (o que produzir) — a ponta BR inteira (§5)
1. **Lá fora (parceiro):** entidade aberta + Certificate of Formation/Good Standing/Operating Agreement + **procuração** ao representante no Brasil.
2. **Apostila** no país de origem → **tradução juramentada** no Brasil (`regularizacao-entidade-estrangeira-br`).
3. **CNPJ da estrangeira** (NJ 221-6) + QSA/beneficiário final.
4. **Cadastro de não residente no BCB (CDNR)** — pode ser pré-requisito/automático do CNPJ.
5. **Constituir/alterar a holding BR** admitindo a estrangeira (junta comercial) — se holding já existe, é **ato de ALTERAÇÃO** de QSA (contrato consolidado + DBE de alteração); ver `alteracao-contratual` / `societario-jucesp-sa`.
6. **Ingresso do capital:** câmbio (moeda) ou conferência de bens/quotas → **registrar o IED no SCE-IED em até 30 dias** (`registro-investimento-bcb`).
7. **Atualizar o CNPJ da holding** (QSA com a estrangeira) + beneficiário final.

## O que redigir
- **Cláusula de qualificação** da sócia estrangeira (dados do §5) na constituição ou alteração.
- **Cláusula de representação** obrigatória (LTDA) exigindo representante no Brasil com os 5 poderes mínimos; na **S.A.**, verificar o art. 119 e o livro de ações.
- **Minuta de procuração** (poderes mínimos) para apostila + tradução.
- **Checklist de sequência** (passos 1-7) com o gate: sem CNPJ 221-6 e sem procuração válida, **não** protocolar a alteração.

## Postura honesta
- **Ordem inegociável:** documentos → CNPJ → BCB → ato societário → registro do IED. Admitir a estrangeira sem CNPJ 221-6 ou sem procuração válida = exigência/rejeição na junta.
- Entrada da estrangeira **não muda** a tributação do beneficiário residente (Lei 14.754) nem torna a holding blindagem — só organiza a titularidade.
- Sinalizar o **ITCMD forward-look** (EC 132 art. 16) se houver sucessão envolvendo os ativos no exterior (`reforma-2027-watch`).

## Cross-link soft
Documentos + CNPJ → `regularizacao-entidade-estrangeira-br` · registro do capital → `registro-investimento-bcb` · jurisdição/decisão → `offshore-diagnostico-fiscal` · alteração/consolidação → `alteracao-contratual` + `registro-jucesp-drei` · S.A. → `estatuto-e-atos-sa`.

## Guard
Qualificação sempre com **CNPJ NJ 221-6**; base do IED = **Lei 14.286/2021** (não 4.131/62); S.A. → **art. 119 Lei 6.404/76**. Nenhum dispositivo sem `validador-holding` (cruzar `context/offshore-ponta-br.md`). Fecha pela `suprema-corte-holding` (R1-R4).
