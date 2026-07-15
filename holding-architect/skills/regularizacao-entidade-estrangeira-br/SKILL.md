---
name: regularizacao-entidade-estrangeira-br
description: Executa a PONTA BRASILEIRA que faz uma entidade estrangeira (ex.: LLC de Delaware) virar apta a ser sócia de holding BR — apostila da Haia (Dec 8.660/2016 + Res. CNJ 228/2016), tradução juramentada (Dec 13.609/1943, CC 224, CPC 192) e CNPJ da estrangeira na RFB (IN RFB 2.119/2022, Natureza Jurídica 221-6, representante domiciliado no Brasil art. 6º §1º + declaração de beneficiário final). A ABERTURA lá fora é parceiro in loco. Use quando o operador disser "preciso do CNPJ da empresa estrangeira", "apostila", "tradução juramentada dos documentos", "como registrar a LLC no Brasil", "documentos da offshore no Brasil", "beneficiário final", "/offshore regularizacao".
---

# REGULARIZAÇÃO DA ENTIDADE ESTRANGEIRA NO BRASIL

> Camada 5 (Offshore — ponta BR). Transforma a entidade já aberta lá fora em entidade **reconhecida no Brasil** (documentos com fé pública + CNPJ próprio). Pré-requisito de `registro-investimento-bcb` e `estrangeira-como-socia`.

## Anexos obrigatórios (context/)
- `context/offshore-ponta-br.md` — **§1** (apostila + tradução juramentada; tabela de documentos da LLC) e **§2** (CNPJ de entidade domiciliada no exterior — IN RFB 2.119/2022, NJ 221-6, representante, QSA/UBO). `grep -n "8.660\|2.119\|221-6\|beneficiário final\|apostila\|juramentada" context/offshore-ponta-br.md`.

## Limite de escopo
A **abertura** da entidade (Certificate of Formation, Good Standing, Operating Agreement, procuração) é providenciada pelo **parceiro in loco / cliente lá fora**. O plugin orienta **o que pedir** e executa a **ponta brasileira**.

## Quando ativar
Cliente já tem (ou está abrindo) a entidade no exterior e precisa dela apta no Brasil para entrar numa holding BR, receber remessas ou constar de QSA.

## Base legal ancorada (context/offshore-ponta-br §1-§2)
- **Apostila da Haia — Dec 8.660/2016** (em vigor no Brasil desde 14/08/2016) + **Res. CNJ 228/2016**: substitui a legalização consular. Emitida **no país de origem** (ex.: Secretary of State em Delaware). Recai sobre documento **público** ou documento **privado notarizado** (apostila-se o selo do notário).
- **Tradução juramentada — Dec 13.609/1943** (tradutor público, fé pública) + **CC art. 224** (documento em língua estrangeira só produz efeito após tradução) + **CPC/2015 art. 192** (em juízo). Junta comercial exige tradução dos atos da estrangeira para arquivamento.
- **CNPJ da estrangeira — IN RFB 2.119/2022** (em vigor desde 01/01/2023): **art. 4º, §2º** obriga a inscrição da entidade domiciliada no exterior **titular de participação societária em PJ no Brasil** → a entidade que será sócia da holding precisa de **CNPJ próprio**, **Natureza Jurídica 221-6** ("Empresa Domiciliada no Exterior", Anexo VIII).
- **Representante no CNPJ (art. 6º, §1º):** procurador/representante legal **domiciliado no Brasil**, pessoa física residente, com poderes para administrar os bens/direitos da entidade no País e representá-la perante a RFB.
- **Beneficiário final (arts. 52-53):** informar QSA + UBO com organograma até a pessoa natural; declaração em **30 dias** da abertura do CNPJ. Critério usual: participação **> 25%** — **conferir o texto literal do art. 53 antes de citar o percentual em peça** (marcar "a confirmar" e rotear ao `validador-holding`).

## Documentos da estrangeira (LLC Delaware — §1.2)
| Documento | Natureza | Caminho |
|---|---|---|
| Certificate of Formation / Incorporation | Público | Apostila → tradução juramentada |
| Certificate of Good Standing | Público | Apostila → tradução juramentada |
| Operating Agreement / Bylaws | Privado | Notarização → apostila do ato notarial → tradução |
| Procuração ao representante no Brasil | Privado | Notarização → apostila → tradução |
| ID do administrador no exterior + prova de poderes | Conforme | Apostila/notarização → tradução |

## Sequência operacional (o que produzir)
1. **Listar e obter (parceiro lá fora)** os documentos da tabela + a **procuração** ao representante no Brasil.
2. **Apostilar no país de origem** (públicos direto; privados via notarização + apostila do selo).
3. **Tradução juramentada no Brasil** de todos os documentos estrangeiros.
4. **CNPJ da estrangeira na RFB** (NJ 221-6): Coletor Nacional + **Anexo VIII** (ato de constituição; ato de poderes do representante no exterior; ID do representante no exterior; **ato de nomeação do representante no Brasil** + ID; todos apostilados + traduzidos).
5. **QSA + beneficiário final** com organograma da cadeia até a pessoa natural — declaração em **30 dias**.
6. **Nota da integração BCB:** a inscrição pode decorrer do cadastramento no **CDNR (Cadastro Declaratório de Não Residentes) do BCB** — integração CNPJ (RFB) ↔ não residente (BCB). "CADEMP" é nomenclatura histórica; hoje o não residente passa pelo CDNR — **confirmar a terminologia no manual SCE-IED vigente** (`registro-investimento-bcb`).
7. **Entregar o checklist** (documento · apostilado? · traduzido? · protocolado onde) + a minuta de **procuração** com os poderes mínimos (delegar a `estrangeira-como-socia` a redação completa).

## Postura honesta
- O prazo real depende do país de origem (apostila) e da fila do tradutor juramentado — não prometer prazo fechado.
- **Ordem inegociável:** documento estrangeiro → (notarização, se privado) → **apostila no país de origem** → **tradução juramentada no Brasil** → uso na RFB/BCB/junta. Pular a apostila = documento rejeitado.
- Percentual de beneficiário final: só citar **após** conferir o art. 53 literal.

## Cross-link soft
Registro do capital que ingressa → `registro-investimento-bcb` · procuração e admissão no quadro → `estrangeira-como-socia` · escolha da jurisdição → `offshore-diagnostico-fiscal` · roteiro de junta → `registro-jucesp-drei`.

## Guard
Nenhum dispositivo/IN/percentual sem `validador-holding` (cruzar com `context/offshore-ponta-br.md`). CNPJ da estrangeira = **NJ 221-6, IN RFB 2.119/2022**. Registro de capital estrangeiro = **Lei 14.286/2021** (não 4.131/62). Fecha pela `suprema-corte-holding` (R1-R4).
