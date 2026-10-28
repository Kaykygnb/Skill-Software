# AGENTS.md — leia isto primeiro

Este repositório é um **pacote de skills** para ajudar uma pessoa a **projetar software**: descobrir a ideia, prototipar, definir requisitos e arquitetura, gerar diagramas, revisar código, testar e documentar.

## Quem é o usuário

Pessoa iniciante e um pouco ingênua em tecnologia, mora em Uberlândia/MG. Quer que você seja **direto e realista** (aponte furos, escopo grande demais, riscos), explique em **português do Brasil, simples e detalhado quando preciso**.

## O que você deve fazer

1. Se o usuário quer **criar** um software: siga `skills/comecar-projeto/SKILL.md`.
2. Se o projeto **já tem** `docs/PROJETO.md`: siga `skills/retomar-projeto/SKILL.md`.
3. Para as demais etapas, use a skill indicada pela tabela abaixo. Leia o `SKILL.md` dela antes de agir.

| Situação | Skill |
|---|---|
| Começar projeto novo ou mapear um existente | `skills/comecar-projeto` |
| Voltar a um projeto já documentado | `skills/retomar-projeto` |
| Ideia vaga, usuário não sabe o que quer | `skills/descobrir-ideia` |
| Ver como vai parecer (telas, fluxo) | `skills/prototipar` |
| Definir o que construir (MVP) | `skills/requisitos` |
| Decidir como construir (dados, tecnologias) | `skills/arquitetura` |
| Desenhar (Mermaid) | `skills/diagramas` |
| Revisar código | `skills/revisar-codigo` |
| Planejar e escrever testes | `skills/testes` |
| README, guias, API | `skills/documentar` |

## Regra central: tudo gira em torno do `docs/PROJETO.md`

No projeto do usuário (não neste repositório), mantenha `docs/PROJETO.md` como documento mestre: o que é, estado atual, o que foi planejado, o que falta, tarefas e próximo passo. **Ao terminar qualquer trabalho, atualize-o.** Assim o próximo agente entende tudo sem perguntar de novo.

## Regras gerais

- Nunca copie segredos (.env, chaves) para documentos.
- Não invente requisitos; marque suposições como *a validar*.
- Só marque algo como feito se existir de fato. Não diga que testes passaram sem rodá-los.
- Não execute código desconhecido nem instale dependências sem avisar.
- Ações irreversíveis (apagar, publicar, enviar a terceiros): peça confirmação.
