# Mapa de Roteamento por Assunto

Este documento serve como indice operacional. Ele diz exatamente quais arquivos o agente deve consultar para cada tipo de tarefa.

**Como usar:** Identifique o assunto da tarefa, localize a secao correspondente e leia os arquivos listados na ordem indicada.

---

## 1. Orquestracao e Coordenacao Multi-agente

**Quando usar:** Tarefa envolve varias areas, precisa decompor problema grande, ha dependencia entre front, back, banco, testes e deploy.

**Arquivos principais:**
- `.agent/agents/orchestrator.md`
- `.agent/workflows/orchestrate.md`
- `.agent/ARCHITECTURE.md`

**Arquivos de apoio:**
- `.agent/skills/parallel-agents/SKILL.md`
- `.agent/skills/intelligent-routing/SKILL.md`
- `.agent/skills/architecture/SKILL.md`
- `.agent/skills/architecture/context-discovery.md`
- `.agent/skills/architecture/pattern-selection.md`
- `.agent/skills/architecture/patterns-reference.md`
- `.agent/skills/architecture/trade-off-analysis.md`

---

## 2. Planejamento e Descoberta

**Quando usar:** Planejar, criar roadmap, levantar requisitos, definir escopo, estruturar fases.

**Arquivos principais:**
- `.agent/agents/project-planner.md`
- `.agent/agents/product-manager.md`
- `.agent/agents/product-owner.md`
- `.agent/workflows/plan.md`
- `.agent/workflows/brainstorm.md`

**Arquivos de apoio:**
- `.agent/skills/plan-writing/SKILL.md`
- `.agent/skills/brainstorming/SKILL.md`
- `.agent/skills/brainstorming/dynamic-questioning.md`
- `.agent/skills/app-builder/project-detection.md`
- `.agent/skills/app-builder/agent-coordination.md`

---

## 3. Criacao de Aplicacao e Scaffolding

**Quando usar:** Criar projeto novo, escolher stack, montar esqueleto inicial.

**Arquivos principais:**
- `.agent/skills/app-builder/SKILL.md`
- `.agent/skills/app-builder/scaffolding.md`
- `.agent/skills/app-builder/tech-stack.md`
- `.agent/skills/app-builder/feature-building.md`

**Templates disponiveis:**
- `.agent/skills/app-builder/templates/nextjs-fullstack/TEMPLATE.md`
- `.agent/skills/app-builder/templates/nextjs-saas/TEMPLATE.md`
- `.agent/skills/app-builder/templates/nextjs-static/TEMPLATE.md`
- `.agent/skills/app-builder/templates/express-api/TEMPLATE.md`
- `.agent/skills/app-builder/templates/python-fastapi/TEMPLATE.md`
- `.agent/skills/app-builder/templates/react-native-app/TEMPLATE.md`
- `.agent/skills/app-builder/templates/flutter-app/TEMPLATE.md`
- `.agent/skills/app-builder/templates/nuxt-app/TEMPLATE.md`
- `.agent/skills/app-builder/templates/astro-static/TEMPLATE.md`
- `.agent/skills/app-builder/templates/electron-desktop/TEMPLATE.md`
- `.agent/skills/app-builder/templates/chrome-extension/TEMPLATE.md`
- `.agent/skills/app-builder/templates/cli-tool/TEMPLATE.md`
- `.agent/skills/app-builder/templates/monorepo-turborepo/TEMPLATE.md`

---

## 4. Frontend, UI/UX e Design Visual

**Quando usar:** Interface web, componentes, layout, UX, responsividade, acessibilidade, design system.

**Arquivos principais:**
- `.agent/agents/frontend-specialist.md`
- `.agent/skills/frontend-design/SKILL.md`

**Arquivos de apoio:**
- `.agent/skills/frontend-design/animation-guide.md`
- `.agent/skills/frontend-design/color-system.md`
- `.agent/skills/frontend-design/decision-trees.md`
- `.agent/skills/frontend-design/motion-graphics.md`
- `.agent/skills/frontend-design/typography-system.md`
- `.agent/skills/frontend-design/ux-psychology.md`
- `.agent/skills/frontend-design/visual-effects.md`
- `.agent/skills/web-design-guidelines/SKILL.md`
- `.agent/skills/tailwind-patterns/SKILL.md`
- `.agent/skills/clean-code/SKILL.md`

