---
name: retomar-projeto
description: Use ao abrir, continuar ou assumir um projeto que já tem docs/PROJETO.md, ou quando o usuário pergunta "onde paramos?" ou "o que falta?". Lê o estado do projeto e propõe o próximo passo.
---

# Retomar projeto

Responda em português do Brasil, simples e direto.

## Passo a passo

1. Leia `docs/PROJETO.md` e, a partir do índice, só os MDs relevantes (tarefas.md, pendencias.md, decisoes.md). Se não existir PROJETO.md, use a skill **comecar-projeto**.
2. Confira se o documento bate com a realidade: olhe o código e o histórico recente do git (se houver). Se divergir, avise e corrija o PROJETO.md.
3. Resuma em até 10 linhas: o que é o projeto, em que fase está, o que já foi feito, o que falta planejar e dúvidas abertas.
4. Proponha **a próxima ação** (uma só, com motivo) e a skill indicada:
   - ideia confusa: descobrir-ideia
   - falta ver telas: prototipar
   - falta definir o que construir: requisitos
   - falta decidir como construir: arquitetura
   - falta desenhar: diagramas
   - código novo para conferir: revisar-codigo e testes
   - falta explicar: documentar
5. Pergunte se o usuário quer seguir esse caminho.

## Ao terminar qualquer trabalho

Atualize no `docs/PROJETO.md`: estado atual, tabela de planejamento, tarefas, pendências, próxima ação e data. Marque tarefas concluídas em `docs/tarefas.md`. Sem isso, o próximo agente começa perdido.

## Regras

- Não confie cegamente no que está escrito; documentos ficam desatualizados.
- Não apague conteúdo escrito por humanos; marque como "revisar".
- Seja realista se o projeto está atrasado, grande demais ou parado.
