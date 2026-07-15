---
name: itbi-integralizacao
description: "Faz a analise tributaria da imunidade de ITBI na integralizacao de imoveis no capital da holding — com a postura HONESTA que blinda o cliente: Tema 796 STF (RE 796.376/SC, imunidade so ate o capital integralizado; o excedente tributa), a excecao da atividade preponderante (CTN 37, >50% da receita em locacao/compra-venda), e o trade-off de QUANTO integralizar (mais capital = mais faixa imune de ITBI, porem mais ganho de capital se a mercado — art. 23 Lei 9.249/95). Use quando o operador disser 'integralizar imovel na holding', 'ITBI da integralizacao', 'a holding e imune de ITBI', 'Tema 796', 'atividade preponderante', 'quanto de capital colocar no imovel', 'holding de aluguel paga ITBI', 'excedente do capital', 'valor venal do imovel'. Analise; o documento/registro fino e da integralizacao-de-imoveis."
---

# ITBI na Integralizacao de Imoveis (imunidade e seus limites — postura honesta)

> A imunidade de ITBI na integralizacao e um dos motores da holding — mas **nao e "imune e ponto"**. Esta skill faz a **analise fiscal**: quanto e imune, quanto pode ser cobrado, e como calibrar o capital. O ato societario e o registro na matricula ficam em `integralizacao-de-imoveis` (C3).

## Anexo obrigatorio (context/)
- `context/itcmd-itbi-sucessao.md` — **§1 ITBI: dispositivo (CF 156, II e §2º, I), Tema 796 (RE 796.376/SC), excedente, excecao da atividade preponderante (CTN 37), postura honesta, registro LRP 167 I item 32**. `grep -niE "796|156|preponderante|CTN|excedente|imunidade"`.
- `context/tributario-holding-2026.md` — **§1** (interacao com o ganho de capital do art. 23 Lei 9.249/95).

## Quando ativa
- Ha imovel para colocar no capital da holding e a pergunta e sobre ITBI / quanto integralizar.
- Gatilhos: "integralizar imovel", "ITBI da integralizacao", "a holding e imune", "Tema 796", "atividade preponderante", "quanto de capital no imovel", "excedente do capital".

## Base tecnica ancorada

### 1. A imunidade (CF art. 156, II e §2º, I) *(§1.1)*
Nao incide ITBI sobre a transmissao de bens **incorporados ao patrimonio de PJ em realizacao de capital**, nem em fusao/incorporacao/cisao/extincao, **salvo se, nesses casos, a atividade preponderante do adquirente** for compra e venda desses bens, locacao de imoveis ou arrendamento mercantil.

### 2. Tema 796 STF — RE 796.376/SC (tese vinculante, verbatim) *(§1.2)*
> "A imunidade em relacao ao ITBI, prevista no inciso I do §2º do art. 156 da Constituicao Federal, **nao alcanca o valor dos bens que exceder o limite do capital social a ser integralizado**."
- **Mecanica do excedente:** a imunidade cobre so a parcela do valor do imovel correspondente ao **capital efetivamente integralizado**; o que exceder e **fato gerador de ITBI** (recolhido ao municipio). Ex.: imovel R$ 1.000.000, capital integralizado R$ 600.000 → imune sobre R$ 600.000, **ITBI sobre R$ 400.000**. A base do excedente pode usar valor venal/de referencia do municipio (confirmar na lei municipal).

### 3. Excecao da atividade preponderante (CTN art. 37) — HONESTA *(§1.3)*
- **Preponderante** = **mais de 50% da receita operacional** nos **2 anos anteriores e 2 subsequentes** a aquisicao (§1º); PJ com menos de 2 anos → apura-se nos **3 primeiros anos seguintes** (§2º).
- **Dois planos que nao se confundem:**
  - **Tese vinculante (Tema 796):** SO que a imunidade nao alcanca o excedente do capital. Nada alem disso e tese obrigatoria.
  - **Obiter dictum:** no voto condutor o STF afirmou que a imunidade da **1ª parte** do art. 156, §2º, I (realizacao de capital) seria **incondicionada** — a ressalva da preponderancia alcancaria so fusao/incorporacao/cisao/extincao. **MAS** o TJSP trata isso como **obiter, nao como tese**, e segue aplicando o teste de preponderancia tambem a integralizacao; fiscos municipais (SP e outros) continuam exigindo prova de ausencia de preponderancia imobiliaria.
