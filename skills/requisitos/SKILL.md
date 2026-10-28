---
name: requisitos
description: Use quando for definir o que o software deve fazer: requisitos funcionais e não funcionais, histórias de usuário, MVP, escopo e tarefas iniciais. Salva em docs/requisitos.md.
---

# Requisitos

Responda em português do Brasil, simples. Explique termos técnicos na primeira vez. Seja realista e direto; aponte furos e escopo grande demais.

## Antes de começar

Leia `docs/PROJETO.md`, `docs/ideia.md` e `docs/prototipo/` se existirem. Sem base, sugira **descobrir-ideia** primeiro, ou faça até 5 perguntas curtas. Se `docs/requisitos.md` existe, atualize em vez de recomeçar.

## Passo a passo

1. **Usuários (personas)**: 1 a 3 tipos e o que cada um quer fazer.
2. **Requisitos numerados**: funcionais (RF01...), não funcionais (RNF01...: desempenho, segurança, usabilidade, disponibilidade, custo, LGPD) e regras de negócio (RN01...). Cada um deve ser verificável: evite "rápido" ou "fácil" sem critério.
3. **Histórias de usuário**: "Como <usuário>, quero <ação> para <benefício>", com critérios de aceite.
4. **Prioridade MoSCoW** (Deve, Deveria, Poderia, Não agora) e **MVP**: versão mínima que já entrega valor. Seja duro: se o MVP é grande para quem vai construir, corte.
5. **Fora do escopo, riscos e perguntas em aberto.**

## Salvar

`docs/requisitos.md` com: Visão geral, Usuários, RF, RNF, Regras, Histórias, MVP, Fora do escopo, Riscos, Perguntas. Gere `docs/tarefas.md` com uma tarefa por história do MVP (status: a fazer). Atualize `docs/PROJETO.md` (status, perguntas, próxima ação, data). Próxima skill: **arquitetura**.

## Regras

- Não invente requisitos como se o usuário tivesse pedido; marque sugestões suas.
- Marque suposições como *a validar*.
