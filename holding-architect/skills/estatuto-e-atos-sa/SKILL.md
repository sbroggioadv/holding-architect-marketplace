---
name: estatuto-e-atos-sa
description: Redige o estatuto da S.A. fechada familiar usada como holding e os atos societários do ciclo (constituição por subscrição particular, AGO/AGE, conselho de administração, diretoria, conselho fiscal, livros) e diz quando a S.A. compensa sobre a LTDA (art. 294 LSA = receita ≤ R$ 78 mi). Use quando o operador pedir "estatuto da S.A.", "holding como S.A.", "vale a pena S.A. ou LTDA?", "ações ON/PN", "voto plural", "conselho de administração", "AGO/AGE", "constituir companhia fechada", "migrar LTDA pra S.A." ou governança sofisticada de família grande. Não é o contrato LTDA (use contrato-social-holding) nem o pacto de voto (use acordo-de-socios).
---

# Estatuto e Atos da S.A. (holding fechada familiar)

## 1. Quando esta skill ativa
Modelar o **estatuto** e os **atos** da S.A. de capital **fechado** familiar usada como holding (companhia de participação, LSA art. 2º, §3º), e decidir **S.A. × LTDA**. Fundamento verbatim em `context/societario-jucesp-sa.md` (§3-5). Dispositivos da Lei 6.404/76 no texto consolidado.

## 2. Quando a S.A. compensa (critério — art. 294 primeiro)
**Regra geral:** para holding familiar a **LTDA basta e é mais barata** na maioria dos casos. A **S.A. fechada compensa** quando:
1. Acordo de acionistas robusto (**art. 118**) > acordo de quotistas — família com conflito, deadlock, put/call, pool de voto.
2. **Conselho de administração** (art. 138) — separar propriedade (família) de gestão.
3. Classes **ON/PN + voto plural** (arts. 15/16/110-A) — engenharia sucessória fina.
4. **Sigilo do quadro** — transferência de ações nominativas nos livros internos (art. 100), sem ir à junta a cada negócio (na LTDA, toda mudança de QSA é pública).
5. Captação/profissionalização; patrimônio elevado + muitas operacionais + muitos herdeiros.

> **Anti-erro (dispositivo travado): art. 294 LSA** — a companhia fechada com **receita bruta anual ≤ R$ 78.000.000,00** (LC 182/2021) pode fazer publicações eletrônicas (III) e substituir livros por registros eletrônicos (IV). **NÃO** é "menos de 20 acionistas + PL até R$ 10 mi" (redação revogada da Lei 13.818/2019). O **§3º** exclui a **companhia controladora de grupo** e filiadas — holding controladora avalia caso a caso.

## 3. Constituição (subscrição particular — caminho da holding familiar)
- **Art. 80:** subscrição por ≥ 2 pessoas de todas as ações; entrada de **≥ 10% em dinheiro** do preço de emissão das ações subscritas **em dinheiro**; **depósito** bancário dessa parcela. **Art. 81:** depósito em 5 dias; restituição se a companhia não se constituir em 6 meses.
- **Art. 88 — subscrição particular:** por assembleia de fundadores ou por **escritura pública**; a via pública exige qualificação dos subscritores, estatuto, relação de ações/entradas, transcrição do recibo do depósito e, havendo bens, **transcrição do laudo de avaliação** (arts. 8º-10). **Art. 82 (subscrição pública)** é desnecessária e antieconômica para holding fechada.
- **Integralização de imóveis:** **art. 89 dispensa escritura pública**; avaliação por **laudo de 3 peritos ou empresa especializada** (arts. 8º-10) aprovado em assembleia. Mecânica ITBI/registro na skill `integralizacao-de-imoveis`.

## 4. Estatuto — conteúdo (art. 83 remete aos requisitos gerais + peculiares)
Denominação + "S.A."/"Companhia"; objeto (holding de participação, art. 2º §3º); sede/prazo; **capital e ações** (espécies/classes); órgãos (assembleia, administração, conselho fiscal); exercício social e destinação do lucro; foro. Não há rol único — extrai-se da combinação da LSA.

**Ações (art. 15):** ordinárias, preferenciais ou de fruição; **PN sem voto ≤ 50%** do total (§2º). Para holding familiar: **ON com voto** para controladores + **PN sem voto** para herdeiros "investidores". **Voto plural — art. 110-A** (até **10 votos** por ação ordinária, por **prazo limitado**): instrumento de controle sucessório.

## 5. Órgãos sociais
- **AGO — art. 132:** nos **4 primeiros meses** após o exercício, para contas/demonstrações, destinação do lucro e dividendos, eleição de administradores/conselho fiscal. Demais matérias (reforma de estatuto, reorganização) = **AGE (art. 122)**.
- **Conselho de administração — arts. 138/140:** **obrigatório apenas** em companhia aberta, de capital autorizado e de economia mista. **Holding fechada sem capital autorizado pode operar só com Diretoria** (simplifica). Se houver: **mínimo 3 membros**, mandato ≤ 3 anos.
- **Diretoria — art. 143 (LC 182/2021):** **admite diretor único** (o texto antigo exigia 2+). Holding familiar pode ter diretoria unipessoal.
- **Conselho fiscal — art. 161:** existência prevista no estatuto; **funcionamento pode ser não-permanente** (instalado a pedido de acionistas — 0,1 das ações com voto ou 5% sem voto). Dá transparência ao ramo minoritário.

## 6. Atos após a constituição
- **Livros — art. 100:** Registro e Transferência de Ações Nominativas, Atas de AG, Presença, Atas do Conselho/Diretoria, Conselho Fiscal. Físicos ou **eletrônicos** (art. 294, IV, no porte do §2).
- Demonstrações financeiras anuais (arts. 176+) submetidas à AGO; atas arquivadas na junta quando alteram estatuto/eleição/capital/reorganização; dividendos (arts. 202+); deveres dos administradores — diligência, lealdade, conflito (arts. 153-156).
- **Acordo de acionistas (art. 118):** ver `acordo-de-socios`.

## 7. Postura honesta
- **Não há diferença tributária relevante** S.A. × LTDA só pela forma — a escolha é de **governança/sigilo/sucessão**, não fiscal.
- A S.A. tem **custo recorrente maior** (livros, AGO formal, eventuais publicações). Migrar LTDA→S.A. só quando os critérios da S.A. **pesarem mais** que esse custo. Não vender S.A. como "mais blindada": a blindagem vem da substância, não do tipo.
- Sem **conflito real / classes / siglo / família grande**, recomendar **LTDA** (mais barata e suficiente).

## 8. Fecho
Fecha por **`suprema-corte-holding`** (R2 lei vigente — nunca redação revogada do art. 294 · R4 forma/órgãos) + **`validador-holding`**. Guard: `anti-alucinacao-holding`. Cross-link soft: `contrato-social-holding` (LTDA), `acordo-de-socios`, `registro-jucesp-drei` (Anexo V DREI), `integralizacao-de-imoveis`.