> **Diretriz anti-alucinacao:** afirmar que a integralizacao em holding **de locacao** e "imune e ponto" e otimista e contestavel. Postura honesta: (i) a tese vinculante cobre so o excedente; (ii) ha fundamento forte (obiter do STF) pela imunidade incondicionada na integralizacao; (iii) TJSP e fiscos resistem → planejar com prova de receita operacional e, em holding de locacao, contar com possivel autuacao + discussao judicial. **Nao ha tese vinculante afastando a preponderancia na integralizacao.**

### 4. Trade-off — quanto integralizar (interacao com o IRPF) *(§1.2 + tributario §1)*
> **Regra de ouro:** quanto **maior** o capital social subscrito com o imovel, **maior a faixa imune de ITBI** — porem **maior o ganho de capital no IRPF** se a integralizacao for a **mercado** (art. 23 Lei 9.249/95: mercado − custo tributado a 15-22,5% na PF). Se a integralizacao for **a custo historico (DIRPF)**, nao ha ganho de capital, mas o capital subscrito fica limitado ao valor de custo → faixa imune menor e maior chance de "excedente" se o municipio arbitrar por valor de referencia. **Decisao caso a caso.**

### 5. Registro (nao averbacao) *(§1.4)*
A transmissao a holding aperfeicoa-se com o **REGISTRO** do titulo societario na matricula (LRP art. 167, I, item 32) — ato de **registro (R)**, nao averbacao. Ordem: (1) registra-se o contrato social na junta → (2) leva-se o ato arquivado a registro na matricula. Detalhe operacional/registral em `integralizacao-de-imoveis`.

## O que produzir
1. **Diagnostico do imovel:** valor de custo (DIRPF), valor de mercado/venal, destino da holding (locacao? participacao? guarda?).
2. **Simulacao da imunidade:** capital a integralizar x valor do imovel → parcela imune e parcela excedente (ITBI sobre o excedente, base municipal).
3. **Teste de preponderancia:** se holding de **locacao**, sinalizar o risco (TJSP/fiscos), orientar prova de receita operacional e a estrategia (documentar objeto, guardar comprovacao de receita nos 2+2 anos).
4. **Recomendacao de calibragem:** quanto de capital subscrever, custo x mercado, com a conta ITBI x ganho de capital lado a lado.

## Postura honesta
- **Holding de locacao normalmente NAO goza da imunidade plena** por conta da preponderancia imobiliaria — nao vender isencao garantida.
- O **excedente do capital tributa** (Tema 796); nao ha como "imunizar" alem do capital integralizado.
- A calibragem do capital e **trade-off**, nao almoco gratis: economizar ITBI a mercado pode custar ganho de capital no IRPF.

## Cross-link
`integralizacao-de-imoveis` (C3 — ato societario, descricao/matricula, registro) · `planejamento-tributario-holding` (ganho de capital, art. 23) · `celula-empresa-cofre`/`celula-adm-de-bens` (destino do imovel) · plugin `tributario-societario-adv-os` (imobiliario/registral fino). **Anti-duplicacao:** aqui e a ANALISE fiscal do ITBI; o documento e o registro sao da C3.

## Guard
Tema 796 = imunidade so ate o capital integralizado (excedente tributa). Preponderancia (CTN 37) nao ha tese vinculante afastando na integralizacao — postura honesta. Registro, nao averbacao (LRP 167 I item 32). Base do excedente = confirmar lei municipal. Nenhum numero sem `validador-holding`. Entrega fecha pela `suprema-corte-holding`.
