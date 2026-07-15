---
name: celula-gestora-pagamentos
description: Desenha a Gestora de Pagamentos — celula de BACK-OFFICE financeiro do grupo (LTDA unipessoal, socio operacional 100%, CNAE 6619-3/99, inalienabilidade 5 anos, atua como MANDATARIA e NUNCA como instituicao financeira, com vedacao BCB expressa no objeto). Use quando o operador disser "gestora de pagamentos", "back-office financeiro", "centraliza os pagamentos do grupo", "celula que paga e recebe pelo grupo", "monta a Gestora", ou ao definir a celula que concentra as transacoes financeiras internas. Entrega os parametros e a fundamentacao (unipessoal, mandataria, vedacao BCB, CNAE) — o instrumento e do contrato-social-holding. So faz sentido com volume relevante de transacoes internas.
---

# CELULA GESTORA DE PAGAMENTOS — back-office (mandataria, nao instituicao financeira)

> Camada 2, celula 4. A Gestora e o **back-office**: paga e recebe **por conta e ordem** das empresas do grupo, como **mandataria** — nunca capta nem intermedia recursos de terceiros. Fiel ao metodo do Doc. Define a celula; o instrumento sai do `contrato-social-holding`. **E a 1ª a registrar** na sequencia de producao.

## Anexos obrigatorios (grep o topico + ler a faixa)
- `context/metodologia-4-celulas.md` §2 (Celula 4) — funcao, CNAE, vedacao BCB.
- `context/clausulas-padrao-holding.md` — blindagem, Livro de Decisoes, vedacoes de objeto.

## Quando ativa
So quando o grupo tem **volume relevante de transacoes financeiras internas** que justifica centralizar o back-office. Sem esse volume, **nao criar a celula** — cada empresa paga o proprio custo. Custo de manutencao (contabilidade, obrigacoes) tem que se pagar.

## 1. Parametros da celula (metodologia-4-celulas §2)
| Campo | Parametro |
|---|---|
| Funcao | Back-office financeiro e de pagamentos do grupo |
| Tipo | **LTDA unipessoal** |
| Composicao | Socio operacional **100%** (controlada 100% pela Holding de Participacoes) |
| Administracao | Socio operacional |
| Capital | A definir conforme o volume de operacoes |
| Inalienabilidade | **5 anos** |
| CNAE principal | **6619-3/99** (atividades auxiliares dos servicos financeiros n.e.) |

## 2. Objeto social e a VEDACAO BCB (o coracao desta celula)
Objeto: administracao financeira e de pagamentos **do proprio grupo** — recebimento e pagamento **por conta e ordem** das sociedades do grupo, conciliacao, tesouraria centralizada, gestao de fluxo interno, na qualidade de **mandataria**.
**Vedacao obrigatoria e EXPRESSA no objeto** — declaracao de que a sociedade **NAO** realiza atividades sujeitas a regulacao do **Banco Central do Brasil**: nao capta recursos do publico, nao intermedia recursos de terceiros, nao opera arranjo de pagamento regulado, nao concede credito a terceiros, nao e instituicao de pagamento nem instituicao financeira. **A Gestora paga e recebe pelo grupo; nao capta nem intermedia recursos de terceiros.** Sem essa vedacao, o objeto pode ser lido como atividade regulada → risco de nulidade/exigencia de autorizacao.

## 3. Vedacoes complementares
Vedar tambem: (a) atividade operacional/comercial/industrial propria; (b) **aval, fianca ou garantia** a terceiros — salvo deliberacao especial do socio unico registrada em Livro de Decisoes; (c) assuncao de obrigacoes de terceiros; (d) prestacao de servicos a controladas sem substancia economica real e a preco de mercado (arm's length).

## 4. Blindagem e governanca (unipessoal — espelha a Participacoes)
- **Incomunicabilidade** (1.911 + 1.668, I + 1.848 CC) · **impenhorabilidade** (1.026, caput CC) · **inalienabilidade 5 anos**.
- **Livro de Decisoes do Socio Unico** (substitui deliberacao assemblear — art. 1.072 CC): contas/balanco, distribuicao, alteracao contratual, garantias nas hipoteses ressalvadas.
- **Segregacao estrita (art. 49-A CC / Lei 13.874/2019):** contas e escrituracao proprias, sede distinta — sem confusao patrimonial (pressuposto contra desconsideracao). **A movimentacao por conta e ordem deve ter lastro documental** (mandato/instrucao de pagamento) para nao virar confusao patrimonial.
- Sem Golden Share (unipessoal).

## 5. Postura honesta
- A Gestora **e mandataria, nao banco.** Operar como se fosse instituicao de pagamento/financeira sem autorizacao e ilicito e destroi a estrutura. O rotulo no objeto tem que bater com a pratica.
- **Movimentar dinheiro das outras empresas sem lastro = confusao patrimonial** — municao pronta para desconsideracao (CC 50). A Gestora exige a disciplina documental mais rigorosa das 4 celulas.
- Impenhorabilidade **nao e absoluta** (frutos ao credor pessoal; nao vence fraude/simulacao/desconsideracao).
- Numero so do `context/`; o que nao confirmar → `validador-holding`.

## Cross-link (soft)
`celula-holding-participacoes` (controla 100% da Gestora) · `sequencia-de-producao` (a Gestora e a **1ª** a registrar) · `contrato-social-holding` (redige o instrumento) · `registro-jucesp-drei`.

## Fecha por
`suprema-corte-holding` R1 (estrutura) + R2 (fundamentacao vigente — vedacao BCB integra) + R4 (forma/registro) antes de virar documento.
