---
name: contrato-social-holding
description: Redige contrato social LTDA das 4 células (Cofre, ADM de Bens, Participações, Gestora) com o pacote de cláusulas de blindagem, Golden Share, administração conjunta, tag along e apuração de haveres validado para a JUCESP. Use quando o operador pedir "monta a holding", "contrato social da Cofre/ADM/Participações/Gestora", "constituir empresa cofre", "blindagem patrimonial via LTDA", "cláusulas de incomunicabilidade/impenhorabilidade/inalienabilidade", "estrutura societária familiar" ou constituição de qualquer célula da estrutura. Não é integralização de imóvel isolada (use integralizacao-de-imoveis), nem alteração de contrato existente (use alteracao-contratual), nem estatuto de S.A. (use estatuto-e-atos-sa).
---

# Contrato Social de Holding (LTDA — 4 células)

## 1. Quando esta skill ativa
Produção do **contrato social originário** de qualquer das 4 células em LTDA. Base territorial de referência: SP/JUCESP — adaptar à junta da sede. Antes de redigir, colher o mapeamento (skill `mapa-patrimonial`) e desenhar a estrutura (`diagnostico-estrutura`). Fundamento estendido em `context/clausulas-padrao-holding.md`, `context/societario-jucesp-sa.md`, `context/itcmd-itbi-sucessao.md`.

## 2. Mapeamento obrigatório antes de escrever
- **Sócios PF:** nome, nacionalidade, estado civil + **regime de bens**, profissão, nascimento, RG/CPF, endereço.
- **Sócias PJ (quando houver):** denominação, CNPJ, NIRE, sede, junta, administrador representante.
- **Estrutura:** denominação/capital/sede de cada empresa, distribuição de quotas (%), junta, **quem é o sócio patrimonial × operacional**, setor de risco das operacionais.

## 3. Estrutura de capítulos (JUCESP aceita — nunca quadro-resumo na abertura)
```
CAP I    Denominação, Objeto, Sede e Duração
CAP II   Capital Social e Quotas
CAP III  Cláusulas de Proteção Patrimonial (BLINDAGEM)
CAP IV   Administração e Golden Share
CAP V    Deliberações Sociais e Quórum   (unipessoal → "Decisões do Sócio Único")
CAP VI   Cessão de Quotas, Tag Along e Preferência
CAP VII  Exercício Social e Lucros
CAP VIII Apuração de Haveres na Saída de Sócio
CAP IX   Sucessão e Dissolução
CAP X    Disposições Gerais
```

## 4. Cláusulas ancoradas (copiar de `context/clausulas-padrao-holding.md`)
**Objeto (CAP I):** por célula. Cofre = guarda pura (vedação absoluta de atividade operacional, compra/venda de imóveis de terceiros, incorporação, loteamento, aval a terceiros). ADM = holding mista (administra + participa). Participações = controle das operacionais (§ não-confusão **art. 1.024 CC**). Gestora = mandatária do grupo com **vedação BCB expressa** no objeto. Incluir as **vedações setoriais específicas** do risco do grupo. CNAE: holdings **6462-0/00**; Gestora **6619-3/99**.

**Blindagem (CAP III):**
- Incomunicabilidade — **CC art. 1.911 c/c 1.668, I, e 1.848** (independe do regime de bens).
- Impenhorabilidade — com parágrafo de **frutos civis, CC art. 1.026, caput** (credor alcança só lucros/dividendos, sem direito político).
- Inalienabilidade — **15 anos** Cofre/ADM · **5 anos** Participações/Gestora, salvo sucessão hereditária.
- Proteção especial das quotas de **2%** (cláusula individualizada, anuência unânime por instrumento público).

**Administração + Golden Share (CAP IV):** administração **conjunta com alçadas** (atos isolados de gestão corrente até R$ 200.000,00; atos conjuntos obrigatórios com **nulidade expressa** para alienação/oneração, dívidas>R$200k, garantias e vinculação a operacionais de risco). **Golden Share em favor do sócio PATRIMONIAL** (nunca o operacional). Habilitação do administrador: **CC art. 1.011, §1º**.

**Cessão + tag along (CAP VI):** preferência dos sócios + **tag along 100%**, notificação prévia de **30 dias**, nulidade da cessão sem notificação; vedação de cessão das quotas de 2% na inalienabilidade.

**Lucros (CAP VII):** parágrafo de distribuição **inter-PJ isenta de IRRF — art. 10 da Lei 9.249/95** (Cofre/ADM → Participações). Não fixar alíquota; a distribuição final à PF sofre IRRF 10%>R$50k/mês + IRPFM (Lei 15.270/2025).

**Apuração de haveres (CAP VIII):** critério **valor patrimonial contábil — CC art. 1.031**, com **afastamento EXPRESSO** de avaliação a mercado e fluxo de caixa descontado; **§ imóveis pelo valor da DIRPF** do integralizador (trava o planejamento da integralização); pagamento em 24 parcelas IPCA + 6% a.a.; retenção 10% por 12 meses.

**Sucessão (CAP IX):** continuidade — **CC art. 1.028**; quotas herdadas mantêm as cláusulas restritivas (**CC art. 1.848**).

**Integralização de imóveis:** se houver, remeter à skill `integralizacao-de-imoveis` (descrição por matrícula, art. 23 Lei 9.249/95, ITBI Tema 796).

## 5. NUNCA incluir (gera exigência JUCESP ou prova contra a empresa)
Quadro-resumo/sumário na abertura · **regime tributário** no contrato (é opção anual na RFB) · reserva de lucros com cap obrigatório · auditoria externa obrigatória · seguros obrigatórios · não-concorrência entre familiares · deadlock/buy-sell em estrutura 98/2 (não há deadlock possível) · cláusula copiando lei literal sem adaptação · instituto exclusivo de S.A. sem adequação ao tipo.

## 6. Regra do administrador de fato
**Quem opera, assina; quem protege, veta.** O sócio operacional **deve** ser coadministrador (gestão corrente) mesmo detendo só 2% — excluí-lo cria risco de administrador de fato + simulação (**CC art. 167**), que pode anular todas as cláusulas de proteção.

## 7. Postura honesta (dizer ao cliente — não vender muralha)
- Holding **não é blindagem absoluta**: não afasta legítima (CC 1.846/1.848), fraude contra credores/à execução (CC 158/167; CPC 792, IV) nem desconsideração (CC 50). A cláusula **organiza e dificulta — não imuniza**.
- Impenhorabilidade contratual **não é absoluta**: o credor pode alcançar lucros e requerer a **liquidação da quota** (CC 1.026/1.031).
- Inalienabilidade sobre a parte que corresponde à **legítima** exige **justa causa declarada** (CC 1.848) — sem ela, é nula sobre a legítima; sobre a parte disponível é livre.
- O que blinda de verdade é **tempestividade + substância econômica** (contabilidade, contratos formais, ITCMD pago). Holding "de gaveta" é alvo fácil.

## 8. Campos que ficam em branco até o registro
Marcar (alerta visual) sede, CNPJ próprio, CNPJ de sócias PJ admitidas e data do instrumento — só existem após os registros. Sequência de produção das células: `sequencia-de-producao` (Gestora → Cofre → Participações → ADM).

## 9. Fecho
Toda minuta fecha por **`suprema-corte-holding`** (R1 estrutura/sócios · R2 lei vigente · R3 tributário · R4 forma/registro) + **`validador-holding`**. Guard permanente: `anti-alucinacao-holding`. Cross-link soft: `integralizacao-de-imoveis`, `acordo-de-socios`, `registro-jucesp-drei`, `tributario-societario` (planejamento tributário geral).
