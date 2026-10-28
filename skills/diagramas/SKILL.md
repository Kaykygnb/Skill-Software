---
name: diagramas
description: Use quando o usuário pedir diagramas de software: fluxo, sequência, classes, banco de dados (ER), arquitetura (C4), estados ou casos de uso. Gera em Mermaid e salva em docs/diagramas/.
---

# Diagramas

Responda em português do Brasil, simples. Gere diagramas em **Mermaid** (texto que o GitHub, Notion e mermaid.live desenham). Diga como visualizar em uma linha.

## Qual diagrama usar

| Pergunta | Diagrama | Mermaid |
|---|---|---|
| Como o sistema se divide? | Blocos / C4 | `flowchart` ou `C4Context` |
| Passo a passo de um processo? | Fluxograma | `flowchart TD` |
| Quem conversa com quem, em que ordem? | Sequência | `sequenceDiagram` |
| Classes e relações? | Classes (UML) | `classDiagram` |
| Banco de dados? | Entidade-relacionamento | `erDiagram` |
| Estados de um objeto? | Estados | `stateDiagram-v2` |
| O que cada usuário faz? | Casos de uso | `flowchart LR` com atores |
| Navegação entre telas? | Fluxo de telas | `flowchart LR` |

Sem pedido específico, sugira os 3 mais úteis: componentes, ER e sequência do fluxo principal.

## Fontes

1. Leia `docs/arquitetura.md`, `docs/entidades.md`, `docs/requisitos.md` e `docs/prototipo/` se existirem.
2. Se há código sem docs, leia modelos, migrations e rotas e cite os arquivos usados.
3. Sem nada, assuma o mínimo e declare as suposições.

## Passo a passo

1. Um diagrama por bloco ```mermaid, com título acima. Máximo ~15 nós; se maior, divida.
2. Explique em 2 a 4 linhas como ler cada um.
3. **Salve** um arquivo por diagrama em `docs/diagramas/` (ex.: `er-banco.md`, `sequencia-login.md`) com título, bloco Mermaid, explicação e data. Atualize em vez de duplicar. Sem acesso a arquivos, entregue o texto.
4. Atualize `docs/PROJETO.md` (tabela de planejamento e índice).
5. Pergunte o que falta ou está errado.

## Sintaxe (evitar erros)

- IDs sem espaço nem acento (`UsuarioApp`); texto visível entre aspas: `A["Cadastro de usuário"]`.
- Não use parênteses ou dois-pontos soltos em rótulos sem aspas.
- `erDiagram`: `||--o{` (um para muitos), `}o--o{` (muitos para muitos), rótulo entre aspas.
- `sequenceDiagram`: declare `participant` antes; use `alt/else` para alternativas.
- Valide com `npx @mermaid-js/mermaid-cli` quando houver terminal.

## Realismo

Diagrama é comunicação, não enfeite: se confunde, simplifique. Para edição visual, mencione draw.io ou Excalidraw; o Mermaid pode continuar como fonte no repositório.
