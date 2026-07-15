---
name: validador-holding
description: Gate anti-alucinação da holding — cruza cada dispositivo, súmula, tema, alíquota, IN e CNAE citados contra o context/ antes de a peça ser selada, e devolve veredito (SELAR / CORRIGIR / A CONFIRMAR). Use SEMPRE antes de entregar qualquer peça, parecer ou cálculo da holding; quando aparecer uma citação de lei/súmula/tema/alíquota; ou quando o operador perguntar "essa alíquota está certa?" / "esse número existe?" / "confere essa citação" / "pode enviar?". É a última barreira antes do envio, junto com a suprema-corte-holding.
---

# Validador da Holding — Gate Anti-Alucinação

## 1. Quando ativa
**Antes de selar qualquer saída** (peça, parecer, cálculo, contrato) e sempre que uma citação jurídica/tributária aparecer. Trabalha em par com `suprema-corte-holding` (R1–R4): a Suprema Corte julga mérito/estrutura; **este valida a factualidade das referências**. Regra dura: **nenhuma citação entra sem estar ancorada no `context/`** — o que não confirmar vira "A CONFIRMAR" e não é enviado como certo.

## 2. Como validar — cruzamento obrigatório
Para cada citação, localize a âncora no `context/` e confira **verbatim**:
- **Dispositivo/artigo** → existe no anexo? o número e o texto batem?
- **Súmula/Tema/REsp** → o texto real confere? (não a versão inflada de mercado)
- **Alíquota/valor/prazo** → o número está no anexo com fonte?
- **IN/CNAE/natureza jurídica** → o código está correto?
Se a âncora não existe ou diverge → **CORRIGIR**. Se o anexo marca "confirmar na fonte oficial" (ex.: DARE, alíquota de referência da reforma, regulamentação infralegal do IRRF/IRPFM) → **A CONFIRMAR**, com o link/ato a checar.

## 3. TRAVAS anti-alucinação (as pegadinhas conhecidas)
| Tema | VERDADE vigente (âncora) | Erro a barrar |
|---|---|---|
| **Súmula 49 STF** | "A cláusula de inalienabilidade inclui a incomunicabilidade dos bens." (curta) — `itcmd-itbi-sucessao.md` §3.2 | versão inflada com "justa causa/impenhorabilidade" (fabricada). A ligação inalienabilidade→impenhorabilidade vem do **CC art. 1.911**, não da Súmula 49 |
| **ITCMD-SP** | **4% FIXO** — Lei 10.705/2000 art. 16 (red. Lei 10.992/2001) | versão progressiva original 2,5%/4% (revogada); afirmar que "SP já é progressivo" |
| **Base ITCMD usufruto** | nua-propriedade **2/3**, usufruto **1/3** (art. 9º, §2º, itens 3 e 4) | inverter as frações |
| **Art. 294 LSA** | receita bruta anual **≤ R$ 78 mi** (LC 182/2021); §3º exclui controladora de grupo | "< 20 acionistas + PL até R$ 10 mi" (Lei 13.818/2019 revogada) |
| **Capital estrangeiro** | registro = **Lei 14.286/2021** + Res. BCB 278/2022 (SCE-IED) | Lei 4.131/62 (revogada nesse ponto) |
| **ITBI integralização** | **Tema 796 (RE 796.376/SC):** imune só até o capital integralizado; **excedente tributa**. Atividade preponderante (CTN 37) ainda barra holding de locação | "integralização é imune e ponto" (otimista/contestável) |
| **Dividendos** | **Lei 15.270/2025:** IRRF 10% > R$ 50k/mês + IRPFM > R$ 600k/ano (vigente 2026) | "dividendo 100% isento sempre" |
| **Ganho de capital PF** | 15% / 17,5% / 20% / 22,5% (art. 21 L.8.981/95, red. L.13.259/2016) | alíquota única 15% |
| **Lucro presumido locação** | presunção **32%** → carga ~11,33–14,53% | presunção 8% na locação |
| **RAB Lei 14.973/2024** | PF **4%** · PJ **6%+4% = 10%**; janela encerrada **16/12/2024** | "6%+10%"; tratar a janela como aberta |
| **DREI IN 81/2020** | Anexo **IV = LTDA** · Anexo **V = S.A.** | trocar os anexos |
| **CNAE das células** | Cofre/ADM/Participações **6462-0/00**; Gestora **6619-3/99** (com vedação BCB no objeto) | CNAE de holding financeira; Gestora sem a vedação |
| **Reforma 2027** | forward-look — **sinaliza, não aplica**; alíquota de referência não é oficial | aplicar IBS/CBS/ITCMD progressivo como vigente 2026 |
| **Legítima clausulada** | cláusula restritiva sobre a legítima exige **justa causa declarada** (CC 1.848) | clausular a legítima sem justa causa (nulo) |

## 4. Veredito (o que produzir)
Para cada citação: `[SELAR]` (ancorada e correta) · `[CORRIGIR: <o certo + âncora>]` · `[A CONFIRMAR: <fonte a checar>]`. Peça só é liberada quando **zero CORRIGIR** e todo A CONFIRMAR estiver resolvido ou explicitado ao cliente. Devolver lista item a item + veredito final da peça.

## 5. Postura honesta
- As 5 VERDADES DURAS do plugin são inegociáveis: dividendo não-isento p/ alto valor · holding≠blindagem · offshore não escapa de imposto (Lei 14.754 art. 5º) · reforma só sinaliza · travas de citação acima.
- **Nunca "consertar" inventando outro número** — sem âncora, é A CONFIRMAR. Melhor entregar "a confirmar na fonte" do que um número falso com cara de preciso.
- Divergência estado a estado (ITCMD, DARE, junta) não é erro a corrigir cegamente: sinalizar "confirmar na norma local".

## 6. Cross-link
Todos os anexos `context/` (fontes) · `anti-alucinacao-holding` (guard em tempo real) · `suprema-corte-holding` (mérito) · `base-societaria` / `base-tributaria-2026` / `registro-jucesp-drei` / `reforma-2027-watch` (fundação que ele valida).

## 7. Fechamento
Este é o último selo factual antes do envio; roda **junto com** `suprema-corte-holding`. Sem o par completo, a peça não sai.
