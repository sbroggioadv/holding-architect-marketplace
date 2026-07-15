---
name: registro-jucesp-drei
description: Roteiro de registro da holding na junta (JUCESP como base) segundo a IN DREI 81/2020 — viabilidade/RedeSim, DBE, integralização de imóveis no contrato, DARE, assinatura digital e as causas mais frequentes de exigência. Use ao protocolar constituição ou alteração das células, montar a documentação da junta, descrever imóveis no capital, ou quando o cliente/escritório perguntar "como registro a holding?" / "caiu em exigência, e agora?" / "qual anexo do DREI é da LTDA?" / "a entrada da Participações na ADM é constituição ou alteração?".
---

# Registro na Junta — JUCESP / DREI IN 81/2020

## 1. Quando ativa
Ao levar qualquer célula à junta: constituição, alteração, integralização de imóveis, correção de exigência. Base = **SP/JUCESP** (variação por estado declarada — confirmar na junta local). Aplica a sequência de produção das 4 células. Alimenta `sequencia-de-producao`, `contrato-social-holding`, `alteracao-contratual`, `integralizacao-de-imoveis`.

## 2. Base normativa ancorada (`societario-jucesp-sa.md`)
**IN DREI nº 81, de 10/06/2020** (alterada pelas INs 55/2021, 88/2022, 112/2022) — normas gerais do Registro Público de Empresas. Manuais/anexos:
- **Anexo II** = Empresário Individual · **Anexo IV = SOCIEDADE LIMITADA** · **Anexo V = SOCIEDADE ANÔNIMA**. (Anexo III/EIRELI esvaziado — Lei 14.195/2021 transformou EIRELI em LTDA unipessoal.)
> **Trava anti-erro:** Anexo **IV = LTDA**, Anexo **V = S.A.** — não trocar.
- Manual da S.A. (Anexo V) exige comprovação de depósito de **≥ 10%** do capital subscrito em dinheiro + **laudo de avaliação** quando há integralização em bens.
- Natureza jurídica da LTDA no DBE = **206-2 (Sociedade Empresária Limitada)**.
- Nome empresarial protegido pela **IN DREI 15/2013**.

## 3. Roteiro de protocolo (VRE / portal JUCESP)
1. **Planejamento** — NJ 206-2, CNAE (holding: 6462-0/00; gestora: 6619-3/99), capital, imóveis a integralizar.
2. **Viabilidade** (nome + endereço) na RedeSim / Via Rápida Empresa → aguardar **deferimento**.
3. **Contrato social** conforme Manual LTDA: nome; capital + quotas + **forma e prazo de integralização**; sede; objeto (com locação de imóveis próprios expressa, se for o caso); prazo de duração; exercício social; administração + poderes; participação em lucros/perdas; foro; cláusula de integralização de imóveis.
4. **DBE** na Coleta Web — **espelhar** capital/sócios/CNAE/endereço do contrato.
5. Montar documentação digital (contrato PDF assinado, viabilidade, DBE, docs dos sócios, capa, comprovante DARE).
6. **DARE** — calcular e pagar (valor varia por estado/tempo — **não fixar número**; confirmar na emissão).
7. **Assinar** digitalmente — **e-CPF (ICP-Brasil)** ou conta gov.br nível Prata/Ouro (certificado inválido trava).
8. **Protocolar** (tipo de ato = Constituição) → nº de protocolo.
9. Acompanhar status → **cumprir exigência no mesmo processo**.
10. Pós-deferimento: CNPJ liberado via DBE; inscrições municipal/estadual.

**Integralização de imóveis no contrato (evita exigência):** individualizar cada imóvel — nº da **matrícula** + **Cartório de RI/comarca**, endereço/área/tipo, **valor em R$** atribuído. O valor pela DIRPF (art. 23 Lei 9.249) é critério fiscal, não exigência do DREI; a junta só checa coerência valor↔capital. A transmissão na matrícula é **ato posterior** no RI (→ `itbi-integralizacao`, `itcmd-itbi-sucessao.md`).

## 4. Constituição × Alteração — impacto nas 4 células
- **Constituição** = 1º ato (contrato originário).
- **Alteração** = ato posterior; novo protocolo, DARE próprio.
> **Chave do método:** a entrada da **Holding de Participações como sócia 2% da ADM de Bens** é **ATO DE ALTERAÇÃO** (não constituição) — exige **contrato consolidado + DBE de evento de alteração de QSA**. Sequência: **Gestora → Cofre → Participações → ADM(alteração)** (dependência de CNPJ — a Participações precisa de CNPJ para entrar na ADM).

## 5. Causas mais frequentes de exigência (checar antes de protocolar)
1. Nome empresarial colidente / incompatível (IN DREI 15/2013).
2. Objeto genérico sem conexão com o CNAE do DBE.
3. Capital/integralização sem "forma e prazo"; imóvel sem matrícula; capital do contrato ≠ DBE.
4. Endereço divergente entre contrato × viabilidade × DBE.
5. Qualificação incompleta de sócio/administrador; poderes não definidos.
6. Assinaturas faltantes; certificado/gov.br inválido.
7. DBE ausente/status inadequado; sem DARE; sem viabilidade deferida.
8. Em LTDA a JUCESP rejeita: quadro-resumo/sumário na abertura; cláusula que copia lei literal sem adaptar; instituto exclusivo de S/A sem adequação; numeração de parágrafo fora do padrão (usar §1º, §2º, Parágrafo único).

## 6. Postura honesta
- Prazos de análise **não têm previsão legal nacional**; prática JUCESP ≈ 3–5 dias úteis em constituição simples (exigência estende) — **não prometer prazo fixo**.
- Valor da DARE e detalhes de procedimento **variam por estado** — fora de SP, confirmar na junta local; não transportar regra da JUCESP como nacional.
- Descrição registral fina do imóvel na matrícula é do domínio imobiliário — cross-link, não duplicar.

## 7. Cross-link
`societario-jucesp-sa.md` (fonte) · `base-societaria` (tipo) · `sequencia-de-producao` · `integralizacao-de-imoveis` · `itcmd-itbi-sucessao.md` (registro no RI) · plugin `direito-imobiliario` (registral fino).

## 8. Fechamento
Documento de registro fecha por **`suprema-corte-holding`** (R4 forma/registro/sequência) + **`validador-holding`** (Anexo IV/V correto, NJ 206-2, CNAE).