**Base visual premium:**
- `.agent/.shared/ui-ux-pro-max/data/colors.csv`
- `.agent/.shared/ui-ux-pro-max/data/styles.csv`
- `.agent/.shared/ui-ux-pro-max/data/typography.csv`
- `.agent/.shared/ui-ux-pro-max/data/icons.csv`
- `.agent/.shared/ui-ux-pro-max/data/landing.csv`
- `.agent/.shared/ui-ux-pro-max/data/products.csv`
- `.agent/.shared/ui-ux-pro-max/data/ui-reasoning.csv`
- `.agent/.shared/ui-ux-pro-max/data/ux-guidelines.csv`
- `.agent/.shared/ui-ux-pro-max/data/web-interface.csv`

**Stacks visuais especificas:**
- `.agent/.shared/ui-ux-pro-max/data/stacks/react.csv`
- `.agent/.shared/ui-ux-pro-max/data/stacks/nextjs.csv`
- `.agent/.shared/ui-ux-pro-max/data/stacks/vue.csv`
- `.agent/.shared/ui-ux-pro-max/data/stacks/svelte.csv`
- `.agent/.shared/ui-ux-pro-max/data/stacks/html-tailwind.csv`
- `.agent/.shared/ui-ux-pro-max/data/stacks/shadcn.csv`
- `.agent/.shared/ui-ux-pro-max/data/stacks/nuxtjs.csv`
- `.agent/.shared/ui-ux-pro-max/data/stacks/nuxt-ui.csv`
- `.agent/.shared/ui-ux-pro-max/data/stacks/flutter.csv`
- `.agent/.shared/ui-ux-pro-max/data/stacks/react-native.csv`
- `.agent/.shared/ui-ux-pro-max/data/stacks/swiftui.csv`
- `.agent/.shared/ui-ux-pro-max/data/stacks/jetpack-compose.csv`

**Workflows recomendados:**
- `.agent/workflows/ui-ux-pro-max.md`
- `.agent/workflows/create.md`
- `.agent/workflows/enhance.md`
- `.agent/workflows/preview.md`

---

## 5. Backend, APIs e Logica de Servidor

**Quando usar:** API, endpoints, autenticacao, rate limiting, contratos de resposta, REST, GraphQL, tRPC.

**Arquivos principais:**
- `.agent/agents/backend-specialist.md`
- `.agent/skills/api-patterns/SKILL.md`

**Arquivos de apoio:**
- `.agent/skills/api-patterns/api-style.md`
- `.agent/skills/api-patterns/auth.md`
- `.agent/skills/api-patterns/documentation.md`
- `.agent/skills/api-patterns/graphql.md`
- `.agent/skills/api-patterns/rate-limiting.md`
- `.agent/skills/api-patterns/response.md`
- `.agent/skills/api-patterns/rest.md`
- `.agent/skills/api-patterns/security-testing.md`
- `.agent/skills/api-patterns/trpc.md`
- `.agent/skills/api-patterns/versioning.md`

**Complementos por stack:**
- `.agent/skills/nodejs-best-practices/SKILL.md`
- `.agent/skills/python-patterns/SKILL.md`
- `.agent/skills/server-management/SKILL.md`

---

## 6. Banco de Dados

**Quando usar:** Modelagem, tabelas, relacionamentos, indices, queries, migracoes, performance de banco, ORM.

**Arquivos principais:**
- `.agent/agents/database-architect.md`
- `.agent/skills/database-design/SKILL.md`

**Arquivos de apoio:**
- `.agent/skills/database-design/database-selection.md`
- `.agent/skills/database-design/indexing.md`
- `.agent/skills/database-design/migrations.md`
- `.agent/skills/database-design/optimization.md`
- `.agent/skills/database-design/orm-selection.md`
- `.agent/skills/database-design/schema-design.md`

---

## 7. Mobile

**Quando usar:** App mobile, UX mobile, Android, iOS, performance mobile, design touch, navegacao mobile.

**Arquivos principais:**
- `.agent/agents/mobile-developer.md`
- `.agent/skills/mobile-design/SKILL.md`

**Arquivos de apoio:**
- `.agent/skills/mobile-design/decision-trees.md`
- `.agent/skills/mobile-design/mobile-backend.md`
- `.agent/skills/mobile-design/mobile-color-system.md`
- `.agent/skills/mobile-design/mobile-debugging.md`
- `.agent/skills/mobile-design/mobile-design-thinking.md`
- `.agent/skills/mobile-design/mobile-navigation.md`
- `.agent/skills/mobile-design/mobile-performance.md`
- `.agent/skills/mobile-design/mobile-testing.md`
- `.agent/skills/mobile-design/mobile-typography.md`
- `.agent/skills/mobile-design/platform-android.md`
- `.agent/skills/mobile-design/platform-ios.md`
- `.agent/skills/mobile-design/touch-psychology.md`

