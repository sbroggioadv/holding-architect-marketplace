---
name: base-societaria
description: Fundação societária da holding — Código Civil (sociedades) + Lei 6.404/76 (LTDA × S.A.), regência supletiva e quando cada tipo compensa. Use ao escolher o tipo societário da holding, comparar LTDA e S.A. fechada, avaliar acordo de sócios/acionistas, governança (conselho, diretoria), classes de ações, voto plural, sigilo do quadro, publicações e livros — ou quando o cliente perguntar "holding tem que ser S.A.?" / "LTDA ou S.A.?" / "preciso de conselho de administração?".
---

# Base Societária — LTDA × S.A. na Holding

## 1. Quando ativa
Sempre que a estrutura precisar decidir **tipo societário** de qualquer das 4 células ou da holding-mãe, comparar LTDA × S.A. fechada, ou dimensionar governança (conselho, diretoria, acordo de sócios, classes de ações). Alimenta `celula-*`, `contrato-social-holding`, `estatuto-e-atos-sa` e `acordo-de-socios`.

## 2. Base legal ancorada (`societario-jucesp-sa.md`)
**LTDA** — CC arts. 1.052–1.087. Regência supletiva pela LSA **só se o contrato previr** (art. 1.053, parágrafo único). Integralização de imóveis: não exige laudo, mas os sócios respondem solidariamente pela exata estimação por **5 anos** (art. 1.055, §1º). Dispensa escritura pública para levar o imóvel ao capital (o ato societário registrado é o título).

**S.A. fechada** — Lei 6.404/76 integral; holding = **companhia de participação** (art. 2º, §3º).
- Constituição por **subscrição particular** (art. 88) — não a pública (art. 82), antieconômica p/ família. Requisitos preliminares: art. 80 (subscrição por ≥ 2 pessoas; **10% mínimo em dinheiro** do preço de emissão das ações subscritas em dinheiro; depósito bancário — arts. 80/81).
- **Art. 89:** incorporação de imóveis ao capital **não exige escritura pública**. Avaliação de bens = **laudo de 3 peritos ou empresa especializada** (arts. 8º–10), aprovado em assembleia.
- Espécies de ações (**art. 15**): ON, PN (PN sem voto ≤ 50% do total — art. 15, §2º) e de fruição. **Voto plural — art. 110-A** (até 10 votos por ação ordinária, prazo limitado; pós-Lei 14.195/2021) = instrumento de controle sucessório.
- **Acordo de acionistas — art. 118:** arquivado na sede é oponível à companhia; averbação nos livros/certificados; **execução específica** (§3º); o presidente **não computa** voto proferido com infração (§8º). Disciplina legal própria, superior ao acordo de quotistas da LTDA (que só tem esse aparato se houver regência supletiva LSA — art. 1.053, §ú).
- Órgãos: **AGO nos 4 primeiros meses** (art. 132); **Conselho de Administração** obrigatório só em cia. aberta, de capital autorizado e economia mista (art. 138, §2º) — holding fechada **pode operar só com Diretoria**; **diretor único** admitido pela **LC 182/2021** (art. 143); Conselho Fiscal de funcionamento não-permanente (art. 161).
- **Livros — art. 100** (Registro/Transferência de Ações Nominativas etc.), físicos ou eletrônicos.
- **Publicações/dispensa — art. 294 (LC 182/2021):** a cia. fechada com **receita bruta anual ≤ R$ 78.000.000,00** pode publicar de forma eletrônica (III) e substituir livros por registros eletrônicos (IV). **§3º:** NÃO se aplica à **companhia controladora de grupo** e filiadas → holding controladora avalia caso a caso.
> **Trava:** o critério do art. 294 é **receita ≤ R$ 78 mi** (não "< 20 acionistas + PL até R$ 10 mi" — redação revogada da Lei 13.818/2019).

## 3. Decisão — quando cada tipo (regra geral: LTDA basta e é mais barata)
**S.A. fechada compensa quando** (`societario-jucesp-sa.md` §4): acordo de acionistas robusto (art. 118) > acordo de quotistas · Conselho de Administração separando propriedade/gestão · classes ON/PN + voto plural (engenharia sucessória fina) · **sigilo do quadro** (transferência de ações lançada em livro interno, não vai à junta a cada negócio) · captação/family office · patrimônio elevado + muitas operacionais + muitos herdeiros com conflito potencial.

**LTDA é melhor quando:** poucos imóveis/participações passivas, quadro pequeno, família coesa, sem investidor externo, foco em custo baixo. A LTDA já permite **golden share, administração conjunta, tag along, inalienabilidade temporária e apuração de haveres por cláusula** (validado pela JUCESP) — cobre boa parte da governança sem o custo da S.A.

**Não há diferença tributária relevante S.A. × LTDA só pela forma.** Migrar LTDA→S.A. vale quando os critérios da S.A. passam a pesar mais que o custo recorrente (livros, AGO, eventuais publicações).

Produzir: recomendação de tipo por célula + justificativa ancorada + o que a escolha destrava/custa.

## 4. Postura honesta (verdades duras)
- **Holding NÃO é blindagem** — a forma societária organiza e protege, mas não afasta legítima (CC 1.846/1.848), fraude (CC 158/167) nem desconsideração (CC 50). Ver `itcmd-itbi-sucessao.md` §6.
- Vender "S.A. é mais blindada que LTDA" é folclore: a proteção vem da **substância** (gestão real, contabilidade, separação de contas), não do tipo.
- Nenhum dispositivo entra em peça sem estar no `context/`; número "de memória" vira "a confirmar" → `validador-holding`.

## 5. Cross-link
`societario-jucesp-sa.md` (fonte) · `registro-jucesp-drei` (protocolo) · `celula-*` (aplicação) · `acordo-de-socios` · `estatuto-e-atos-sa` · plugin-mãe `tributario-societario-adv-os` (societário geral).

## 6. Fechamento
Toda peça que nasça desta base fecha por **`suprema-corte-holding`** (R1 estrutura · R4 forma/registro) + **`validador-holding`** antes de selar.
