# Reforma Tributária 2027 — Forward-Look para Holdings

> **CAMADA "MONITORAR / SINALIZAR" — NÃO É LEI DE HOJE.**
> Este documento descreve o que a Reforma Tributária do Consumo (EC 132/2023 + LC 214/2025, alterada pela LC 227/2026) **vai** mudar para holdings ao longo da transição **2026 → 2033**.
> **A lei VIGENTE de 2026 continua autoritativa** (lucro presumido, PIS/COFINS, ICMS/ISS, ITCMD estadual atual — ver `tributario-holding-2026.md` e `itcmd-itbi-sucessao.md`). O plugin aplica a lei de hoje; isto aqui é forward-look para o advogado avisar o cliente e tomar decisões que **envelheçam bem**. **Nenhum número de alíquota-teste/referência entra em peça como definitivo sem fonte oficial.**

---

## 0. TL;DR para o advogado de holding

1. **O IVA dual (IBS+CBS) alcança a locação de imóveis** — a holding patrimonial que vive de aluguel deixa de só pagar PIS/COFINS 3,65%; passa a ter IBS/CBS sobre a receita locatícia, **com redução de 70%** + redutor social nas residenciais.
2. **A transição é longa** (2026 teste → 2027 CBS cheia → 2029-2032 IBS gradual → 2033 pleno). Nada é "de uma vez".
3. **ITCMD vira progressivo obrigatório** (EC 132) — estados de alíquota fixa (SP 4%) terão de criar faixas; teto continua 8% (Senado), com debate de elevação. Doação de quotas e sucessão de alto valor ficam mais caras na ponta de cima.
4. **Split payment** recolhe IBS/CBS na hora da liquidação financeira (cartão/PIX/boleto) → mata o float de caixa do grupo e exige NF-e/NFS-e disciplinada, inclusive intragrupo e na locação.
5. **Decisão que envelhece bem:** estrutura societária, blindagem e sucessão **não dependem do regime de consumo** — montar a holding agora segue válido. **Decisão que envelhece mal:** vender "locação isenta/3,65% pra sempre" como argumento central; e adiar doação de quotas se o estado subir a alíquota / criar progressividade.

---

## 1. EC 132/2023 + LC 214/2025 — o IVA dual (IBS + CBS + IS)

| Novo tributo | Competência | Substitui / extingue | Base (EC 132) |
|---|---|---|---|
| **IBS** — Imposto sobre Bens e Serviços | Estados, DF e Municípios (gerido pelo Comitê Gestor do IBS) | **ICMS** + **ISS** | CF art. 156-A; Comitê art. 156-B |
| **CBS** — Contribuição sobre Bens e Serviços | União | **PIS/Pasep** + **COFINS** | CF art. 195, V |
| **IS** — Imposto Seletivo | União (extrafiscal) | assume a função reguladora do IPI (bens/serviços nocivos) | dispositivo de imposto seletivo da EC 132 |

O **IPI** não é formalmente extinto, mas tem alíquotas reduzidas a zero a partir de 2027 para quase tudo, preservado apenas para a Zona Franca de Manaus. Modelo: IVA dual (CBS federal + IBS subnacional) + IS, com não cumulatividade plena (crédito financeiro amplo).

### Cronograma de transição 2026 → 2033 (estrutura confirmada; alíquotas-teste em fonte didática — confirmar na resolução oficial)

| Ano | CBS | IBS | Tributos antigos |
|---|---|---|---|
| **2026** | Fase TESTE | Fase TESTE | PIS/COFINS/ICMS/ISS/IPI todos plenos (mandam) |
| **2027** | **alíquota cheia** | mantém teste | **PIS/COFINS extintos** · IPI a zero (exceto ZFM) · ICMS/ISS plenos |
| **2028** | cheia | teste | ICMS/ISS plenos |
| **2029-2032** | cheia | **rampa gradual** (sobe ~1/10 ao ano) | ICMS/ISS **decrescentes** na mesma proporção |
| **2033** | cheia | **PLENO** | **ICMS e ISS extintos** |

A alíquota de referência combinada IBS+CBS é estimada em ~26,5% a 28% (teto de referência fixado em lei) — número final só sai com as resoluções de calibragem; **não citar como definitivo**.

---

## 2. Impacto em HOLDING — regime específico de bens imóveis (LC 214/2025, arts. 251-270)

> Pergunta-chave do cliente: "Minha holding de aluguel vai pagar esse IVA?" **Resposta honesta: em regra, SIM — mas com regime favorecido e com filtro para PF.**

### 2.1 Locação/cessão de imóveis ENTRA no IBS/CBS
A LC 214/2025 criou um **regime específico de bens imóveis** (Cap. V, arts. 251-270). Entram no IVA dual: alienação/venda (inclusive incorporação e parcelamento do solo); **locação, cessão onerosa e arrendamento**; cessão/constituição de direitos reais; administração e intermediação. A locação não está fora do IVA — está **dentro, com tratamento favorecido**.

