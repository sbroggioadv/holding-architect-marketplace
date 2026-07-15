---
name: celula-adm-de-bens
description: Desenha a Administradora de Bens — celula de RENDA ATIVA (holding mista LTDA 98/2: socio patrimonial 98% + Holding de Participacoes 2% PJ para distribuicao PJ->PJ isenta de IRRF, art. 10 Lei 9.249/95; CNAE 6462-0/00 + secundario 68.10-2/02 aluguel de imoveis proprios; Golden Share do patrimonial; inalienabilidade 15 anos). Use quando o operador disser "adm de bens", "administradora de bens", "holding que recebe aluguel", "celula que opera o patrimonio", "holding mista", "monta a ADM", "vou reaproveitar a holding que ja existe", ou ao definir a celula que administra patrimonio que GERA renda. Entrega os parametros e a fundamentacao da celula — o instrumento e do contrato-social-holding.
---

# CELULA ADM DE BENS — administracao ativa (holding mista)

> Camada 2, celula 2. A ADM **opera**: administra patrimonio proprio que gera renda ativa (aluguel, cessao onerosa, gestao de carteira) **e** detem participacoes. A Cofre so guarda; a ADM opera. Fiel ao metodo do Doc (ADM-DE-BENS-TEMPLATE). Define a celula; o instrumento sai do `contrato-social-holding`.

## Anexos obrigatorios (grep o topico + ler a faixa)
- `context/metodologia-4-celulas.md` §2 (Celula 2), §4 (fluxo de lucros).
- `context/tributario-holding-2026.md` — art. 10 Lei 9.249/95 (isencao inter-PJ), **Lei 15.270/2025** (fim da isencao PJ→PF de alto valor), lucro presumido.
- `context/clausulas-padrao-holding.md` — blindagem, Golden Share, objeto/CNAE, integralizacao.

## Quando ativa
Patrimonio que **gera renda ativa** — locacao, cessao onerosa de uso, gestao de aplicacoes, participacoes. Duas modalidades:
- **A — Alteracao** (caso mais comum): reaproveita uma **holding ja existente** do cliente → alteracao contratual com consolidacao integral + admissao da Participacoes.
- **B — Constituicao** do zero: usa a base da Cofre ajustando o objeto para **holding mista** (administracao de bens **+** participacoes).

## 1. Parametros da celula (metodologia-4-celulas §2)
| Campo | Parametro |
|---|---|
| Funcao | Administracao **ativa** do patrimonio + holding mista (renda) |
| Tipo | LTDA pluripessoal |
| Composicao | Socio patrimonial **98%** + **Holding de Participacoes LTDA 2% (PJ)** |
| Administracao | **Conjunta** |
| Golden Share | Socio **patrimonial** |
| Inalienabilidade | **15 anos** |
| CNAE | principal **6462-0/00**; secundario admitido **68.10-2/02** (aluguel de imoveis proprios) |

**Por que os 2% aqui sao da Holding de Participacoes (PJ), nao PF:** a distribuicao de lucros **PJ→PJ e isenta de IRRF** (**art. 10, Lei 9.249/1995**). Os lucros da ADM circulam no ambiente PJ enquanto o grupo desejar. A interposicao da Participacoes entre a PF e a ADM difere a tributacao na saida para a PF. Como a ADM e a **3ª** a registrar (apos Participacoes ja com CNPJ), a admissao dela e **ato de ALTERACAO** contratual (contrato consolidado + DBE de alteracao de QSA).

## 2. Objeto social (holding mista) e CNAE
Administracao do patrimonio **proprio** + participacao no capital de outras sociedades: (a) administracao/guarda/conservacao e **cessao onerosa de uso** de bens proprios; (b) participacao em outras sociedades (holding pura e mista — art. 2, §3, Lei 6.404/1976); (c) recebimento de alugueis, rendimentos, lucros e dividendos **proprios e das participacoes**; (d) gestao de aplicacoes proprias.
**Auditar o registro existente (modalidade A):** **EXCLUIR** os CNAEs de compra e venda de imoveis proprios (**68.10-2/01**) e loteamento (**68.10-2/03**) — objeto/CNAE imobiliario compromete a imunidade de ITBI (Tema 796). Manter so 6462-0/00 (+68.10-2/02 aluguel proprio).

## 3. Vedacoes ao objeto
Vedar: (a) compra e venda de imoveis **de terceiros**; (b) incorporacao imobiliaria e loteamento; (c) **atividade imobiliaria preponderante**; (d) qualquer atividade operacional/comercial/industrial; (e) **aval, fianca ou garantia** a terceiros ou a operacionais.

## 4. Blindagem e governanca (clausulas-padrao-holding)
Mesma arquitetura da Cofre: **incomunicabilidade** (1.911 + 1.668, I + 1.848 CC) · **impenhorabilidade** (1.026, caput CC) · **inalienabilidade 15 anos** · **protecao especial das quotas de 2%** (finalidade tributaria exclusiva — sem poder de gestao/veto) · **Golden Share ao patrimonial** · **administracao conjunta com alcadas** (quem opera assina; quem protege veta) · **tag along 100%** · **apuracao de haveres pelo valor contabil** (art. 1.031 CC, imoveis pelo valor DIRPF — afasta expressamente avaliacao a mercado).
**Na modalidade A**, a cessao dos 2% a Participacoes **nao gera ITBI** (quota, nao imovel) **nem ITCMD** (ato oneroso a valor nominal, sem animus donandi) — condicionada ao CNPJ da Participacoes ja registrado.

## 5. Fluxo de lucros e o ALERTA 2026 (verdade dura)
```
ADM apura lucro → 98% socio patrimonial (PF) | 2% Participacoes (PJ) — ISENTO IRRF (art. 10)
```
- **A isencao inter-PJ (art. 10) CONTINUA.** O que mudou e a **saida final para a PF**: a **Lei 15.270/2025** instituiu **IRRF de 10%** sobre dividendos de uma mesma PJ a uma mesma PF **acima de R$ 50.000/mes**, e o **IRPFM** (minimo) para quem recebe **> R$ 600.000/ano**. A tese "deixa na PJ e saca isento" **morreu para alto valor**.
- Recalcular a economia caso a caso (presumido 32% da atividade + carga da distribuicao) → `planejamento-tributario-holding` / `comparativo-pf-pj`. **Nunca** vender isencao total de dividendos.

## 6. Postura honesta
- ADM **nao e blindagem** (mesmos limites da Cofre: CC 50, fraude, simulacao, frutos ao credor).
- **Integralizacao imune so ate o capital** (Tema 796); excedente tributa ITBI.
- Numero so do `context/`; o que nao confirmar → `validador-holding`.

## Cross-link (soft)
`celula-empresa-cofre` (guarda pura) · `celula-holding-participacoes` (a socia 2% PJ) · `alteracao-contratual` (modalidade A) · `contrato-social-holding` (modalidade B) · `planejamento-tributario-holding` · `sequencia-de-producao`.

## Fecha por
`suprema-corte-holding` R1 (estrutura) + R3 (tributario correto — Lei 15.270, art. 10, Tema 796) + R4 (forma) antes de virar documento.
