---
name: revisar-codigo
description: Use quando o usuário pedir para revisar, auditar ou avaliar código, um PR ou uma mudança. Procura bugs, falhas de segurança e problemas de qualidade, explica de forma simples e salva em docs/revisoes/.
---

# Revisar código

Responda em português do Brasil, simples e direto. Explique **por que** algo é problema, não só que é. Seja honesto, sem bajular, mas respeitoso.

## Passo a passo

1. **Contexto primeiro**: leia README, `docs/PROJETO.md`, `docs/entidades.md`, `docs/arquitetura.md` e os arquivos ligados ao trecho (quem chama, o que chama, modelos, testes). Se o projeto é desconhecido e grande, use **comecar-projeto** (modo mapear) antes. Se só recebeu um trecho colado, diga o que não deu para avaliar.
2. **Alvo**: PR, diff atual, arquivo/pasta ou projeto todo. No projeto todo, priorize login, acesso a dados, pagamentos e entradas do usuário.
3. Procure, nesta ordem:
   - **Bugs**: lógica, casos de borda, nulos, concorrência.
   - **Segurança**: segredos no código, SQL injection, XSS, entrada não validada, permissões, dependências vulneráveis.
   - **Robustez**: erros, falhas de rede, dados inválidos.
   - **Aderência ao design**: respeita entidades e regras documentadas?
   - **Legibilidade**: nomes, funções grandes, duplicação.
   - **Desempenho**: só se houver problema real.
   - **Testes**: o que importante está sem teste.
4. Classifique: Crítico, Importante, Sugestão.
5. Para cada achado: `arquivo:linha`, problema, por que importa, como corrigir (trecho curto).
6. Termine com 2 ou 3 pontos positivos reais (se houver) e o veredito: pode ir para produção ou não.
7. **Salve** em `docs/revisoes/AAAA-MM-DD-<alvo>.md` (se houver acesso) e atualize `docs/PROJETO.md` e `docs/tarefas.md` com as correções necessárias. Não altere o código sem o usuário pedir.

## Regras

- Não invente problemas; se está bom, diga.
- Separe fato de gosto pessoal.
- Diga o que não foi lido ou executado; revisão sem rodar testes não garante que funciona.
- Nunca copie segredos encontrados para o relatório; cite o local e recomende trocar a chave.
