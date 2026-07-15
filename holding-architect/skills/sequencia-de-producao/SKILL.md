---
name: sequencia-de-producao
description: Orquestra a ordem de constituicao e registro das 4 celulas — Gestora -> Cofre -> Participacoes -> ADM de Bens — respeitando as dependencias de CNPJ (a Participacoes precisa de CNPJ existente para ser admitida como socia de 2% da ADM). Use quando o operador disser "qual a ordem de abrir as empresas?", "o que registro primeiro?", "sequencia de producao", "sequencia de registro", "monta o cronograma da holding", "ja tenho a Cofre, e agora?", ou ao planejar a producao/registro dos documentos. Entrega a ordem, o porque de cada passo, o que cada registro depende e onde entram alteracao/DBE — nao redige os instrumentos (isso e contrato-social-holding / alteracao-contratual).
---

# SEQUENCIA DE PRODUCAO — a ordem que respeita a dependencia de CNPJ

> Camada 2, orquestra as 4 celulas no tempo. A ordem nao e estilo — e **dependencia registral**: uma PJ so entra como socia de outra depois de ter CNPJ. Fiel ao metodo do Doc. Define a ordem; os instrumentos saem do `contrato-social-holding` / `alteracao-contratual`.

## Anexo obrigatorio (grep o topico + ler a faixa)
- `context/metodologia-4-celulas.md` §5 (sequencia de producao) — a ordem e o porque.
- `context/societario-jucesp-sa.md` — roteiro JUCESP, DBE/Redesim, viabilidade, ato de alteracao de QSA.

## Quando ativa
Depois que `diagnostico-estrutura` definiu quais celulas e antes/durante a producao dos documentos. Tambem quando o cliente ja tem parte da estrutura e precisa saber o proximo passo.

## A ORDEM (sempre nesta sequencia)
```
1. GESTORA DE PAGAMENTOS   → constituicao → obtem CNPJ
2. EMPRESA COFRE           → constituicao → obtem CNPJ
3. HOLDING DE PARTICIPACOES → constituicao → obtem CNPJ
4. ADM DE BENS             → ALTERACAO com admissao da Participacoes como socia 2%
                             (insere o CNPJ obtido no passo 3)
```

### Por que esta ordem (dependencia de CNPJ)
- **A Participacoes precisa de CNPJ existente** para ser admitida como socia de 2% da ADM de Bens. Por isso a Participacoes (passo 3) vem **antes** da entrada na ADM (passo 4).
- **A entrada da Participacoes na ADM e ato de ALTERACAO contratual** — nao constituicao: exige contrato **consolidado** + **DBE de evento de alteracao de QSA** (quadro societario). Ver `alteracao-contratual` e `societario-jucesp-sa.md`.
- **A ADM em modalidade A** (reaproveita holding existente) ja tem CNPJ/NIRE — o passo 4 e a 1ª alteracao com consolidacao. Em **modalidade B** (ADM do zero), o passo 4 vira constituicao apos o passo 3.

### O 2% da Cofre (passo 2) — decisao GUIADA (ver `celula-empresa-cofre` §1.1)
Duas rotas, pela intencao do cliente:
- **(A) 2% PF direto** — quando ha socio PF "limpo" que pode participar da retirada util ate ~R$ 50k/mes (dividendo ainda favoravel, abaixo do gatilho da Lei 15.270/2025). A Cofre entra no passo 2 com os 2% em **PF**; a Participacoes nasce no passo 3 sem afetar a Cofre. **Sequencia padrao Gestora→Cofre→Participacoes→ADM intacta.**
- **(B) 2% da Participacoes (fidelidade ao COFRE-TEMPLATE)** — quando NAO ha esse socio PF, ou o objetivo e concentracao/controle. Exige **inverter a ordem**: constituir a Participacoes **antes** da Cofre (Gestora→**Participacoes**→Cofre→ADM), OU fazer **cessao posterior** das quotas PF para a Participacoes (ato de alteracao adicional apos o CNPJ do passo 3).
Nao ha dependencia de CNPJ para constituir a Cofre com os 2% em PF (rota A).

## Passo a passo operacional de cada registro (societario-jucesp-sa)
Para cada celula, na sua vez:
1. **Viabilidade de nome + endereco** (Redesim/JUCESP) — consulta previa.
2. **DBE / coleta** na RFB (evento de inscricao; no passo 4, evento de alteracao).
3. **Instrumento** (constituicao ou alteracao consolidada) — `contrato-social-holding` / `alteracao-contratual`.
4. **Arquivamento na Junta** (JUCESP se SP; confirmar na junta local se outro estado).
5. **CNPJ / inscricoes** apos deferimento → alimenta o proximo passo.
6. **Atualizar `memoria-de-caso-holding`** com o CNPJ obtido e a fase.

## Campos que ficam em branco ate o registro (marcar como pendencia)
- **CNPJ** de cada celula — so apos o arquivamento dela.
- **CNPJ da socia PJ** (Participacoes) no instrumento da ADM — inserir antes de arquivar o passo 4.
- **Endereco da sede** — cliente define antes do registro.
- **Data** do instrumento — no ato da assinatura.
Nenhum instrumento vai a arquivamento com esses campos vazios.

## Postura honesta
- **Nao paralelizar cegamente:** tentar registrar a ADM (passo 4) com a Participacoes ainda sem CNPJ = exigencia/indeferimento na Junta. A ordem existe por isso.
- **Modalidade A pede coordenacao com o contador** do cliente para evitar conflito de procuracoes no ato da alteracao, e **auditoria dos CNAEs** do registro original (excluir 68.10-2/01 e 68.10-2/03 — ver `celula-adm-de-bens`).
- Prazos e exigencias variam por Junta/estado — confirmar no `registro-jucesp-drei`; o que nao confirmar → `validador-holding`.

## Cross-link (soft)
`celula-gestora-pagamentos` (passo 1) · `celula-empresa-cofre` (passo 2) · `celula-holding-participacoes` (passo 3) · `celula-adm-de-bens` (passo 4) · `contrato-social-holding` / `alteracao-contratual` (instrumentos) · `registro-jucesp-drei` · `memoria-de-caso-holding`.

## Fecha por
`suprema-corte-holding` R4 (forma/registro/sequencia) confirma a ordem e as dependencias antes da producao.