**Copias adicionais:**
- `agents/Mobile/mobile-developer.md`
- `agents/Mobile/mobile-design/SKILL.md` (e todos os arquivos de apoio espelhados)

---

## 8. React e Next.js Avancado

**Quando usar:** Performance avancada React, otimizacao de bundle, renderizacao, cache, waterfalls, re-render.

**Arquivos principais:**
- `.agent/skills/nextjs-react-expert/SKILL.md`

**Arquivos de apoio (9 modulos):**
- `.agent/skills/nextjs-react-expert/1-async-eliminating-waterfalls.md`
- `.agent/skills/nextjs-react-expert/2-bundle-bundle-size-optimization.md`
- `.agent/skills/nextjs-react-expert/3-server-server-side-performance.md`
- `.agent/skills/nextjs-react-expert/4-client-client-side-data-fetching.md`
- `.agent/skills/nextjs-react-expert/5-rerender-re-render-optimization.md`
- `.agent/skills/nextjs-react-expert/6-rendering-rendering-performance.md`
- `.agent/skills/nextjs-react-expert/7-js-javascript-performance.md`
- `.agent/skills/nextjs-react-expert/8-advanced-advanced-patterns.md`
- `.agent/skills/nextjs-react-expert/9-cache-components.md`

---

## 9. Depuracao e Investigacao

**Quando usar:** Bug, erro dificil, comportamento legado, rastrear origem de problema.

**Arquivos principais:**
- `.agent/agents/debugger.md`
- `.agent/agents/code-archaeologist.md`
- `.agent/workflows/debug.md`

**Arquivos de apoio:**
- `.agent/skills/systematic-debugging/SKILL.md`
- `.agent/skills/code-review-checklist/SKILL.md`
- `.agent/skills/testing-patterns/SKILL.md`
- `.agent/skills/webapp-testing/SKILL.md`
- `.agent/skills/lint-and-validate/SKILL.md`

---

## 10. Performance e Otimizacao

**Quando usar:** Lentidao, gargalo, uso excessivo de recursos, Lighthouse, otimizacao de rendering.

**Arquivos principais:**
- `.agent/agents/performance-optimizer.md`
- `.agent/skills/performance-profiling/SKILL.md`

**Arquivos de apoio:**
- `.agent/skills/nextjs-react-expert/SKILL.md`
- `.agent/.shared/ui-ux-pro-max/data/react-performance.csv`
- `.agent/skills/database-design/optimization.md`
- `.agent/skills/mobile-design/mobile-performance.md`

---

## 11. Testes e Qualidade

**Quando usar:** Estrategia de testes, automacao, validacao de comportamento, reduzir regressao.

**Arquivos principais:**
- `.agent/agents/test-engineer.md`
- `.agent/agents/qa-automation-engineer.md`
- `.agent/workflows/test.md`

**Arquivos de apoio:**
- `.agent/skills/testing-patterns/SKILL.md`
- `.agent/skills/tdd-workflow/SKILL.md`
- `.agent/skills/webapp-testing/SKILL.md`
- `.agent/skills/lint-and-validate/SKILL.md`
- `.agent/skills/code-review-checklist/SKILL.md`

---

## 12. Seguranca e Auditoria

**Quando usar:** Risco de seguranca, auditoria, revisao de vulnerabilidade, teste de seguranca, hardening.

**Arquivos principais:**
- `.agent/agents/security-auditor.md`
- `.agent/agents/penetration-tester.md`
- `.agent/skills/vulnerability-scanner/SKILL.md`

**Arquivos de apoio:**
- `.agent/skills/vulnerability-scanner/checklists.md`
- `.agent/skills/api-patterns/security-testing.md`
- `.agent/skills/red-team-tactics/SKILL.md`

---

## 13. DevOps, Deploy e Servidor

**Quando usar:** Deploy, ambiente, automacao operacional, Linux, Windows, servidor.

**Arquivos principais:**
- `.agent/agents/devops-engineer.md`
- `.agent/workflows/deploy.md`
- `.agent/skills/deployment-procedures/SKILL.md`
- `.agent/skills/server-management/SKILL.md`

