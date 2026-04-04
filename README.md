<div align="center">

<br>

```text
██████╗ ███████╗██╗   ██╗    ███████╗██╗  ██╗██╗██╗     ██╗     ███████╗
██╔══██╗██╔════╝██║   ██║    ██╔════╝██║ ██╔╝██║██║     ██║     ██╔════╝
██║  ██║█████╗  ██║   ██║    ███████╗█████╔╝ ██║██║     ██║     ███████╗
██║  ██║██╔══╝  ╚██╗ ██╔╝     ╚════██║██╔═██╗ ██║██║     ██║     ╚════██║
██████╔╝███████╗ ╚████╔╝      ███████║██║  ██╗██║███████╗███████╗███████║
╚═════╝ ╚══════╝  ╚═══╝       ╚══════╝╚═╝  ╚═╝╚═╝╚══════╝╚══════╝╚══════╝
```

# dev-skills

**Base de Conhecimento Operacional para Agentes de IA**

<sub>Um repositório pensado para transformar agentes em especialistas reais por domínio, com leitura orientada, roteamento por contexto e execução com consistência.</sub>

<br>

![Agentes](https://img.shields.io/badge/agentes-20-00d4ff?style=for-the-badge&labelColor=0b0b0f)
![Skills](https://img.shields.io/badge/skills-36+-00ffa3?style=for-the-badge&labelColor=0b0b0f)
![Workflows](https://img.shields.io/badge/workflows-11-ff7a59?style=for-the-badge&labelColor=0b0b0f)
![Templates](https://img.shields.io/badge/templates-13-c084fc?style=for-the-badge&labelColor=0b0b0f)
![n8n](https://img.shields.io/badge/n8n_skills-7-ffcc00?style=for-the-badge&labelColor=0b0b0f)

<br>

![Python](https://img.shields.io/badge/python-base-1f6feb?style=flat-square&labelColor=0b0b0f)
![Arquitetura](https://img.shields.io/badge/arquitetura-modular-00d4ff?style=flat-square&labelColor=0b0b0f)
![Documentação](https://img.shields.io/badge/documenta%C3%A7%C3%A3o-orientada_a_uso-00ffa3?style=flat-square&labelColor=0b0b0f)
![Git](https://img.shields.io/badge/git-pronto_para_versionamento-c084fc?style=flat-square&labelColor=0b0b0f)

</div>

---

## Visão geral

O **dev-skills** é uma base de conhecimento modular criada para agentes de IA que precisam trabalhar com mais precisão, contexto e especialização.

Em vez de depender de respostas genéricas, o agente passa a:

- identificar o domínio do problema;
- consultar os arquivos corretos do repositório;
- carregar agentes e skills especializadas;
- seguir workflows estruturados;
- executar respeitando regras globais de qualidade.

Na prática, este projeto funciona como uma **camada operacional de inteligência**, onde o agente aprende por **releitura contextual** e não por improviso.

---

## O que este projeto resolve

Muitos agentes erram porque tentam responder apenas com memória, sem consultar a fonte correta. Este repositório corrige isso com uma arquitetura onde:

- cada assunto possui arquivos especializados;
- cada agente tem um papel técnico claro;
- cada skill tem escopo definido;
- cada workflow organiza a execução;
- as regras globais mantêm consistência entre tarefas e projetos.

O resultado é um ecossistema em que o agente consegue atuar com muito mais coerência em temas como frontend, backend, arquitetura, mobile, banco de dados, testes, segurança, performance, documentação e n8n.

---

## Para quem serve

| Perfil | Como este repositório ajuda |
|---|---|
| **Desenvolvedor solo** | Permite usar agentes com muito mais profundidade técnica, consultando as fontes certas para cada tarefa. |
| **Times de engenharia** | Ajuda a padronizar a forma como agentes e automações tomam decisões dentro de múltiplos projetos. |
| **Quem usa n8n** | Entrega um pacote dedicado com skills, documentação e padrões específicos para workflows n8n. |
| **Quem está estudando** | Funciona como um acervo técnico organizado por domínio, com trilhas claras de leitura. |
| **Quem quer criar seus próprios agents** | Serve como referência prática para estruturar agentes, skills, workflows e regras globais. |

---

## Princípio central

> **O agente nunca deve depender apenas da memória.**  
> Ele deve reler os arquivos corretos sempre que o domínio do problema mudar.

Esse é o coração do projeto.

---

## Arquitetura de conhecimento

```text
dev-skills/
├── .agent/                                # Núcleo principal do sistema
│   ├── ARCHITECTURE.md                    # Mapa técnico do ecossistema
│   ├── rules/GEMINI.md                    # Regras globais de comportamento
│   ├── agents/                            # Agentes especialistas
│   ├── skills/                            # Skills modulares por domínio
│   ├── workflows/                         # Fluxos operacionais por comando
│   ├── scripts/                           # Scripts de verificação e apoio
│   └── .shared/ui-ux-pro-max/             # Base visual compartilhada
│
├── agents/                                # Cópias operacionais e agrupamentos
│   ├── fullstack/
│   └── Mobile/
│
├── docs/                                  # Documentação central do projeto
│   ├── regras-totais.md
│   ├── guia-de-aprendizado-do-agent.md
│   └── mapa-de-roteamento.md
│
├── n8n-skills/                            # Pacote especializado para n8n
│   ├── docs/
│   ├── evaluations/
│   ├── skills/
│   └── dist/
│
├── agente_mestre_regras_aprendizado.md    # Documento mestre para o agent
└── README.md                              # Porta de entrada do projeto
```

---

## Como o ecossistema funciona

O repositório é organizado em quatro pilares:

### 1. Agentes
São personas técnicas especializadas, cada uma focada em um domínio específico.

### 2. Skills
São módulos de conhecimento acionados sob demanda para resolver tarefas com profundidade.

### 3. Workflows
São procedimentos operacionais que organizam como o agente deve executar determinadas ações.

### 4. Regras globais
São os critérios de comportamento, linguagem, consistência e prioridade de leitura.

---

## Os agentes especialistas

Cada agente atua como um especialista técnico de referência.

| Agente | Domínio principal | Função prática |
|---|---|---|
| `orchestrator` | Coordenação multiagente | Organiza tarefas complexas e distribui responsabilidades |
| `project-planner` | Planejamento | Estrutura etapas, escopo e execução |
| `frontend-specialist` | Frontend e UI/UX | Resolve interface, experiência, design e implementação visual |
| `backend-specialist` | Backend e APIs | Atua em lógica de servidor, contratos, autenticação e integração |
| `database-architect` | Banco de dados | Modelagem, schema, índices, migrações e performance |
| `mobile-developer` | Mobile | Android, iOS, navegação, UI mobile e arquitetura |
| `game-developer` | Games | Estruturação e lógica de desenvolvimento de jogos |
| `devops-engineer` | DevOps e infraestrutura | Deploy, automação, servidores e pipelines |
| `security-auditor` | Segurança defensiva | Auditoria, hardening, boas práticas e verificação |
| `penetration-tester` | Segurança ofensiva | Simulação de ataque e análise ofensiva |
| `test-engineer` | Testes | Estratégia, cobertura, qualidade e validação |
| `qa-automation-engineer` | QA e automação | Testes automatizados e fluxos E2E |
| `debugger` | Depuração | Investigação de causa raiz |
| `performance-optimizer` | Performance | Web Vitals, renderização e otimização |
| `seo-specialist` | SEO | Visibilidade, estrutura e sinais técnicos |
| `documentation-writer` | Documentação | Escrita técnica e padronização documental |
| `product-manager` | Produto | Requisitos, valor, alinhamento e priorização |
| `product-owner` | Backlog e estratégia | Direção de produto e evolução |
| `code-archaeologist` | Código legado | Leitura, entendimento e refatoração de bases existentes |
| `explorer-agent` | Exploração de codebase | Mapeamento e leitura inicial do repositório |

---

## Skills por domínio

### Frontend e UI
- `frontend-design`
- `nextjs-react-expert`
- `tailwind-patterns`
- `web-design-guidelines`
- `ui-ux-pro-max`

### Backend e API
- `api-patterns`
- `nodejs-best-practices`
- `python-patterns`

### Banco de dados
- `database-design`

### Mobile
- `mobile-design`

### Arquitetura e planejamento
- `architecture`
- `app-builder`
- `plan-writing`
- `brainstorming`

### Testes e qualidade
- `testing-patterns`
- `webapp-testing`
- `tdd-workflow`
- `code-review-checklist`
- `lint-and-validate`

### Segurança
- `vulnerability-scanner`
- `red-team-tactics`

### DevOps e infraestrutura
- `deployment-procedures`
- `server-management`
- `bash-linux`
- `powershell-windows`

### Outros domínios
- `clean-code`
- `game-development`
- `seo-fundamentals`
- `i18n-localization`
- `mcp-builder`
- `performance-profiling`
- `systematic-debugging`

---

## Workflows disponíveis

Os workflows funcionam como rotas operacionais para o agent.

| Comando | Objetivo |
|---|---|
| `/brainstorm` | Explorar ideias e descobrir caminhos |
| `/create` | Criar uma aplicação ou estrutura nova |
| `/debug` | Investigar e resolver problemas |
| `/deploy` | Organizar publicação e entrega |
| `/enhance` | Melhorar algo já existente |
| `/orchestrate` | Coordenar múltiplos agentes |
| `/plan` | Planejar a execução |
| `/preview` | Revisar e antecipar mudanças |
| `/status` | Entender situação atual |
| `/test` | Executar validação e testes |
| `/ui-ux-pro-max` | Acionar raciocínio visual premium |

---

## Templates de projeto

O conjunto `app-builder` inclui templates prontos para acelerar scaffolding e padronização.

| Template | Finalidade |
|---|---|
| `nextjs-fullstack` | Aplicações fullstack com Next.js |
| `nextjs-saas` | SaaS com base em Next.js |
| `nextjs-static` | Sites estáticos em Next.js |
| `express-api` | APIs em Express |
| `python-fastapi` | APIs e serviços em FastAPI |
| `react-native-app` | Aplicativos React Native |
| `flutter-app` | Aplicativos Flutter |
| `nuxt-app` | Aplicações Nuxt |
| `astro-static` | Sites estáticos com Astro |
| `electron-desktop` | Aplicativos desktop |
| `chrome-extension` | Extensões para navegador |
| `cli-tool` | Ferramentas de linha de comando |
| `monorepo-turborepo` | Estruturas monorepo com Turborepo |

---

## Pacote especializado para n8n

A pasta `n8n-skills/` expande o projeto com um pacote dedicado ao ecossistema n8n.

### O que existe lá
- documentação de instalação e uso;
- skills específicas para expression syntax, code nodes, validação, MCP tools e patterns;
- cenários de avaliação;
- builds distribuíveis.

### Skills n8n disponíveis
- `n8n-expression-syntax`
- `n8n-mcp-tools-expert`
- `n8n-workflow-patterns`
- `n8n-validation-expert`
- `n8n-node-configuration`
- `n8n-code-javascript`
- `n8n-code-python`

---

## Roteamento rápido por assunto

Esta é a visão rápida. Para o mapa completo, consulte [`docs/mapa-de-roteamento.md`](docs/mapa-de-roteamento.md).

| Assunto | Agente principal | Primeiro arquivo a ler |
|---|---|---|
| Frontend / UI | `frontend-specialist` | `.agent/skills/frontend-design/SKILL.md` |
| Backend / API | `backend-specialist` | `.agent/skills/api-patterns/SKILL.md` |
| Banco de dados | `database-architect` | `.agent/skills/database-design/SKILL.md` |
| Mobile | `mobile-developer` | `.agent/skills/mobile-design/SKILL.md` |
| Arquitetura | `orchestrator` | `.agent/skills/architecture/SKILL.md` |
| Testes | `test-engineer` | `.agent/skills/testing-patterns/SKILL.md` |
| Segurança | `security-auditor` | `.agent/skills/vulnerability-scanner/SKILL.md` |
| Performance | `performance-optimizer` | `.agent/skills/performance-profiling/SKILL.md` |
| DevOps / Deploy | `devops-engineer` | `.agent/skills/deployment-procedures/SKILL.md` |
| Debugging | `debugger` | `.agent/skills/systematic-debugging/SKILL.md` |
| Documentação | `documentation-writer` | `.agent/skills/documentation-templates/SKILL.md` |
| Planejamento | `project-planner` | `.agent/skills/plan-writing/SKILL.md` |
| n8n | `n8n-skills` | `n8n-skills/skills/.../SKILL.md` |
| Jogo | `game-developer` | `.agent/skills/game-development/SKILL.md` |
| UI/UX premium | `frontend-specialist` | `.agent/.shared/ui-ux-pro-max/data/` |
| Novo app | `orchestrator` | `.agent/skills/app-builder/SKILL.md` |

---

## Fluxo recomendado de uso

### 1. Clone o repositório

```bash
git clone https://github.com/LucasLgomes/dev-skills.git
cd dev-skills
```

### 2. Direcione o agent para o documento mestre

Peça explicitamente para o agent começar por este arquivo:

```text
Leia o arquivo agente_mestre_regras_aprendizado.md e siga todas as regras do projeto.
```

### 3. Faça uma solicitação orientada por contexto

Exemplo:

```text
Preciso criar uma API REST com autenticação JWT.
Consulte os arquivos corretos e siga as regras do projeto.
```

### 4. O comportamento esperado do agent será

1. classificar o domínio da tarefa;
2. consultar as regras globais;
3. ler o agente especialista correto;
4. abrir a skill adequada;
5. executar respeitando a hierarquia de decisão do repositório.

---

## Exemplo prático de raciocínio

### Solicitação
```text
Preciso melhorar a performance de uma tela Next.js com carregamento lento.
```

### Caminho esperado
1. identificar domínio: frontend + performance;
2. ler `.agent/agents/frontend-specialist.md`;
3. ler `.agent/agents/performance-optimizer.md`;
4. abrir `.agent/skills/nextjs-react-expert/SKILL.md`;
5. consultar módulos de waterfalls, bundle, server-side performance e re-render;
6. executar com base nas regras globais de `.agent/rules/GEMINI.md`.

---

## Protocolo de carregamento de skills

```text
Solicitação do usuário
       │
       ▼
Identificar domínio
       │
       ▼
Selecionar agente especialista
       │
       ▼
Ler frontmatter e skills relacionadas
       │
       ▼
Abrir SKILL.md da skill principal
       │
       ▼
Ler somente os módulos relevantes
       │
       ▼
Aplicar regras globais
       │
       ▼
Executar
```

### Prioridade de decisão
1. **P0** → `.agent/rules/GEMINI.md`
2. **P1** → `.agent/agents/*.md`
3. **P2** → `.agent/skills/**/SKILL.md`
4. **P3** → arquivos auxiliares da skill
5. **P4** → opinião ou extrapolação do modelo

---

## Scripts de validação

O projeto já inclui scripts para checagem automatizada.

| Script | Função | Uso recomendado |
|---|---|---|
| `.agent/scripts/checklist.py` | Validação por prioridade | Durante desenvolvimento |
| `.agent/scripts/verify_all.py` | Verificação mais completa | Antes de entrega ou deploy |

### Exemplos

```bash
python .agent/scripts/checklist.py .
```

```bash
python .agent/scripts/verify_all.py . --url http://localhost:3000
```

---

## Documentos principais do projeto

| Arquivo | Finalidade |
|---|---|
| `README.md` | Porta de entrada do projeto |
| `agente_mestre_regras_aprendizado.md` | Documento mestre para orientar o agent |
| `docs/regras-totais.md` | Consolidação das regras operacionais |
| `docs/guia-de-aprendizado-do-agent.md` | Explica como o agent aprende com o repositório |
| `docs/mapa-de-roteamento.md` | Índice operacional por assunto |
| `.agent/ARCHITECTURE.md` | Mapa técnico do sistema |
| `.agent/rules/GEMINI.md` | Regras globais de comportamento |

---

## Regras fundamentais

- **Idioma padrão:** português do Brasil
- **Fuso horário padrão:** `America/Sao_Paulo`
- **Nomenclatura:** nomes claros, completos e sem abreviações confusas
- **Fonte da verdade:** os arquivos do repositório sempre vencem suposições
- **Releitura obrigatória:** o agent deve reler os arquivos corretos antes de agir
- **Sem improviso:** se existe fonte especializada, ela deve ser priorizada
- **Clareza acima de enfeite:** documentação deve ser útil antes de ser bonita
- **Especialização por contexto:** o agent precisa mudar de trilha conforme o domínio da tarefa

---

## Como contribuir

### Adicionar um novo agent
1. criar o arquivo em `.agent/agents/`;
2. definir `name`, `description` e `skills`;
3. atualizar a arquitetura, se necessário;
4. garantir coerência com as regras globais.

### Adicionar uma nova skill
1. criar a pasta em `.agent/skills/`;
2. criar o `SKILL.md` como índice principal;
3. adicionar módulos auxiliares relevantes;
4. atualizar referências e roteamento quando necessário.

### Adicionar um novo workflow
1. criar o arquivo em `.agent/workflows/`;
2. definir objetivo e descrição;
3. alinhar com a lógica operacional do restante do sistema.

---

## Git e versionamento

### Fluxo básico

```bash
git clone https://github.com/LucasLgomes/dev-skills.git
git status
git add .
git commit -m "refina documentação e melhora experiência de entrada do projeto"
git push origin main
```

### Boas práticas
- escreva commits claros e objetivos;
- mantenha README e docs sincronizados;
- evite criar documentação decorativa;
- prefira mudanças que melhorem uso real do repositório.

---

## Caminho ideal para um novo usuário

Se alguém acabou de chegar no projeto, a ordem ideal é:

1. ler este `README.md`;
2. abrir `agente_mestre_regras_aprendizado.md`;
3. consultar `docs/mapa-de-roteamento.md`;
4. abrir `.agent/rules/GEMINI.md`;
5. seguir para o agent e skill do domínio desejado.

---

## Direção do projeto

O objetivo do **dev-skills** não é apenas armazenar arquivos.

Ele existe para criar uma base viva de especialização, onde agents consigam:

- entender melhor o contexto;
- consultar a fonte certa;
- reduzir improviso;
- manter consistência entre tarefas;
- evoluir com mais segurança, qualidade e profundidade.

---

<div align="center">

### Base de conhecimento operacional para agents que precisam trabalhar com contexto real

<sub>20 agentes especialistas · 36+ skills modulares · 11 workflows · 13 templates · 7 skills n8n</sub>

</div>
