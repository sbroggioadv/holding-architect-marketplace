---
name: memoria-de-caso-holding
description: Mantém o estado do caso de holding entre skills e turnos — perfil do escritório, sócios e papéis, patrimônio, células já desenhadas/constituídas, CNPJs, fase da produção, atos registrados e pendências. Use sempre que uma skill precisar ler ou gravar o andamento (o que já foi feito, o que falta, qual CNPJ já saiu), quando o usuário perguntar "onde paramos", "resume o caso", "o que falta", ou quando o `holding-master` retomar um caso. É a fonte única do estado; não redige peça.
---

# memoria-de-caso-holding — estado vivo do caso

Memória de trabalho do plugin. Todas as skills leem daqui antes de agir e gravam aqui ao terminar. Impede retrabalho e mantém a sequência de produção coerente (que célula já tem CNPJ, qual é o próximo ato).

## Quando ativa
- No início de qualquer skill (ler o estado).
- Ao concluir um passo (gravar o avanço).
- Sob demanda: "onde paramos?", "resume o caso", "o que falta?", retomada pelo `holding-master`.

## Estrutura do estado
Mantenha dois escopos separados:

### A) Perfil do escritório (persistente entre casos — vem do `holding-onboarding`)
- `perfil_configurado`: sim/não
- nome/marca · OAB+seccional · cidade/UF
- praça de registro predominante · estilo de peça · postura Reforma 2027

### B) Caso atual
- **Sócios:** cada um com papel (patrimonial / operacional / único), % nas células, regime de bens, se é herdeiro necessário.
- **Patrimônio:** bens a estruturar, valor aproximado, base DIRPF, quais geram renda ativa.
- **Objetivo(s):** proteção / sucessão / tributário / offshore.
- **Estrutura desenhada:** nº de células, variação (sócio único / família ampla / alto risco), sub-holdings.
- **Células — status por célula:** `desenhada` → `contrato pronto` → `protocolada` → `registrada (CNPJ: ____)`.
- **CNPJs obtidos:** Gestora, Cofre, Participações, ADM (na ordem da sequência).
- **Fase da produção:** diagnóstico / desenho / documentos / tributário-sucessório / offshore / governança / registro / concluído.
- **Atos e registros:** contratos, alterações, integralizações, doações, acordos já produzidos e seu status na junta/cartório.
- **Pendências e "a confirmar":** itens que o `validador-holding` marcou para checar; próximos passos.

## Regras de gravação
1. **Append-first:** registre o avanço sem apagar o histórico do caso (o que já foi feito é auditoria).
2. **Sequência de produção é invariante:** a fase "ADM registrada" só é válida se Participações já tem CNPJ (a ADM recebe a Participações por **alteração** — ver `metodologia-4-celulas.md` §5). Se o estado violar a ordem Gestora → Cofre → Participações → ADM, sinalize.
3. **Zero PII no produto:** este estado vive na sessão/no caso do operador; **nunca** migra para o conteúdo do plugin nem para repositório público. Dados de cliente ficam com o advogado.
4. **Número sem âncora não vira verdade:** se uma skill gravar um dispositivo/alíquota "a confirmar", mantenha o rótulo até o `validador-holding` confirmar contra o `context/`.

## Saída típica ("onde paramos")
```
CASO: <apelido> · FASE: <fase>
Sócios: <papéis e %>
Estrutura: <nº células / variação>
Células: Gestora [reg CNPJ ..] · Cofre [reg CNPJ ..] · Particip. [contrato pronto] · ADM [pendente alteração]
Próximo ato: <o quê> · Pendências: <lista> · A confirmar: <lista>
```

## Fronteira
Só guarda estado — não decide estrutura (é `diagnostico-estrutura`) nem redige peça (skills de C3). O produto que sair de qualquer fase fecha por `suprema-corte-holding`.
