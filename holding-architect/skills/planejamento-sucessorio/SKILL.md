---
name: planejamento-sucessorio
description: "Desenha a sucessao patrimonial pela holding e a compara com o inventario, respeitando os limites que a lei impoe: legitima dos herdeiros necessarios (CC 1.789/1.845/1.846), doacao como adiantamento de legitima e colacao (CC 544/2.002/2.004), nulidade do que exceder a parte disponivel (CC 549), partilha em vida (CC 2.018), vedacao do pacto sucessorio (CC 426) e testamento. Entrega com honestidade obrigatoria: a holding organiza e antecipa, mas NAO afasta a legitima, a colacao, a fraude contra credores/execucao, a desconsideracao ou a simulacao. Use quando o operador disser 'planejamento sucessorio', 'holding x inventario', 'evitar inventario', 'legitima dos filhos', 'parte disponivel', 'partilha em vida', 'testamento', 'doacao desigual entre herdeiros', 'a holding blinda a heranca', 'deserdar por holding'."
---

# Planejamento Sucessorio pela Holding (com limites honestos)

> A holding **antecipa e organiza** a sucessao (doacao de quotas em vida, governanca, continuidade sem dissolucao) e reduz o custo/tempo do inventario sobre os bens que ela detem. O que ela **nao faz**: afastar a legitima, a colacao, a fraude ou a desconsideracao. O produto vende a verdade.

## Anexo obrigatorio (context/)
- `context/itcmd-itbi-sucessao.md` — **§4.2 legitima/colacao (CC 1.789/1.845/1.846/544/549/2.018/2.002/2.004) · §6 LIMITES (o que a holding NAO faz — CC 549/544/158-165/CPC 792 IV/CC 50/167)**. `grep -niE "1.789|1.846|1.848|544|549|colacao|2.002|legitima|fraude|desconsidera"`.
- `context/clausulas-padrao-holding.md` — §8 continuidade (herança das quotas, CC 1.028).

## Quando ativa
- O objetivo do caso e organizar quem fica com o que na sucessao, comparar com inventario, testar limites.
- Gatilhos: "planejamento sucessorio", "holding x inventario", "evitar inventario", "legitima", "parte disponivel", "partilha em vida", "testamento", "doacao desigual".

## Base tecnica ancorada

### 1. Legitima e limites da doacao (verbatim) *(§4.2)*
> **CC 1.789:** "Havendo herdeiros necessarios, o testador so podera dispor da metade da heranca."
> **CC 1.845:** herdeiros necessarios = descendentes, ascendentes e conjuge.
> **CC 1.846:** a metade dos bens da heranca pertence aos herdeiros necessarios de pleno direito = **legitima**.
> **CC 544:** doacao de ascendente a descendente (ou de um conjuge a outro) importa **adiantamento** do que cabe por heranca.
> **CC 549:** e **nula** a doacao quanto a parte que exceder o que o doador poderia dispor em testamento no momento da liberalidade.
> **CC 2.018:** valida a partilha feita por ascendente, por ato entre vivos ou de ultima vontade, desde que **nao prejudique a legitima**.

### 2. Colacao (verbatim) *(§4.2)*
> **CC 2.002:** os descendentes que concorrem a sucessao devem **conferir o valor das doacoes** recebidas em vida, para igualar as legitimas, sob pena de sonegacao (par. unico: computado na parte indisponivel, sem aumentar a disponivel).
> **CC 2.004:** o valor de colacao e o atribuido no ato de liberalidade.
> **Diretriz:** doacao **igual** a todos os filhos neutraliza a colacao. Doacao **desigual** (mais quotas/Golden Share a um) exige **imputacao a parte disponivel com dispensa expressa de colacao** (CC 2.005/2.006), senao o preterido exige igualacao. Perguntar sempre: "doacao igual ou desigual entre herdeiros?".

### 3. Vedacao do pacto sucessorio
> **CC 426:** nao pode ser objeto de contrato a heranca de pessoa viva. Instrumentos que disponham sobre sucessao futura de herdeiro vivo sao nulos — a estrutura opera por **doacao em vida** (com usufruto) + **testamento** (parte disponivel) + **partilha em vida** (CC 2.018), nunca por pacto sobre heranca futura.

