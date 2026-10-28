# Pacote de skills para projetar software

Skills em português para o Claude (e outros agentes) ajudarem a **descobrir, planejar, prototipar, desenhar, revisar, testar e documentar** um software, tudo organizado em `docs/PROJETO.md`.

## Skills

`comecar-projeto`, `retomar-projeto`, `descobrir-ideia`, `prototipar`, `requisitos`, `arquitetura`, `diagramas`, `revisar-codigo`, `testes`, `documentar`. Veja `AGENTS.md` para quando usar cada uma.

## Como baixar

```bash
git clone https://github.com/Kaykygnb/Skill-Software.git
```

## Como instalar no Claude Code

Para todos os seus projetos:
```bash
mkdir -p ~/.claude/skills
cp -r Skill-Software/skills/* ~/.claude/skills/
```
Para um projeto só: copie para `.claude/skills/` dentro dele.

## Como usar com qualquer agente

Abra o agente na pasta do projeto e diga: "leia AGENTS.md do pacote e me ajude a começar um projeto". Também funciona colocando este repositório dentro do seu projeto ou apontando o agente para ele.

## Limites

Ativação automática das skills não é 100%: se não disparar, peça pelo nome (ex.: "use a skill comecar-projeto").