### 2.2 Reduções de alíquota — art. 261
| Operação | Redução IBS/CBS |
|---|---|
| Operações com imóveis em geral (venda, incorporação) | **−50%** das alíquotas |
| **Locação, cessão onerosa e arrendamento** | **−70%** das alíquotas |

> Correção de premissa comum: não é "70% na venda". O correto é **50% em geral / 70% em locação** (art. 261). Não inverter.

Cálculo ilustrativo da locação (estimativa — depende da alíquota de referência): alíquota cheia ~26,5% × (1 − 0,70) ≈ ~7,95% efetivos sobre a receita de locação. **Não prometer percentual fechado** enquanto a referência não for oficial.

### 2.3 Redutores
- **Redutor SOCIAL (art. 260):** abatimento fixo de **R$ 600,00 por imóvel** na **locação residencial**, atualizado pelo IPCA, deduzido da base até o limite dela.
- **Redutor de AJUSTE (art. 258, a partir de 01/01/2027):** vinculado ao imóvel do contribuinte, usado exclusivamente para reduzir a base na **alienação futura** do próprio bem (evita tributar ganho inflado / dupla incidência).

### 2.4 Filtro da PESSOA FÍSICA locadora — art. 251 §§1º e 2º (alterado pela LC 227/2026, verbatim)
A PF **só vira contribuinte** do regime regular (e só então a locação dela sofre IBS/CBS) se cruzar limites objetivos:
> **Art. 251. §1º** As pessoas físicas (...) serão consideradas contribuintes do regime regular (...) nos casos de:
> **I – locação, cessão onerosa e arrendamento de bem imóvel, desde que, no ano-calendário anterior:**
> **a)** a receita total com essas operações **exceda R$ 240.000** (duzentos e quarenta mil reais); **e**
> **b)** tenham por objeto **mais de 3 (três) bens imóveis distintos;**
> **§2º** Também será considerada contribuinte (...) **no próprio ano-calendário** (...): **II –** a locação (...) **em valor que exceda em 20% o limite previsto na alínea "a"** [= **R$ 288.000**].

Os dois requisitos do §1º são **cumulativos** (receita > R$ 240k **E** > 3 imóveis). **Ambiguidade relevante:** o §2º, II remete só ao limite de receita (R$ 288k), **sem repetir** o requisito dos 3 imóveis — abre brecha para enquadrar, no próprio ano, locador com menos de 3 imóveis que estoure R$ 288k. Tema **não pacificado** — avisar o cliente do risco.

### 2.5 Holding patrimonial de aluguel — "antes × depois"
| | HOJE (vigente 2026) | PÓS-REFORMA (regime pleno) |
|---|---|---|
| Natureza | PIS/COFINS cumulativo 3,65% sobre aluguel (presumido) + IRPJ/CSLL | IBS/CBS sobre o aluguel, **−70%** (art. 261) + redutor social residencial (art. 260); IRPJ/CSLL seguem |
| PF locadora | sem PIS/COFINS; só IRPF | só vira contribuinte IBS/CBS se > R$ 240k **e** > 3 imóveis (art. 251) |
| Veredito | carga conhecida, baixa sobre consumo | pode subir ou descer conforme alíquota de referência × redutor — **exige simulação caso a caso** |

> **Mensagem honesta:** a holding **continua fazendo sentido** por blindagem, governança e sucessão; mas o argumento "aluguel quase sem imposto pra sempre" vai mudar. A vantagem da PJ sobre a PF na locação **se estreita** quando o IVA dual entra — rodar simulação quando as alíquotas de referência saírem.

---

## 3. ITCMD na EC 132 — progressividade obrigatória e competência

> Atenção à vigência: a parte constitucional da EC 132 sobre ITCMD **já está em vigor** (promulgada 20/12/2023), mas depende de **lei estadual** adaptada e da LC nacional (PLP 108/2024) para eficácia plena. É o item da reforma que **mais cedo** afeta holding/sucessão.