**Arquivos de apoio:**
- `.agent/skills/bash-linux/SKILL.md`
- `.agent/skills/powershell-windows/SKILL.md`

---

## 14. Documentacao Tecnica

**Quando usar:** Escrever documentacao, README, guias, explicacoes tecnicas, onboarding.

**Arquivos principais:**
- `.agent/agents/documentation-writer.md`
- `.agent/skills/documentation-templates/SKILL.md`

**Arquivos de apoio:**
- `.agent/skills/api-patterns/documentation.md`
- `.agent/skills/app-builder/feature-building.md`

---

## 15. SEO

**Quando usar:** SEO, estruturacao para busca, conteudo indexavel.

**Arquivos principais:**
- `.agent/agents/seo-specialist.md`
- `.agent/skills/seo-fundamentals/SKILL.md`

**Arquivos de apoio:**
- `.agent/skills/web-design-guidelines/SKILL.md`

---

## 16. Jogos

**Quando usar:** Jogo, mecanica, arte, audio, multiplayer, VR/AR.

**Arquivos principais:**
- `.agent/agents/game-developer.md`
- `.agent/skills/game-development/SKILL.md`

**Subareas:**
- `.agent/skills/game-development/2d-games/SKILL.md`
- `.agent/skills/game-development/3d-games/SKILL.md`
- `.agent/skills/game-development/game-art/SKILL.md`
- `.agent/skills/game-development/game-audio/SKILL.md`
- `.agent/skills/game-development/game-design/SKILL.md`
- `.agent/skills/game-development/mobile-games/SKILL.md`
- `.agent/skills/game-development/multiplayer/SKILL.md`
- `.agent/skills/game-development/pc-games/SKILL.md`
- `.agent/skills/game-development/vr-ar/SKILL.md`
- `.agent/skills/game-development/web-games/SKILL.md`

---

## 17. Internacionalizacao

**Quando usar:** Localizacao, multiplos idiomas, adaptacao regional.

**Arquivos principais:**
- `.agent/skills/i18n-localization/SKILL.md`
- `.agent/skills/geo-fundamentals/SKILL.md`

---

## 18. n8n e Automacao

**Quando usar:** n8n, workflows automatizados, code nodes, expressoes, validacao, MCP tools.

**Prioridade de leitura:**

1. `n8n-skills/CLAUDE.md`
2. `n8n-skills/README.md`
3. `n8n-skills/docs/USAGE.md`
4. `n8n-skills/docs/INSTALLATION.md`
5. `n8n-skills/docs/DEVELOPMENT.md`
6. `n8n-skills/docs/CODE_NODE_BEST_PRACTICES.md`

**Skills por subarea:**

| Subarea | Arquivo principal | Apoio |
|---------|-------------------|-------|
| JavaScript | `n8n-skills/skills/n8n-code-javascript/SKILL.md` | BUILTIN_FUNCTIONS.md, COMMON_PATTERNS.md, DATA_ACCESS.md, ERROR_PATTERNS.md |
| Python | `n8n-skills/skills/n8n-code-python/SKILL.md` | COMMON_PATTERNS.md, DATA_ACCESS.md, ERROR_PATTERNS.md, STANDARD_LIBRARY.md |
| Expressoes | `n8n-skills/skills/n8n-expression-syntax/SKILL.md` | COMMON_MISTAKES.md, EXAMPLES.md |
| Ferramentas MCP | `n8n-skills/skills/n8n-mcp-tools-expert/SKILL.md` | SEARCH_GUIDE.md, VALIDATION_GUIDE.md, WORKFLOW_GUIDE.md |
| Configuracao | `n8n-skills/skills/n8n-node-configuration/SKILL.md` | DEPENDENCIES.md, OPERATION_PATTERNS.md |
| Validacao | `n8n-skills/skills/n8n-validation-expert/SKILL.md` | ERROR_CATALOG.md, FALSE_POSITIVES.md |
| Padroes | `n8n-skills/skills/n8n-workflow-patterns/SKILL.md` | webhook_processing.md, http_api_integration.md, database_operations.md, ai_agent_workflow.md, scheduled_tasks.md |

**Exemplos concretos:** `n8n-skills/evaluations/{subarea}/*.json`

---

## 19. Modos Comportamentais

**Quando usar:** Ajustar postura do agente, exploracao do repositorio, comportamento investigativo.

**Arquivos principais:**
- `.agent/skills/behavioral-modes/SKILL.md`
- `.agent/agents/explorer-agent.md`
