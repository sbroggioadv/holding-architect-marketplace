---
name: celula-holding-participacoes
description: Desenha a Holding de Participacoes — celula de CONTROLE das operacionais (LTDA unipessoal, socio operacional 100%, CNAE 6462-0/00, quotas impenhoraveis, inalienabilidade 5 anos, Livro de Decisoes do Socio Unico). Detem 100% das operacionais + 100% da Gestora + 2% da ADM de Bens (interposicao inter-PJ). Use quando o operador disser "holding de participacoes", "celula que controla as empresas", "onde ficam as operacionais", "holding do socio de risco", "monta a Participacoes", ou ao definir a celula que segrega o risco operacional do patrimonio (art. 1.024 CC). Entrega os parametros e a fundamentacao — o instrumento e do contrato-social-holding.
---

# CELULA HOLDING DE PARTICIPACOES — controle e segregacao do risco

> Camada 2, celula 3. A Participacoes **controla** as operacionais e **interpoe** o socio de risco entre a PF e o patrimonio. Credor da operacional para na quota impenhoravel dela e nao alcanca Cofre nem ADM (art. 1.024 CC). Fiel ao metodo do Doc (PARTICIPACOES-TEMPLATE). Define a celula; o instrumento sai do `contrato-social-holding`.

## Anexos obrigatorios (grep o topico + ler a faixa)
- `context/metodologia-4-celulas.md` §2 (Celula 3), §3 (fluxo de protecao).
- `context/clausulas-padrao-holding.md` — blindagem, vedacoes, Livro de Decisoes, integralizacao de participacoes.
- `context/tributario-holding-2026.md` — art. 10 (isencao inter-PJ), presumido.

## Quando ativa
Ha empresas operacionais de risco a controlar. A Participacoes e a **camada de risco** do grupo — 100% do socio operacional, unipessoal. Nao guarda patrimonio imobilizado (isso e Cofre/ADM).

## 1. Parametros da celula (metodologia-4-celulas §2)
| Campo | Parametro |
|---|---|
| Funcao | Controle societario das operacionais + interposicao inter-PJ |
| Tipo | **LTDA unipessoal** (art. 1.052, §§1º-2º, CC) |
| Composicao | Socio operacional **100%** |
| Administracao | Socio operacional |
| Capital | Minimo funcional (ex.: R$ 10.000 a R$ 100.000) |
| Inalienabilidade | **5 anos** |
| CNAE principal | **6462-0/00** |

**Por que o socio operacional NAO detem as operacionais diretamente:** credor de qualquer operacional (trabalhista, fiscal, contratual) nao penhora as quotas da Participacoes (impenhoraveis por clausula) nem alcanca a Cofre ou a ADM — **separacao societaria absoluta (art. 1.024 CC:** os bens da sociedade respondem por suas dividas; nao se confundem com os do socio nem com os de outra PJ). **Por que 5 anos** (nao 15): celula operacional precisa de flexibilidade para reorganizacoes societarias.

## 2. Portfolio tipico
- **100%** das operacionais do setor do grupo;
- **100%** da Gestora de Pagamentos;
- **2%** da ADM de Bens (interposicao inter-PJ — viabiliza distribuicao PJ→PJ isenta, art. 10 Lei 9.249/95).

## 3. Objeto social e participacoes inter-PJ
Objeto **exclusivo**: participacao societaria em outras sociedades (quotista/acionista), exercendo controle, coordenacao estrategica e governanca das participadas, com enfase no setor operacional do grupo. **Proposito negocial declarado** (unificacao da governanca + organizacao patrimonial) afasta CTN 116 §unico. Admitir expressamente a **participacao minoritaria de 2%** nas holdings patrimoniais (Cofre e ADM) com **finalidade exclusiva** do art. 10 Lei 9.249/95.

## 4. Vedacoes ao objeto
Vedar: (a) **atividade imobiliaria preponderante** (preserva imunidade ITBI — Tema 796 / RE 796.376/SC); (b) atividade operacional/comercial/industrial direta; (c) **aval, fianca ou garantia** a controladas/coligadas/terceiros — **salvo deliberacao especial expressa do socio unico** registrada em Livro de Decisoes, com interesse societario; (d) assuncao de obrigacoes de terceiros nas mesmas condicoes; (e) prestacao de servicos a controladas sem substancia economica real e a preco de mercado.

## 5. Blindagem e governanca (unipessoal)
- **Incomunicabilidade** (1.911 + 1.668, I + 1.848 CC) · **impenhorabilidade** (1.026, caput CC) · **inalienabilidade 5 anos**.
- **Livro de Decisoes do Socio Unico** — substitui a deliberacao assemblear (art. 1.072 CC): aprovacao de contas/balanco, distribuicao, alteracao contratual, transformacao/fusao/cisao, aquisicao/alienacao de participacoes relevantes, endividamento, garantias nas hipoteses ressalvadas. Prova a regularidade da gestao perante Fisco e Judiciario.
- **Segregacao estrita (art. 49-A CC / Lei 13.874/2019):** escrituracao segregada, contas proprias, sede distinta da residencia e das operacionais — pressuposto pratico contra a **desconsideracao inversa**.
- Sem Golden Share (unipessoal — o controle ja e 100% do titular). Nao ha tag along salvo ingresso futuro de socio.

## 6. Integralizacao de participacoes
Aumento de capital com quotas/acoes de outras sociedades, avaliadas por **laudo contabil (CRC)** pelo valor patrimonial, observados JUCESP e RFB. (A regra do valor DIRPF do art. 23 Lei 9.249/95 e para **imoveis** — participacoes vao por laudo.) A transferencia das operacionais para a Participacoes e negocio autonomo, formalizado em instrumento proprio.

## 7. Postura honesta
- A impenhorabilidade **nao e absoluta**: o credor **pessoal** do socio alcanca os **frutos** (lucros — CC 1.026, caput) e pode requerer a **liquidacao da quota** (CC 1.031). A segregacao nao vence fraude a execucao, fraude contra credores, simulacao nem desconsideracao (CC 50).
- A blindagem **depende da pratica**: sem escrituracao segregada e sem ausencia de confusao patrimonial (art. 49-A), a clausula formal nao segura. Estrutura de papel cai.
- Numero so do `context/`; o que nao confirmar → `validador-holding`.

## Cross-link (soft)
`celula-gestora-pagamentos` (100% controlada pela Participacoes) · `celula-adm-de-bens` (recebe os 2% PJ) · `celula-empresa-cofre` · `sequencia-de-producao` (registrar apos Gestora e Cofre) · `contrato-social-holding` · `acordo-de-socios` (se entrar socio futuro).

## Fecha por
`suprema-corte-holding` R1 (estrutura/segregacao) + R2 (fundamentacao vigente) + R4 (forma) antes de virar documento.
