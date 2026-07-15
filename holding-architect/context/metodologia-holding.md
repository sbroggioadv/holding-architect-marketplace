# Metodologia do Holding Architect

Anexo-mestre do plugin. Define o que o produto faz, o ciclo de trabalho, as premissas invioláveis e o regime anti-alucinação. Os demais anexos de `context/` são a fundação de conhecimento que as skills consultam em runtime.

---

## 1. O que o plugin faz

O Holding Architect é o sistema operacional do advogado que estrutura **holdings patrimoniais e familiares brasileiras** — da arquitetura societária ao registro na junta, passando por tributação, sucessão, governança e a ponta brasileira do investimento estrangeiro (offshore).

Cobre, de ponta a ponta:
- **Estrutura societária** — o método das 4 células (Cofre, ADM de Bens, Holding de Participações, Gestora), variações e sequência de produção.
- **Documentos** — contrato social, alteração contratual, integralização de imóveis, acordo de sócios/acionistas, protocolo familiar, estatuto e atos da S.A.
- **Tributário-sucessório** — integralização (custo × mercado), ITBI (imunidade + Tema 796), ITCMD (doação de quotas com usufruto), ganho de capital, atualização de bens (Lei 14.973/2024), dividendos pós-Lei 15.270/2025, legítima/colação, apuração de haveres.
- **Offshore — ponta BR** — apostilamento, CNPJ da estrangeira (IN RFB 2.119/2022), registro do investimento no BCB (SCE-IED, Lei 14.286/2021), entrada da estrangeira como sócia + panorama fiscal das jurisdições.
- **Governança e registro** — conselhos, acordo de sócios, planejamento sucessório, roteiro JUCESP/DREI, ciclo da S.A.

**Fronteira de escopo:** o plugin **não faz a abertura da empresa no exterior** (constituição da LLC/Corp lá fora) — isso é parceiro in loco. Domina a ponta brasileira até o talo + panorama fiscal comparativo para o cliente decidir onde abrir.

---

## 2. Mapa dos anexos de conhecimento (`context/`)

| Anexo | Conteúdo |
|---|---|
| `metodologia-4-celulas.md` | Arquitetura das 4 células, CNAEs, Golden Share, inalienabilidade, fluxos de proteção e lucros, sequência de produção, variações |
| `clausulas-padrao-holding.md` | Biblioteca de cláusulas-modelo (objeto, blindagem, administração, Golden Share, tag along, apuração de haveres, inter-PJ, integralização) |
| `societario-jucesp-sa.md` | Roteiro JUCESP, IN DREI 81/2020, ciclo da S.A. (Lei 6.404), comparativo S.A. × LTDA |
| `tributario-holding-2026.md` | Tributação vigente: integralização, Lei 14.973/2024, Lei 14.754/2023, dividendos (Lei 15.270/2025), lucro presumido, limites |
| `itcmd-itbi-sucessao.md` | ITBI (Tema 796), ITCMD-SP, doação com usufruto, cláusulas restritivas, legítima/colação, registro, apuração de haveres, limites da holding |
| `offshore-ponta-br.md` | Apostila, CNPJ estrangeira, SCE-IED, sócia estrangeira, Lei 14.754 art. 5º, panorama Delaware/Wyoming/Paraguai/Uruguai/Dubai |
| `reforma-2027-watch.md` | Forward-look: IBS/CBS/IS, locação no IVA, ITCMD progressivo, split payment, transição 2026→2033 |

---

## 3. Ciclo de trabalho (a "esteira")

```
1. DIAGNÓSTICO        ──► quem é o sócio patrimonial × operacional; patrimônio;
                          setor de risco; regime de bens; herdeiros; sede;
                          objetivo (proteção / renda / sucessão / offshore)
        │
2. ESTRUTURA          ──► escolher e dimensionar as células (4 células ou subset);
                          variação (sócio único / família ampla / alto risco);
                          decidir LTDA × S.A.
        │
3. DOCUMENTOS         ──► montar contratos na sequência Gestora → Cofre →
                          Participações → ADM (alteração); aplicar a biblioteca
                          de cláusulas; campos pendentes marcados até o registro
        │
4. TRIBUTÁRIO-        ──► integralização custo × mercado; ITBI (Tema 796);
   SUCESSÓRIO             doação de quotas com usufruto e ITCMD; legítima/colação;
                          recalcular a economia com dividendos (Lei 15.270)
        │
5. OFFSHORE (se há)   ──► ponta BR: apostila → CNPJ estrangeira → SCE-IED →
                          sócia estrangeira; panorama fiscal; Lei 14.754
        │
6. GOVERNANÇA         ──► acordo de sócios; protocolo familiar; conselhos;
                          usufruto (voto + frutos); deadlock só em 50/50
        │
7. REGISTRO JUCESP    ──► viabilidade → DBE → DARE → assinatura digital →
                          protocolo → cumprimento de exigência → CNPJ
```

A esteira não é rígida: muitos casos param em algumas etapas. O diagnóstico define quais células e quais frentes entram.

