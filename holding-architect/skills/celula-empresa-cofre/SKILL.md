---
name: celula-empresa-cofre
description: Desenha a Empresa Cofre — celula de GUARDA PURA do patrimonio imobilizado (LTDA 98/2, socio patrimonial 98% + socio operacional 2% em PF direto OU via Participacoes conforme a intencao do cliente, CNAE 6462-0/00, Golden Share do patrimonial, inalienabilidade 15 anos, administracao conjunta). Use quando o operador disser "empresa cofre", "holding de guarda", "quero blindar os imoveis parados", "celula que so guarda", "cofre patrimonial", "monta a Cofre", ou ao definir a celula que abriga bens que nao operam nem geram risco. Entrega os parametros e a fundamentacao da celula (98/2, objeto, vedacoes, blindagem, Golden Share, integralizacao) — a redacao do instrumento e do contrato-social-holding.
---

# CELULA EMPRESA COFRE — guarda pura do patrimonio imobilizado

> Camada 2, celula 1. A Cofre **guarda**: recebe o patrimonio imobilizado blindado, nao opera, nao cede a terceiros, nao gera risco. Fiel ao metodo do Doc (COFRE-TEMPLATE). Esta skill DEFINE a celula; o instrumento sai do `contrato-social-holding`.

## Anexos obrigatorios (grep o topico + ler a faixa)
- `context/metodologia-4-celulas.md` §2 (Celula 1) — composicao, CNAE, inalienabilidade.
- `context/clausulas-padrao-holding.md` — blindagem (incomunicabilidade/impenhorabilidade/inalienabilidade), Golden Share, objeto/vedacoes, integralizacao.
- `context/itcmd-itbi-sucessao.md` — ITBI Tema 796, inalienabilidade sobre legitima.

## Quando ativa
Quando o diagnostico apontou patrimonio que o cliente quer **guardar** de qualquer atividade operacional. Se o patrimonio gera renda ativa (aluguel, cessao, carteira), a celula certa e a ADM de Bens (`celula-adm-de-bens`), nao a Cofre.

## 1. Parametros da celula (metodologia-4-celulas §2)
| Campo | Parametro |
|---|---|
| Funcao | Guarda e protecao **pura** do patrimonio imobilizado — nao opera, nao cede risco |
| Tipo | LTDA pluripessoal |
| Composicao | Socio patrimonial **98%** + socio operacional **2%** — **PF direto OU Participacoes-socia-2** (decisao guiada pela intencao, ver §1.1) |
| Administracao | **Conjunta** — ambos coadministradores |
| Golden Share | Socio **patrimonial** |
| Inalienabilidade | **15 anos** |
| CNAE principal | **6462-0/00** (holdings de instituicoes nao-financeiras) |

### 1.1 Os 2% da Cofre — decisao GUIADA (leve as duas opcoes ao cliente; ele decide pela intencao)
Nao ha default cego. As duas estruturas sao validas — a escolha e da intencao do cliente:

- **(A) 2% do socio operacional PF direto** — vantajoso quando **HA um socio PF "limpo"** (sem passivo, sem risco) que pode **participar da distribuicao de lucros ate ~R$ 50 mil/mes**, faixa em que o dividendo ainda e favoravel (abaixo do gatilho de IRRF 10% da Lei 15.270/2025). Os 2% em PF abrem uma **porta de retirada eficiente**. Na sequencia de producao (Gestora → Cofre → Participacoes → ADM) a Participacoes ainda nao existe na constituicao da Cofre — entao os 2% PF entram naturalmente ja na constituicao.
- **(B) 2% da Holding de Participacoes (socia-2) — fidelidade ao COFRE-TEMPLATE** — quando **NAO ha esse socio PF limpo** com retirada util, ou o objetivo e concentracao/controle e sucessao sem porta de dividendo em PF. Exige constituir a Participacoes **antes** da Cofre (sequencia alternativa) ou ceder as quotas da PF para a Participacoes depois — registrar em `sequencia-de-producao`.

**Regra pratica:** socio PF limpo com retirada util ate ~R$ 50k/mes → opcao **(A)**; caso contrario → opcao **(B)**, fiel ao template. **Apresente as duas e deixe o cliente decidir pela intencao** (retirada eficiente × concentracao/controle). **Socio unico:** detem 98%-100%; Golden Share e veto do proprio controlador (efeito pleno na sucessao).

