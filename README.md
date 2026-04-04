<div align="center">

<!-- HEADER -->
<br>

```
██████╗ ███████╗██╗   ██╗    ███████╗██╗  ██╗██╗██╗     ██╗     ███████╗
██╔══██╗██╔════╝██║   ██║    ██╔════╝██║ ██╔╝██║██║     ██║     ██╔════╝
██║  ██║█████╗  ██║   ██║    ███████╗█████╔╝ ██║██║     ██║     ███████╗
██║  ██║██╔══╝  ╚██╗ ██╔╝    ╚════██║██╔═██╗ ██║██║     ██║     ╚════██║
██████╔╝███████╗ ╚████╔╝     ███████║██║  ██╗██║███████╗███████╗███████║
╚═════╝ ╚══════╝  ╚═══╝      ╚══════╝╚═╝  ╚═╝╚═╝╚══════╝╚══════╝╚══════╝
```

**Base de Conhecimento Operacional para Agentes de IA**

<sub>20 agentes especialistas | 36+ skills modulares | 11 workflows | 13 templates | 7 skills n8n</sub>

<br>

![Agentes](https://img.shields.io/badge/agentes-20-00d4ff?style=for-the-badge&labelColor=0a0a0a)
![Skills](https://img.shields.io/badge/skills-36+-00ffa3?style=for-the-badge&labelColor=0a0a0a)
![Workflows](https://img.shields.io/badge/workflows-11-ff6b35?style=for-the-badge&labelColor=0a0a0a)
![Templates](https://img.shields.io/badge/templates-13-c084fc?style=for-the-badge&labelColor=0a0a0a)
![Cobertura](https://img.shields.io/badge/cobertura-~90%25_web%2Fmobile-00d4ff?style=for-the-badge&labelColor=0a0a0a)

---

</div>

## O que e este projeto

O **dev-skills** e uma base de conhecimento modular que transforma agentes de IA em especialistas de desenvolvimento. Em vez de depender de respostas genericas, o agente consulta arquivos especificos por dominio e executa com precisao, contexto e consistencia.

O sistema opera como um **kit de expansao cognitiva**: agentes especialistas carregam skills sob demanda, seguem workflows estruturados e respeitam regras globais de qualidade.

<br>

## Para quem serve

| Perfil | Como usar |
|--------|-----------|
| **Desenvolvedor solo** | Clone e aponte seu agente para os arquivos do dominio. Receba orientacao especializada em frontend, backend, mobile, banco, seguranca, testes e mais. |
| **Time de engenharia** | Use como base padronizada de conhecimento para manter consistencia entre agentes e projetos. |
| **Quem usa n8n** | Acesse o pacote `n8n-skills/` com 7 skills especializadas para construir workflows profissionais. |
| **Quem quer aprender** | Leia os agents e skills como material de referencia tecnica por dominio. |

<br>

---

## Arquitetura de Conhecimento

```
dev-skills/
├── .agent/                          # Nucleo principal do sistema
│   ├── ARCHITECTURE.md              # Mapa completo de agentes, skills e workflows
│   ├── rules/GEMINI.md              # Regras globais de comportamento
│   ├── agents/                      # 20 agentes especialistas
│   ├── skills/                      # 36+ skills modulares por dominio
│   ├── workflows/                   # 11 comandos slash (/create, /plan, /debug...)
│   ├── scripts/                     # Scripts mestres de validacao
│   └── .shared/ui-ux-pro-max/      # Base visual: 50 estilos, 21 paletas, 50 fontes
│
├── agents/                          # Copias operacionais dos agentes
│   ├── fullstack/                   # Fullstack (frontend-design, app-builder)
│   └── Mobile/                      # Mobile (mobile-design)
│
├── n8n-skills/                      # Pacote especializado para n8n
│   ├── skills/                      # 7 skills n8n
│   ├── docs/                        # Documentacao n8n
│   └── evaluations/                 # Cenarios de teste
│
├── docs/                            # Documentacao do projeto
│   ├── regras-totais.md             # Todas as regras consolidadas
│   ├── guia-de-aprendizado-do-agent.md
│   └── mapa-de-roteamento.md        # Indice operacional por assunto
│
├── agente_mestre_regras_aprendizado.md  # Documento mestre do agente
└── README.md                        # Este arquivo
```

<br>

---

## Os 20 Agentes Especialistas

Cada agente e uma persona tecnica focada em um dominio. O agente carrega suas skills automaticamente via frontmatter.

| Agente | Dominio | Skills carregadas |
|--------|---------|-------------------|
| `orchestrator` | Coordenacao multi-agente | parallel-agents, behavioral-modes, architecture |
| `project-planner` | Planejamento e descoberta | brainstorming, plan-writing, architecture |
| `frontend-specialist` | Interface web e UI/UX | frontend-design, tailwind-patterns |
| `backend-specialist` | API e logica de servidor | api-patterns, nodejs-best-practices, database-design |
| `database-architect` | Modelagem e SQL | database-design |
| `mobile-developer` | iOS, Android, React Native | mobile-design |
| `game-developer` | Logica de jogo e mecanica | game-development |
| `devops-engineer` | CI/CD e infraestrutura | deployment-procedures |
| `security-auditor` | Seguranca e conformidade | vulnerability-scanner, red-team-tactics |
| `penetration-tester` | Seguranca ofensiva | red-team-tactics |
| `test-engineer` | Estrategia de testes | testing-patterns, tdd-workflow, webapp-testing |
| `qa-automation-engineer` | Testes E2E e pipelines | webapp-testing, testing-patterns |
| `debugger` | Analise de causa raiz | systematic-debugging |
| `performance-optimizer` | Velocidade e Web Vitals | performance-profiling |
| `seo-specialist` | Ranking e visibilidade | seo-fundamentals, geo-fundamentals |
| `documentation-writer` | Manuais e documentacao | documentation-templates |
| `product-manager` | Requisitos e historias | plan-writing, brainstorming |
| `product-owner` | Estrategia e backlog | plan-writing, brainstorming |
| `code-archaeologist` | Codigo legado e refatoracao | clean-code, code-review-checklist |
| `explorer-agent` | Analise de codebase | - |

<br>

---

## Skills por Dominio

### Frontend e UI

| Skill | Descricao |
|-------|-----------|
| `frontend-design` | Padroes UI/UX, design system, animacao, tipografia, psicologia UX, efeitos visuais |
| `nextjs-react-expert` | 9 modulos de performance React/Next.js (waterfalls, bundle, SSR, cache, re-render) |
| `tailwind-patterns` | Utilitarios Tailwind CSS v4 |
| `web-design-guidelines` | Auditoria web: 100+ regras de acessibilidade, UX e performance |
| `ui-ux-pro-max` | Base visual compartilhada: 50 estilos, 21 paletas, 50 fontes, 12 stacks |

### Backend e API

| Skill | Descricao |
|-------|-----------|
| `api-patterns` | REST, GraphQL, tRPC, autenticacao, rate limiting, versionamento |
| `nodejs-best-practices` | Node.js async, modulos, padroes |
| `python-patterns` | Python, FastAPI, padroes |

### Banco de Dados

| Skill | Descricao |
|-------|-----------|
| `database-design` | Schema, indexacao, migracoes, otimizacao, selecao de ORM |

### Mobile

| Skill | Descricao |
|-------|-----------|
| `mobile-design` | UI/UX mobile, navegacao, performance, testes, plataforma Android/iOS, psicologia touch |

### Arquitetura e Planejamento

| Skill | Descricao |
|-------|-----------|
| `architecture` | Padroes de sistema, trade-offs, selecao de padroes |
| `app-builder` | Scaffolding fullstack com 13 templates prontos |
| `plan-writing` | Planejamento e decomposicao de tarefas |
| `brainstorming` | Descoberta socratica |

### Testes e Qualidade

| Skill | Descricao |
|-------|-----------|
| `testing-patterns` | Jest, Vitest, estrategias de teste |
| `webapp-testing` | E2E com Playwright |
| `tdd-workflow` | Desenvolvimento orientado a testes |
| `code-review-checklist` | Padroes de revisao de codigo |
| `lint-and-validate` | Linting e validacao |

### Seguranca

| Skill | Descricao |
|-------|-----------|
| `vulnerability-scanner` | Auditoria OWASP, checklists |
| `red-team-tactics` | Seguranca ofensiva |

### DevOps e Infraestrutura

| Skill | Descricao |
|-------|-----------|
| `deployment-procedures` | CI/CD e deploy |
| `server-management` | Gestao de infraestrutura |
| `bash-linux` | Comandos Linux e scripting |
| `powershell-windows` | PowerShell Windows |

### Outros

| Skill | Descricao |
|-------|-----------|
| `clean-code` | Padroes de codigo limpo (global) |
| `game-development` | Logica de jogo, 2D, 3D, multiplayer, VR/AR |
| `seo-fundamentals` | SEO, E-E-A-T, Core Web Vitals |
| `i18n-localization` | Internacionalizacao |
| `mcp-builder` | Model Context Protocol |
| `performance-profiling` | Web Vitals e otimizacao |
| `systematic-debugging` | Depuracao sistematica |

<br>

---

## 11 Workflows (Comandos Slash)

Workflows sao procedimentos invocados por comando. Definem o fluxo operacional do agente.

| Comando | Funcao |
|---------|--------|
| `/brainstorm` | Descoberta socratica |
| `/create` | Criar nova aplicacao |
| `/debug` | Depurar problemas |
| `/deploy` | Deploy da aplicacao |
| `/enhance` | Melhorar codigo existente |
| `/orchestrate` | Coordenacao multi-agente |
| `/plan` | Planejamento de tarefas |
| `/preview` | Pre-visualizar mudancas |
| `/status` | Status do projeto |
| `/test` | Executar testes |
| `/ui-ux-pro-max` | Design com 50 estilos |

<br>

---

## 13 Templates de Projeto

O `app-builder` inclui templates prontos para scaffolding rapido:

| Template | Stack |
|----------|-------|
| `nextjs-fullstack` | Next.js com API routes |
| `nextjs-saas` | Next.js SaaS |
| `nextjs-static` | Next.js estatico |
| `express-api` | Express.js API |
| `python-fastapi` | Python FastAPI |
| `react-native-app` | React Native |
| `flutter-app` | Flutter |
| `nuxt-app` | Nuxt.js |
| `astro-static` | Astro estatico |
| `electron-desktop` | Electron desktop |
| `chrome-extension` | Extensao Chrome |
| `cli-tool` | Ferramenta CLI |
| `monorepo-turborepo` | Monorepo Turborepo |

<br>

---

## Pacote n8n-skills

Pacote especializado com 7 skills para construir workflows n8n profissionais usando o servidor MCP n8n-mcp.

| Skill | Foco |
|-------|------|
| `n8n-expression-syntax` | Sintaxe de expressoes n8n |
| `n8n-mcp-tools-expert` | Uso eficiente das ferramentas MCP |
| `n8n-workflow-patterns` | Padroes arquiteturais de workflow |
| `n8n-validation-expert` | Interpretacao de erros de validacao |
| `n8n-node-configuration` | Configuracao de nodes |
| `n8n-code-javascript` | JavaScript em Code nodes |
| `n8n-code-python` | Python em Code nodes |

Documentacao completa em `n8n-skills/docs/`.

<br>

---

## Roteamento por Assunto

A tabela abaixo mostra exatamente onde o agente deve buscar conhecimento para cada tipo de tarefa. Para o mapa completo com todos os caminhos, consulte [`docs/mapa-de-roteamento.md`](docs/mapa-de-roteamento.md).

| Assunto | Agente principal | Primeiro arquivo a ler |
|---------|------------------|------------------------|
| Frontend / UI | `frontend-specialist` | `.agent/skills/frontend-design/SKILL.md` |
| Backend / API | `backend-specialist` | `.agent/skills/api-patterns/SKILL.md` |
| Banco de dados | `database-architect` | `.agent/skills/database-design/SKILL.md` |
| Mobile | `mobile-developer` | `.agent/skills/mobile-design/SKILL.md` |
| Arquitetura | `orchestrator` | `.agent/skills/architecture/SKILL.md` |
| Testes | `test-engineer` | `.agent/skills/testing-patterns/SKILL.md` |
| Seguranca | `security-auditor` | `.agent/skills/vulnerability-scanner/SKILL.md` |
| Performance | `performance-optimizer` | `.agent/skills/performance-profiling/SKILL.md` |
| DevOps / Deploy | `devops-engineer` | `.agent/skills/deployment-procedures/SKILL.md` |
| Debugging | `debugger` | `.agent/skills/systematic-debugging/SKILL.md` |
| Documentacao | `documentation-writer` | `.agent/skills/documentation-templates/SKILL.md` |
| Planejamento | `project-planner` | `.agent/skills/plan-writing/SKILL.md` |
| n8n | - | `n8n-skills/skills/.../SKILL.md` |
| Jogo | `game-developer` | `.agent/skills/game-development/SKILL.md` |
| UI/UX Premium | `frontend-specialist` | `.agent/.shared/ui-ux-pro-max/data/` |
| App novo | `orchestrator` | `.agent/skills/app-builder/SKILL.md` |

<br>

---

## Como Comecar

### 1. Clone o repositorio

```bash
git clone https://github.com/LucasLgomes/dev-skills.git
cd dev-skills
```

### 2. Aponte o agente para o documento mestre

Ao iniciar uma sessao com qualquer agente de IA, peca para ele ler o arquivo principal:

```
Leia o arquivo agente_mestre_regras_aprendizado.md e siga todas as regras.
```

Esse arquivo contem:
- todas as regras globais de idioma, nomenclatura e qualidade;
- a ordem obrigatoria de leitura antes de qualquer tarefa;
- o roteamento completo por assunto com caminhos exatos;
- o algoritmo operacional que o agente deve seguir;
- politicas de releitura e validacao.

### 3. Peça uma tarefa especifica

```
Preciso criar uma API REST com autenticacao JWT. 
Consulte os arquivos corretos e siga as regras do projeto.
```

O agente vai:
1. Classificar a tarefa (backend + seguranca);
2. Consultar `GEMINI.md` para regras globais;
3. Ler `backend-specialist.md` e `security-auditor.md`;
4. Carregar `api-patterns/SKILL.md` e `api-patterns/auth.md`;
5. Executar seguindo todas as regras de qualidade.

<br>

---

## Scripts de Validacao

O projeto inclui scripts mestres para verificacao automatizada:

| Script | Uso | Quando executar |
|--------|-----|-----------------|
| `checklist.py` | Validacao por prioridade (seguranca, lint, schema, testes, UX, SEO) | Durante desenvolvimento |
| `verify_all.py` | Verificacao completa (tudo acima + Lighthouse, E2E, bundle, mobile) | Antes de deploy |

```bash
# Validacao rapida
python .agent/scripts/checklist.py .

# Verificacao completa
python .agent/scripts/verify_all.py . --url http://localhost:3000
```

<br>

---

## Protocolo de Carregamento de Skills

```
Requisicao do usuario
       |
       v
Identificar dominio → Selecionar agente → Ler frontmatter "skills:"
       |
       v
Carregar SKILL.md (indice) → Ler somente secoes relevantes
       |
       v
Aplicar regras → Executar
```

Prioridade de regras:
1. **P0** — `GEMINI.md` (regras globais)
2. **P1** — Arquivo do agente (`.agent/agents/*.md`)
3. **P2** — `SKILL.md` (skill especifica)

<br>

---

## Documentacao Complementar

| Documento | Conteudo |
|-----------|----------|
| [`agente_mestre_regras_aprendizado.md`](agente_mestre_regras_aprendizado.md) | Documento mestre com todas as regras, roteamento completo e algoritmo operacional |
| [`docs/regras-totais.md`](docs/regras-totais.md) | Consolidacao de todas as regras operacionais |
| [`docs/guia-de-aprendizado-do-agent.md`](docs/guia-de-aprendizado-do-agent.md) | Como o agente aprende com o repositorio |
| [`docs/mapa-de-roteamento.md`](docs/mapa-de-roteamento.md) | Indice operacional: qual arquivo ler para cada assunto |
| [`.agent/ARCHITECTURE.md`](.agent/ARCHITECTURE.md) | Mapa tecnico completo de agentes, skills e workflows |
| [`.agent/rules/GEMINI.md`](.agent/rules/GEMINI.md) | Regras globais de comportamento do agente |

<br>

---

## Contribuicao

### Para adicionar um novo agente

1. Crie o arquivo em `.agent/agents/nome-do-agente.md`
2. Defina o frontmatter com `name`, `description`, `skills`
3. Atualize `ARCHITECTURE.md`

### Para adicionar uma nova skill

1. Crie a pasta em `.agent/skills/nome-da-skill/`
2. Crie o `SKILL.md` com frontmatter e instrucoes
3. Adicione arquivos complementares conforme necessario
4. Atualize `ARCHITECTURE.md`

### Para adicionar um novo workflow

1. Crie o arquivo em `.agent/workflows/nome.md`
2. Defina `description` no frontmatter
3. Atualize `ARCHITECTURE.md`

<br>

---

## Git

```bash
# Clonar
git clone https://github.com/LucasLgomes/dev-skills.git

# Verificar status
git status

# Adicionar mudancas
git add .

# Commit
git commit -m "descricao clara da mudanca"

# Enviar
git push origin main
```

<br>

---

## Regras Fundamentais

- **Idioma:** Portugues do Brasil para toda comunicacao e codigo
- **Fuso horario:** America/Sao_Paulo
- **Nomenclatura:** Nomes claros, completos, sem abreviacoes confusas
- **Fonte da verdade:** Os arquivos do repositorio sempre vencem suposicoes
- **Releitura obrigatoria:** O agente deve reler os arquivos corretos antes de cada tarefa
- **Sem improviso:** Se existe arquivo especializado sobre o tema, ele tem prioridade

<br>

---

<div align="center">

<sub>Construido como base de conhecimento operacional para agentes de IA</sub>

<sub>20 agentes | 36+ skills | 11 workflows | 13 templates | 7 skills n8n</sub>

</div>