---

## 4. Premissas invioláveis

1. **A lei VIGENTE de 2026 manda.** A Reforma Tributária (EC 132/2023 + LC 214/2025) é **forward-look** — sinaliza o que vai mudar, nunca se aplica como lei de hoje. Nenhum número de alíquota-teste/referência da reforma entra em peça como definitivo.
2. **Dividendos NÃO são mais sempre isentos.** A **Lei 15.270/2025** instituiu IRRF de 10% sobre dividendos a PF acima de R$ 50 mil/mês e o IRPFM para rendimentos > R$ 600 mil/ano. A isenção inter-PJ (art. 10, Lei 9.249/95) segue; o impacto é na saída para a pessoa física. Recalcular a economia caso a caso. Nunca afirmar "dividendo é 100% isento, sempre".
3. **A holding NÃO é blindagem absoluta.** Ela não afasta a legítima, não escapa da colação, não vence fraude contra credores / fraude à execução, não impede a desconsideração da personalidade jurídica, não sobrevive à simulação. O divisor legítimo × abusivo é **tempestividade** (antes da dívida) + **substância** (gestão e contabilidade reais) + respeito à legítima.
4. **Offshore não é "não pagar imposto".** A Lei 14.754/2023 fechou o diferimento: holding offshore de renda passiva (só participações/dividendos) é tributada a 15%/ano no Brasil, em 31/12, independentemente de distribuição — **mesmo em Delaware**. A offshore serve a privacidade, proteção, moeda forte, acesso a mercados e sucessão, não a economia de imposto por acúmulo.
5. **Quem opera, assina.** Administração conjunta com divisão de alçadas; Golden Share com o sócio patrimonial (não o operacional). Excluir o operador da gestão cria risco de administrador de fato + simulação.
6. **Substância documentada.** A holding precisa fazer algo (administrar, contratar, ter contabilidade e fluxo real) e ter propósito documentado (contrato social, atas, governança). Sem isso, é envelope vazio = autuação.
7. **Variação por estado declarada.** JUCESP é a base; em outro estado, confirmar exigências, prazos e taxas na junta local. ITCMD é estadual (SP = 4% fixo hoje).

---

## 5. Porta única e auditoria

**Orquestrador `holding-master`:** toda entrada passa por uma porta única que faz o diagnóstico, classifica o caso (qual estrutura, quais frentes), dirime as skills e dispara a esteira. Não se redige documento antes do diagnóstico estar completo — perguntar antes de supor; nenhuma suposição silenciosa.

**Suprema Corte (R1-R4):** auditoria de excelência sobre o que sai — coerência da estrutura, fundamento legal de cada cláusula, conformidade com a lei vigente, e o pente fino anti-alucinação antes da entrega.

---

## 6. Anti-alucinação (R-HOLDING)

- **Nenhum dispositivo, tese, súmula, IN, alíquota, CNAE ou prazo entra sem fonte.** Citações legais verbatim. Variação por estado declarada.
- **Fatos-âncora que a IA tende a errar (corrigir sempre):**
  - **Súmula 49 STF** é a CURTA: *"A cláusula de inalienabilidade inclui a incomunicabilidade dos bens."* A versão inflada (com "justa causa... impenhorabilidade...") é fabricada. A ligação inalienabilidade→impenhorabilidade vem do **CC art. 1.911**.
  - **ITCMD-SP = 4% FIXO** (Lei 10.992/2001). A versão progressiva original (2,5%/4%) foi revogada. Progressividade é tendência (EC 132), não lei vigente em SP.
  - **Dividendos não são mais sempre isentos** (Lei 15.270/2025).
  - **Art. 294 da Lei 6.404** vigente = receita ≤ R$ 78 milhões (LC 182/2021); o §3º exclui a controladora de grupo. Não usar o critério antigo "20 acionistas + PL R$ 10 mi".
  - **IN DREI 81/2020:** Anexo IV = LTDA, Anexo V = S.A. (Anexo II = EI).
  - **Diretoria da S.A. pode ser unipessoal** (art. 143, LC 182/2021).
  - **Registro do investimento estrangeiro** = Lei 14.286/2021 + Res. BCB 278/2022 (SCE-IED), não Lei 4.131/62 (residual).
  - **Tema 796 STF:** a imunidade de ITBI só não alcança o excedente do capital; afirmar que "holding imobiliária é imune e ponto" é contestável (atividade preponderante; obiter dictum).
  - **EAU é paraíso fiscal** (IN RFB 1.037/2010); EUA não.
- **Postura honesta obrigatória:** declarar limites (holding não é blindagem; imunidade de ITBI contestada na locação; consolidação de usufruto pode gerar ITCMD; cláusula de valor contábil revisável se aviltante). Não vender certeza onde há controvérsia.
- **Despersonalizado:** o plugin é genérico; cada advogado-cliente configura o próprio escritório. Os modelos do operador alimentam **metodologia e cláusulas-padrão** — nunca dados de cliente real.