- **Progressividade obrigatória (CF art. 155, §1º, VI):** "será progressivo em razão do valor do quinhão, do legado ou da doação." Antes era facultativa (SP = 4% fixo). Agora todos os estados terão de adotar faixas progressivas — alíquota linear fixa fica incompatível com a CF. **Teto continua 8%** (Resolução do Senado 9/1992; a EC 132 não mexeu nisso). Debate de elevação para 12%/16% depende de nova Resolução do Senado — **não vigente, não vender como certo**. Impacto: doação/sucessão de quotas de alto valor migra para a faixa de topo → transmitir o patrimônio fica mais caro na ponta de cima.
- **Elemento no exterior (EC 132, art. 16):** autoriza os estados a cobrar ITCMD sobre **doação de doador no exterior** e **herança de bens no exterior**, independentemente de LC prévia (até a LC nacional vir). Holding com ativos no exterior / offshore (LLC, imóveis lá fora) **passa a poder gerar ITCMD** na sucessão/doação — sinalizar na célula offshore.
- **Bens móveis/quotas — domicílio do de cujus:** quotas de holding = bens móveis → competência pelo **domicílio do falecido/doador** (não mais "local do inventário"). Importa para escolher onde domiciliar o titular das quotas.
- **Doação disfarçada:** distribuição desproporcional de lucros, redução de capital com entrega de bens e cessão gratuita de quotas podem ser requalificadas como **doação** (ITCMD) — agora com progressividade, o valor global transmitido pesa mais.

---

## 4. Split payment e nota fiscal — operacional para o grupo (LC 214/2025, arts. 31-35)

**Split payment:** na liquidação financeira da operação (cartão/PIX/boleto), o valor é dividido entre a parcela líquida do fornecedor e a parcela de **IBS/CBS**, recolhida automaticamente **antes** de o dinheiro chegar inteiro ao vendedor (arts. 31-35; art. 35 prevê a extinção do crédito tributário na liquidação + implantação gradual). Modalidades: inteligente/automático (transação eletrônica dispara a segregação) e simplificado (parametrização por percentuais, sobretudo B2C). A não cumulatividade plena tende a ficar condicionada ao recolhimento efetivo na etapa anterior — se o fornecedor não liquidou, o crédito do adquirente pode ser bloqueado (regulamentação infralegal ainda fechando).

**Impacto para holding / grupo:**
- **Fluxo de caixa:** o tributo deixa de "ficar na empresa até o mês seguinte" — recolhe na hora. **Mata o float** do grupo; a tesouraria replaneja o capital de giro.
- **Operações intragrupo** (serviços entre as células, reembolso, mútuos, locação intragrupo) exigem **NF-e/NFS-e disciplinada** — faturamento informal vira inconformidade que **trava crédito**.
- **Locação** dentro do IVA tende a exigir documento fiscal eletrônico — revisar ERP, cadastro e contratos de cada fluxo faturável.
- **Governança fiscal:** mapear CNPJs, centros de faturamento, contas de recebimento, PSPs, conciliação de recebíveis. Implantação gradual (testes 2026, operação 2027+).

---

## 5. O que avisar o cliente HOJE ao montar a holding pensando em 2027

### Decisões que ENVELHECEM BEM (fazer agora, valem independente da reforma)
1. **Constituir a holding agora** — a arquitetura societária (4 células, blindagem, Golden Share, incomunicabilidade/inalienabilidade, acordo de sócios, governança) não depende do regime de consumo.
2. **Antecipar doação de quotas com reserva de usufruto** — enquanto o estado tiver alíquota fixa (ex.: SP 4%) e antes de eventual elevação/progressividade plena, doar agora pode travar custo menor. Avaliar a janela estado a estado, respeitando a anterioridade.
3. **Imunidade de ITBI na integralização** (CF art. 156, §2º, I + Tema 796 STF) **segue vigente** — usar a integralização para subir imóveis à holding não é afetada pela reforma do consumo.
4. **Documentar e formalizar TUDO** (NF-e/NFS-e, contratos de locação, operações intragrupo) — o split payment e a não cumulatividade condicionada **punem informalidade**.

### Decisões que ENVELHECEM MAL (evitar / não prometer)
1. Vender "aluguel quase isento pra sempre" como argumento central — o IVA dual vai alcançar a locação (−70%, mas não zero).
2. Prometer percentual fechado de carga — a alíquota de referência (~26,5-28%) ainda não é oficial.
3. Adiar sucessão/doação indefinidamente apostando que "nada muda" — a progressividade do ITCMD já é norma constitucional; estados estão adaptando leis; o teto pode subir.
4. Estruturar distribuição desproporcional / cessão gratuita de quotas sem cuidado — risco de requalificação como doação (ITCMD progressivo).
5. Ignorar a ponta exterior — holding com offshore/ativos no exterior agora pode gerar ITCMD (EC 132, art. 16).

### Frase-guia do plugin (R-HOLDING)
> "A lei vigente de 2026 é a que vale hoje e é a que aplico. A Reforma Tributária (EC 132 + LC 214/2025) é forward-look: monto a estrutura para que ela sobreviva à transição 2026-2033, sinalizo o que vai mudar (locação no IVA, ITCMD progressivo, split payment) e recalibro quando as alíquotas de referência forem oficializadas. Nenhum número de alíquota-teste/referência entra em peça como definitivo sem fonte oficial."
