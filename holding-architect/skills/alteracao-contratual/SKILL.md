---
name: alteracao-contratual
description: Redige alterações de contrato social de holding LTDA — admissão de sócia (inclusive a Holding de Participações como sócia 2% da ADM), integralização de novo capital, mudança de objeto/sede/denominação/administração — com contrato consolidado e roteiro de protocolo/DBE na junta. Use quando o operador pedir "altera o contrato", "admite a Participações na ADM", "aumenta o capital", "muda o objeto/sede", "consolida o contrato social", "entra sócio novo na holding", "integraliza mais um imóvel" ou o passo 4 da sequência das células. Não é a constituição originária (use contrato-social-holding) nem a integralização em si (use integralizacao-de-imoveis para a mecânica ITBI/ganho de capital).
---

# Alteração Contratual de Holding (LTDA)

## 1. Quando esta skill ativa
Produção de **ato posterior** que modifica cláusula(s) de contrato já registrado. Casos típicos na estrutura das 4 células:
- **Admissão da Holding de Participações como sócia 2% da ADM de Bens** — é o **passo 4** da sequência de produção (ver `sequencia-de-producao`): a Participações só pode ser admitida depois de já ter CNPJ.
- Aumento de capital por **integralização de bens** (remeter a mecânica a `integralizacao-de-imoveis`).
- Mudança de objeto, sede, denominação, prazo, administração ou quadro de sócios (QSA).
Fundamento em `context/societario-jucesp-sa.md` (§1.3, §1.7).

## 2. Constituição × alteração (não confundir)
- **Constituição** = 1º ato; nasce a sociedade.
- **Alteração** = ato posterior; **depende do contrato já registrado**; cada alteração é **novo protocolo com DARE/taxas próprias**. Normalmente dispensa nova viabilidade, **salvo** mudança de **sede, atividade (objeto) ou nome** — nesses casos, refazer a viabilidade no VRE.

## 3. O que produzir
1. **Instrumento de alteração** com o(s) artigo(s) modificado(s), redação nova e cláusula de **consolidação** ("passa a vigorar com a seguinte redação consolidada").
2. **Contrato social consolidado** anexo (a junta e o CPC 599 §1º exigem o consolidado; a dissolução parcial se instrui com ele).
3. **DBE de evento** correspondente na Coleta Web/RedeSim — na admissão de sócia PJ, evento de **alteração de QSA**; espelhar capital/sócios/CNAE/endereço do instrumento.
4. Documentação digital: instrumento + consolidado (PDF assinado por e-CPF/gov.br Prata/Ouro), DBE, docs dos novos sócios/administradores, comprovante de **DARE**.

## 4. Admissão da Participações como sócia 2% (caso central)
- Preencher o **CNPJ e NIRE** da Participações (obtidos no passo 3 da sequência) na qualificação da nova sócia PJ.
- Redistribuir o capital: sócio patrimonial 98% + **Participações 2% (PJ)** — a finalidade é **distribuição inter-PJ isenta de IRRF, art. 10 da Lei 9.249/95** (nomear o fundamento no parágrafo de lucros).
- Manter no consolidado o **pacote de blindagem** e a **proteção especial das quotas de 2%** (anuência unânime, vedação de constrição por dívida estranha do titular).
- Repetir o pacote de cláusulas restritivas no consolidado — não deixá-lo "para trás" na versão anterior.

## 5. Erros que geram exigência (evitar)
- Divergência de **capital, endereço ou nome** entre DBE × instrumento × consolidado × viabilidade.
- Integralização de imóvel **sem matrícula/CRI** ou sem cláusula de **forma e prazo**; valor do imóvel ≠ acréscimo de capital.
- Qualificação incompleta do novo sócio/administrador; poderes do administrador não definidos.
- Numeração de parágrafo fora do padrão (usar §1º, §2º, Parágrafo único); cláusula que copia lei literal sem adaptação; instituto exclusivo de S.A. sem adequação ao tipo.
- Certificado digital/gov.br inválido; DARE não paga; DBE em status inadequado.

## 6. Alteração de sede interestadual (nota)
Transferência de sede para outro estado muda a junta competente e **exige nova viabilidade**. Decidir com o cliente se mantém a sede no estado original ou transfere, e instruir o procedimento na junta de destino antes de protocolar.

## 7. Postura honesta
- Alteração **não retroage** para "consertar" fraude anterior: se a estrutura original for atacável por fraude contra credores/à execução (CC 158/167; CPC 792, IV) ou simulação (CC 167), a alteração não sana.
- Toda mudança de QSA em LTDA é **pública** (certidão da junta) — não há sigilo do quadro (diferença estrutural para a S.A. — ver `estatuto-e-atos-sa`).

## 8. Fecho
Fecha por **`suprema-corte-holding`** (R1-R4) + **`validador-holding`**. Guard: `anti-alucinacao-holding`. Cross-link soft: `contrato-social-holding` (originário), `integralizacao-de-imoveis`, `registro-jucesp-drei`, `sequencia-de-producao`.
