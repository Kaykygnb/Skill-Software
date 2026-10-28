---
name: testes
description: Use quando o usuário quiser planejar ou escrever testes de um software: casos de teste a partir dos requisitos, tipos de teste e ferramentas gratuitas. Salva em docs/testes.md.
---

# Testes

Responda em português do Brasil, simples. Seja realista: teste não prova que não há bugs, só reduz o risco.

## Passo a passo

1. Leia `docs/PROJETO.md`, `docs/requisitos.md` (critérios de aceite) e o código. Sem requisitos, use **requisitos** ou pergunte o essencial.
2. Pergunte ou descubra a linguagem e sugira ferramentas gratuitas (Jest/Vitest para JavaScript, pytest para Python, JUnit para Java, Playwright para navegador).
3. Monte a **pirâmide**: muitos testes unitários (funções isoladas), alguns de integração (partes juntas, banco), poucos ponta a ponta (fluxo completo).
4. Tabela de casos: ID, requisito, cenário, entrada, resultado esperado, tipo, prioridade.
5. Inclua bordas e erros: campos vazios, valores extremos, sem permissão, falha de rede, duplicados.
6. Liste testes básicos de segurança (login, permissões, entrada maliciosa) e de desempenho se relevante.
7. Se pedido, escreva o código dos testes mais importantes e, se houver terminal, rode-os e informe o resultado real.

## Salvar

`docs/testes.md` (estratégia, ferramentas, tabela, riscos não cobertos, como rodar). Atualize `docs/PROJETO.md` e `docs/tarefas.md`.

## Regras

- Priorize o que mais dói se quebrar; não exija 100% de cobertura em projeto pequeno.
- Nunca diga que testes passaram sem tê-los rodado.