### 4. Holding x inventario (o desenho)
- **Via holding:** integraliza os bens na PJ → doa a nua-propriedade das quotas com reserva de usufruto (cross-link `doacao-quotas-usufruto`) → na morte, consolida-se a propriedade no nu-proprietario (ja titular), em regra sem novo inventario sobre aqueles bens; a holding **nao se dissolve** (CC 1.028, §8 do anexo de clausulas).
- **Via inventario:** os bens do falecido passam por partilha judicial/extrajudicial + ITCMD sobre o acervo; mais lento e custoso.
- **Ganho real:** antecipacao ordenada, governanca, continuidade e potencial economia de tempo/custo — **desde que a doacao respeite a legitima**. As quotas nao doadas em vida ainda integram a sucessao.
- **Testamento:** complementa a estrutura para a **parte disponivel** (metade) e para clausulas sobre ela.

## O que produzir
1. **Mapa dos herdeiros necessarios** e do acervo (cross-link `mapa-patrimonial`): quem sao, regime de bens, o que ja foi doado.
2. **Perguntar (botoes `AskUserQuestion`):** doacao igual ou desigual? · quer reservar usufruto? · ha parte disponivel a destinar por testamento? · algum herdeiro precisa de protecao especial (justa causa)?
3. **Plano sucessorio:** sequencia de doacoes de quotas (com usufruto), imputacao a legitima/disponivel, dispensa de colacao quando desigual, testamento da parte disponivel, clausulas restritivas (com justa causa quando tocar a legitima — `doacao-quotas-usufruto`).
4. **Comparativo holding x inventario** para o caso concreto (custo, tempo, ITCMD, controle).

## Postura honesta (o §6 — o que a holding NAO faz) *(§6)*
A holding **nao**:
1. **Afasta a LEGITIMA** — doacao que a invada e nula no excedente (CC 549). Nao serve para "deserdar por via transversa".
2. **Escapa da COLACAO** — doacao de quotas a descendente = adiantamento (CC 544/2.002-2.004); o preterido exige igualacao, salvo dispensa imputada a disponivel.
3. **Vence FRAUDE CONTRA CREDORES** (CC 158-165, acao pauliana) — holding integralizada apos divida preexistente, gerando insolvencia, e anulavel.
4. **Vence FRAUDE A EXECUCAO** (CPC 792, IV) — alienacao/oneracao apos citacao capaz de gerar insolvencia = ineficaz perante o credor.
5. **Impede DESCONSIDERACAO** (CC 50, red. Lei 13.874/2019) — desvio de finalidade ou confusao patrimonial autorizam desconsiderar a PJ.
6. **Sobrevive a SIMULACAO** (CC 167) — holding "de papel", integralizacao artificial, doacao aparente sem transferencia real = nula.
> **Divisor agua legitimo x abusivo:** **tempestividade** (antes de dividas/litigios relevantes) + **substancia economica** (gestao real, contabilidade, ITCMD pago, avaliacao nao artificial) + respeito a legitima. Holding "de gaveta" e alvo facil.
- **EC 132/2023** (ITCMD progressivo obrigatorio, teto 8%) so **sinaliza** — SP segue 4% fixo hoje; usar como janela para antecipar. `reforma-2027-watch`.

## Cross-link
`doacao-quotas-usufruto` (execucao da antecipacao) · `mapa-patrimonial` (levantamento) · `protocolo-familiar` (governanca) · `apuracao-de-haveres` (saida do herdeiro) · plugin `civel-adv-os` (inventario judicial, sucessoes).

## Guard
Legitima intocavel (CC 549); doacao desigual sem imputacao/dispensa = igualacao. Pacto sucessorio vedado (CC 426). Holding nao e blindagem — sempre o §6. ITCMD-SP 4% fixo; progressividade so sinaliza. Nenhum dispositivo sem `validador-holding`. Entrega fecha pela `suprema-corte-holding`.
