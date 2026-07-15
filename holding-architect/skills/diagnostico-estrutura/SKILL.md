---
name: diagnostico-estrutura
description: Mapeia patrimonio, socios (operacional x patrimonial), setor de risco e objetivo, e desenha QUANTAS celulas e QUAL variacao da estrutura das 4 celulas aplicar (socio unico / familia ampla / alto risco com sub-holding). Use quando o operador disser "quantas empresas preciso?", "qual estrutura de holding serve pro caso?", "vale Cofre e ADM separadas ou uma so?", "tenho socio, como divido?", "monta o desenho da holding", "diagnostico de estrutura", "quantas celulas", ou antes de constituir qualquer celula. Entrega o DESENHO da estrutura + justificativa por celula + variacao escolhida (nao o contrato — isso e contrato-social-holding).
---

# DIAGNOSTICO DE ESTRUTURA — quantas celulas e qual variacao

> Camada 2 (nucleo do metodo das 4 celulas). Traduz patrimonio + socios + risco + objetivo no DESENHO da estrutura. Nao redige documento — decide a arquitetura que as demais `celula-*` e o `contrato-social-holding` executam.

## Anexo obrigatorio (ler primeiro)
- `context/metodologia-4-celulas.md` — arquitetura, §2 (as 4 celulas), §7 (variacoes), §8 (checklist de adaptacao). Grep o topico + ler a faixa.

## Quando ativa
Entrada consultiva de estrutura: o cliente ainda nao sabe quantas empresas nem qual composicao. Vem antes de `sequencia-de-producao` e das `celula-*`. Se o operador ja definiu a estrutura, pule para elas.

## 1. Levantamento obrigatorio (checklist §8 — perguntar por botoes)
Colete via **AskUserQuestion** (lista fechada = botao), nunca supor em silencio:
1. **Quem e o socio patrimonial** (detem o patrimonio imobiliario/financeiro) **e quem e o operacional** (opera as empresas de risco)? Pode ser a mesma PF (socio unico).
2. **Setor de risco das operacionais** — define as vedacoes do objeto de cada celula.
3. **Patrimonio a integralizar** (imoveis, participacoes, aplicacoes) — define o capital da Cofre/ADM.
4. **O patrimonio gera renda ativa?** (aluguel, cessao onerosa, gestao de carteira) → indica ADM de Bens; so guarda → Cofre.
5. **Regime de bens do socio patrimonial** — dispara a incomunicabilidade.
6. **Sede: SP (JUCESP) ou outro estado.**
7. **Ha sociedade ja existente** para reaproveitar (alteracao) ou tudo do zero (constituicao)?
8. **Ha herdeiros necessarios?** Doacao sera igual ou desigual? → dispara legitima/colacao (roteia a `planejamento-sucessorio`).
9. **Objetivo dominante:** protecao patrimonial / sucessao / eficiencia tributaria / offshore.

## 2. Regra de decisao — quantas celulas
| Sinal do caso | Celula indicada |
|---|---|
| Patrimonio imobilizado a **guardar** (nao opera, nao cede risco) | **Empresa Cofre** (98/2 PF, 15a) — `celula-empresa-cofre` |
| Patrimonio que **gera renda ativa** (aluguel, cessao, carteira) | **ADM de Bens** (98% + Participacoes 2% PJ, 15a) — `celula-adm-de-bens` |
| Ha **empresas operacionais de risco** a controlar | **Holding de Participacoes** (unipessoal, 5a) — `celula-holding-participacoes` |
| **Volume relevante** de transacoes financeiras internas | **Gestora de Pagamentos** (mandataria, vedacao BCB, 5a) — `celula-gestora-pagamentos` |

Nao inventar celula: cada uma tem custo de manutencao (contabilidade, obrigacoes acessorias, DBE). So desenhe a celula que resolve um sinal real do caso.

## 3. Variacoes (metodologia-4-celulas §7) — escolher e justificar
- **Socio unico** — o titular detem 98%-100% de tudo; Golden Share fica com ele; sucessao via testamento ou **doacao de quotas com reserva de usufruto** (roteia `doacao-quotas-usufruto`).
- **Familia ampla (varios socios patrimoniais)** — os 98% da Cofre/ADM divididos entre membros; Golden Share no patriarca/matriarca; **deadlock so** em 50/50 real (com controlador claro e inutil — nao incluir).
- **Alto risco (operacionais em setor perigoso)** — camada extra: Participacoes → **sub-holding setorial** → operacional; cada camada e uma barreira a mais contra credor; troca = custo/complexidade.

## 4. Entrega
Desenho da estrutura (mapa das celulas escolhidas + composicao societaria + % + prazos de inalienabilidade + Golden Share) + **1 linha de justificativa por celula** + variacao adotada + o que fica de fora e por que. Encaminha a `sequencia-de-producao` para a ordem de registro.

## 5. Postura honesta (repetir ao cliente)
- **Holding NAO e blindagem.** Organiza, sucede, torna eficiente — nao vence legitima (CC 1.846/1.848), fraude (CC 158/167) nem desconsideracao (CC 50). Prometer muralha e erro (e risco de venda).
- **Mais celulas ≠ mais protecao automatica.** Estrutura superdimensionada so aumenta custo e superficie de fiscalizacao. Desenhe o minimo que atende o objetivo.
- **Quem opera, assina; quem protege, veta** — o socio operacional e coadministrador de fato; excluir da gestao gera administrador de fato + simulacao (art. 167 CC).
- Numero (aliquota, capital, prazo) so vem do `context/`; o que nao confirmar, marcar "a confirmar" e rotear ao `validador-holding`.

## Cross-link (soft, nao duplicar)
`triagem-holding` (classificacao de entrada) · cada `celula-*` (design fino) · `sequencia-de-producao` (ordem de registro) · `parecer-viabilidade-holding` ("vale a pena?") · `contrato-social-holding` (instrumento).

## Fecha por
`suprema-corte-holding` R1 (estrutura/socios/patrimonio) valida o desenho antes de virar documento.
