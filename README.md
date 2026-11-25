# Agent Working Principles

Skills curtas para colaborar com agentes de IA na definição e implementação de produtos. Os princípios são independentes de pessoa, empresa ou framework.

## Skills

- [Definição e implementação](skills/definition-and-implementation/SKILL.md): ciclos rápidos de definição com a pessoa responsável e execução autônoma quando a direção estiver suficientemente clara e autorizada.
- [Direção de design de interfaces](skills/interface-design-direction/SKILL.md): coerência entre telas, reutilização de estruturas comuns e estabilidade visual durante o carregamento.
- [Preferência por Astro + Cloudflare](skills/astro-cloudflare-preference/SKILL.md): orientação opcional para quem prefere essa stack ao iniciar projetos web; preserva escolhas explícitas e stacks existentes.

Este repositório é **público**. Tenha cuidado com o conteúdo e as mensagens dos commits; compartilhe apenas material genérico, sem informações privadas.

## Uso

Cada diretório em `skills/` contém uma skill completa. Instale os diretórios desejados no local de skills reconhecido pelo seu agente, preservando o `SKILL.md` e seus arquivos de apoio. Os arquivos `agents/openai.yaml` fornecem metadados opcionais para Codex; os princípios estão nos arquivos Markdown.

Para agentes sem descoberta de skills, forneça o `SKILL.md` relevante como instrução. Uma orientação curta no projeto pode tornar o uso recorrente:

> Use `definition-and-implementation` para orientar a colaboração. Ao criar, alterar ou revisar interfaces, aplique também `interface-design-direction`, junto à identidade e à direção de design do projeto.

As skills orientam decisões conforme o contexto e a autorização recebida. Não exigem fases de gestão ou issues; a preferência opcional de stack não impõe tecnologia aos demais fluxos.

## Contribuição

Mantenha as instruções abstratas, curtas e fundamentadas em necessidades reais. Prefira corrigir o princípio existente a acumular regras particulares. Exemplos devem esclarecer decisões, sem impor ferramentas ou processos desnecessários.

Para ativar o lembrete local antes de cada push, execute na raiz do clone:

```sh
git config core.hooksPath .githooks
```

Se o clone já tiver hooks configurados, preserve-os e incorpore este aviso ao fluxo existente. O hook exibe um aviso; a revisão do conteúdo continua sendo responsabilidade de quem publica.
