---
name: arquitetura
description: Use quando for decidir como construir o software: estrutura, banco de dados, tecnologias, hospedagem, custos e trade-offs. Salva em docs/arquitetura.md, entidades.md e decisoes.md.
---

# Arquitetura

Responda em português do Brasil, simples. Explique cada conceito (API, banco relacional, monólito...) em uma frase. Seja realista: recomende a opção **mais simples que atende**, não a mais moderna.

## Antes de começar

Leia `docs/PROJETO.md` e `docs/requisitos.md`. Sem requisitos, use a skill **requisitos** ou pergunte o mínimo (o que faz, quantos usuários, onde roda, orçamento, quem mantém). Se já existe código, documente a arquitetura real antes de propor mudanças.

## Passo a passo

1. **Estilo geral**: compare 2 ou 3 opções (monólito simples, modular, serviços, serverless). Para equipe pequena, recomende monólito e explique. Microsserviços só com motivo concreto.
2. **Componentes**: responsabilidade, entradas, saídas, com quem conversa.
3. **Dados**: entidades, relacionamentos, banco (relacional por padrão; NoSQL só se compensar).
4. **Tecnologias**: linguagem, framework, banco, hospedagem, login. Considere o que o usuário já conhece e o custo mensal em reais (o usuário mora em Uberlândia/MG; muita hospedagem cobra em dólar). Custos são estimativas em faixas.
5. **Não funcionais**: segurança, backup, desempenho, logs, LGPD.
6. **Decisões** como mini-ADR: contexto, opções, escolha, consequências.
7. **Riscos e evolução**: o que quebra primeiro se crescer.

## Salvar

`docs/arquitetura.md`, `docs/entidades.md`, `docs/decisoes.md`. Acrescente tarefas técnicas em `docs/tarefas.md`. Atualize `docs/PROJETO.md` (stack, status, próxima ação, data). Próxima skill: **diagramas**.

## Regras

- Avise quando a ideia é grande demais para o tamanho da equipe.
- Diferencie fato de opinião; não invente números como certos.