## 2. Objeto social (o que a Cofre PODE)
Guarda, protecao, administracao e conservacao do patrimonio **proprio**: (a) propriedade/guarda/conservacao e cessao onerosa de uso de bens **proprios**; (b) participacao no capital de outras sociedades (holding pura — art. 2, §3, Lei 6.404/1976); (c) recebimento de alugueis, rendimentos e dividendos **proprios**; (d) gestao de aplicacoes e investimentos **proprios**. Sempre com **proposito negocial declarado** (organizacao patrimonial + sucessao + protecao) — afasta o art. 116, §unico, CTN.

## 3. Vedacoes ao objeto (o que a Cofre NUNCA)
Vedar expressamente: (a) qualquer atividade operacional, comercial ou industrial; (b) compra e venda de imoveis **de terceiros**, incorporacao, loteamento; (c) locacao de imoveis de terceiros; (d) **atividade imobiliaria preponderante** — preserva a imunidade de ITBI (CF 156, §2, I; **Tema 796 STF — RE 796.376/SC**); (e) participacao em operacionais de risco; (f) **aval, fianca ou garantia a terceiros** (vedacao ao aval cruzado — pressuposto contra a desconsideracao inversa, CC 1.015 §unico). Somar as vedacoes **setoriais** do risco do grupo.

## 4. Blindagem sobre as quotas (Cap. III — clausulas-padrao-holding)
- **Incomunicabilidade** — art. 1.911 + 1.668, I + 1.848 CC (nao se comunica ao conjuge, qualquer regime).
- **Impenhorabilidade** — art. 1.026, caput CC (credor pessoal alcanca so os frutos civis).
- **Inalienabilidade 15 anos** — contados do registro; salvo sucessao hereditaria.
- **Protecao especial das quotas de 2%** — paragrafo individualizado, incessiveis no prazo.
- **Golden Share ao patrimonial** — veto nas materias relevantes (alienacao/onerar, divida/garantia > alcada, alteracao de objeto/sede/capital, admissao/exclusao de socio, vinculo a operacional de risco). Prevalece sobre o quorum.
- **Administracao conjunta com alcadas** — gestao corrente isolada ate o teto; alienacao/divida/garantia exigem deliberacao. **Quem opera, assina; quem protege, veta.**

## 5. Integralizacao de imoveis na Cofre
Aumento de capital por integralizacao pelo **valor da DIRPF** do integralizador, **sem ganho de capital** (art. 23, Lei 9.249/1995), com **imunidade de ITBI** (Tema 796) **desde que**: (i) o valor integralizado nao ultrapasse o capital subscrito — **o excedente TRIBUTA** (limite honesto do Tema 796); e (ii) a sociedade nao tenha atividade imobiliaria preponderante. Detalhe e estrategia de quanto integralizar → `itbi-integralizacao` / `integralizacao-de-imoveis`.

## 6. Postura honesta
- A Cofre **organiza e protege — nao e muralha**. Impenhorabilidade contratual nao e absoluta: nao vence fraude contra credores, fraude a execucao, simulacao nem desconsideracao (CC 50); e o credor pessoal ainda alcanca os frutos (CC 1.026, caput).
- **Inalienabilidade que recai sobre a legitima** de herdeiro necessario exige **justa causa declarada** (CC 1.848), sob pena de nulidade — ver `itcmd-itbi-sucessao.md` e rotear `planejamento-sucessorio`.
- **Excedente de integralizacao sobre o capital nao e imune** de ITBI. Nunca prometer imunidade total.
- Nenhum dispositivo/aliquota entra sem estar no `context/`; o que nao confirmar, "a confirmar" → `validador-holding`.

## Cross-link (soft)
`celula-adm-de-bens` (a que opera/renda) · `celula-holding-participacoes` (a que controla operacionais) · `sequencia-de-producao` (ordem de registro) · `contrato-social-holding` (redige o instrumento) · `itbi-integralizacao` / `registro-jucesp-drei`.

## Fecha por
`suprema-corte-holding` R1 (estrutura/socios) + R4 (forma/registro) antes de virar contrato.
