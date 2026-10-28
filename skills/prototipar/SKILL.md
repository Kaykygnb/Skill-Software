---
name: prototipar
description: Use quando o usuário quer ver como o software vai parecer: telas, navegação, wireframes ou protótipo clicável. Cria rascunhos de telas e fluxo para o usuário reagir antes de construir.
---

# Prototipar

Responda em português do Brasil, simples. Protótipo é um rascunho para **descobrir o que o usuário quer ver** antes de gastar tempo programando. Mostre algo cedo e peça reação ("é isso? o que muda?").

## Passo a passo

1. Leia `docs/PROJETO.md`, `docs/ideia.md` e `docs/requisitos.md` se existirem. Se não houver nada, faça 3 perguntas rápidas: quem usa, as 3 ações principais, celular ou computador.
2. **Liste as telas** necessárias (ex.: login, início, lista, detalhe, cadastro) e o **fluxo**: de qual tela vai para qual. Desenhe o fluxo em Mermaid (`flowchart LR`).
3. **Desenhe cada tela** em um destes níveis, perguntando ao usuário qual prefere (padrão: nível A):
   - **A. Wireframe em texto** (caixas e rótulos em bloco de código): rápido, serve para decidir conteúdo e organização.
   - **B. Protótipo HTML clicável** de um arquivo só (`docs/prototipo/index.html`), simples, sem bibliotecas, com navegação entre telas, aberto direto no navegador.
   - **C. Descrição para Figma** (lista de componentes, textos, cores) caso o usuário queira refinar lá.
4. Mostre uma tela ou um fluxo por vez e pergunte: o que está faltando? o que está sobrando? está claro para quem vai usar?
5. Registre as decisões de interface (o que ficou, o que mudou, por quê) em `docs/prototipo/decisoes-de-tela.md`.
6. Atualize `docs/PROJETO.md` e sugira **requisitos**: as telas aprovadas viram funções e histórias de usuário.

## Regras

- Protótipo não é o produto: avise que não tem lógica real nem dados reais.
- Foco em clareza e poucos elementos por tela; não gaste tempo com enfeite.
- Pense em celular primeiro quando o público for o cidadão comum no Brasil.
- Não escolha por ele: apresente 2 opções quando houver dúvida de layout.
