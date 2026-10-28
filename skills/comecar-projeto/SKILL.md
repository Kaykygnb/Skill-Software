---
name: comecar-projeto
description: Use quando o usuário quer iniciar, planejar ou criar um software/app/site novo, ou analisar um projeto sem docs/PROJETO.md. Cria o documento mestre docs/PROJETO.md e guia qual skill usar em cada etapa.
---

# Começar projeto

Responda em português do Brasil, simples. O usuário pode ser iniciante: explique termos técnicos na primeira vez e seja realista, sem enrolar.

Objetivo: qualquer pessoa ou agente que abrir o repositório entende em 5 minutos **o que o projeto é, o que deve fazer, em que ponto está e como continuar**. Isso fica em arquivos Markdown no projeto, não só na conversa.

## Primeiro: onde estamos?

1. Existe `docs/PROJETO.md`? Então use a skill **retomar-projeto** e pare aqui.
2. Existe código mas não existe docs/? **Modo mapear** (abaixo).
3. Não existe nada? **Modo novo** (abaixo).

## Mapa das skills (qual usar em cada etapa)

| Etapa | Skill | Resultado |
|---|---|---|
| 1. Ideia vaga | **descobrir-ideia** | entrevista guiada, visão do produto |
| 2. Ver como vai parecer | **prototipar** | telas e fluxo de navegação |
| 3. Definir o que construir | **requisitos** | docs/requisitos.md, MVP, tarefas |
| 4. Decidir como construir | **arquitetura** | docs/arquitetura.md, dados, tecnologias |
| 5. Desenhar | **diagramas** | docs/diagramas/*.md (Mermaid) |
| 6. Construir e conferir | **revisar-codigo** e **testes** | revisão e plano de testes |
| 7. Explicar para os outros | **documentar** | README, guias, API |
| Voltar ao projeto depois | **retomar-projeto** | lê PROJETO.md e continua |

Ao final de cada skill, sugira a próxima da tabela.

## Estrutura criada (só o que fizer sentido agora)

```
docs/
  PROJETO.md      <- documento mestre, sempre o primeiro a ler
  ideia.md        requisitos.md   arquitetura.md   entidades.md
  tarefas.md      decisoes.md     pendencias.md
  prototipo/      diagramas/      revisoes/
```

## Conteúdo obrigatório do docs/PROJETO.md

1. **O que é** (2 a 4 linhas) e para quem.
2. **Objetivo e escopo**: o que deve fazer e o que não fará.
3. **Estado atual** com data: fase (ideia, planejamento, desenvolvimento, produção).
4. **Planejamento**: tabela com áreas (ideia, protótipo, requisitos, arquitetura, dados, diagramas, testes, documentação), status Feito / Parcial / Falta e link para o MD.
5. **Stack e como rodar** (comandos reais, se existirem).
6. **Tarefas**: feitas, em andamento, próximas 5, com link para tarefas.md.
7. **O que falta planejar** e dúvidas abertas.
8. **Como prosseguir**: a próxima ação recomendada, em passos.
9. **Regras para agentes**: ler este arquivo primeiro; ao terminar qualquer trabalho, atualizar status, tarefas e data; não inventar requisitos; marcar suposições.
10. **Índice** de todos os MDs.

## Modo novo

Rode **descobrir-ideia**. Crie o PROJETO.md com o que souber e marque o resto como "Falta". Siga a tabela de etapas atualizando o PROJETO.md a cada uma.

## Modo mapear (projeto existente)

Leia README, arquivos de dependências, estrutura de pastas, ponto de entrada, rotas, modelos e migrations (entidades), integrações, testes e CI. Escreva o que achou com referência `arquivo:linha`. Separe fato de *(suposição)*. Registre dúvidas de regra de negócio em pendencias.md para o usuário confirmar. Gere entidades.md, arquitetura.md (como é hoje) e o PROJETO.md. Em projeto grande, diga o que não foi lido.

## Regras

- Nunca copie segredos (.env, chaves) para os docs.
- Não execute código desconhecido nem instale dependências sem avisar.
- Sem acesso para gravar arquivos, entregue o conteúdo em blocos por arquivo e avise.
- Seja realista no status: só marque Feito o que existe de fato.
- Termine dizendo a próxima ação recomendada.
