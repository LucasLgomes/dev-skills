# Guia de Aprendizado do Agente

Este documento ensina como o agente de IA deve aprender com o repositorio **dev-skills**. O objetivo e garantir que o agente opere com precisao, contexto e consistencia, consultando sempre as fontes corretas antes de agir.

---

## Principio Fundamental

> O agente nunca deve depender apenas de memoria. Ele deve reler os arquivos corretos sempre que mudar o dominio do problema, iniciar uma nova tarefa ou precisar de precisao tecnica.

O repositorio **dev-skills** nao e uma colecao de arquivos. E uma **base viva de conhecimento operacional** onde o agente aprende por releitura contextual.

---

## Fluxo de Aprendizado

### Etapa 1 — Regras-mae do projeto

Antes de qualquer tarefa, ler:

1. `.agent/rules/GEMINI.md` — Regras globais de comportamento
2. `.agent/ARCHITECTURE.md` — Mapa de agentes, skills e workflows
3. `agents/ARCHITECTURE.md` — Arquitetura operacional

**Objetivo:** Alinhar comportamento, entender a estrutura, conhecer as regras que nunca devem ser violadas.

### Etapa 2 — Workflow da tarefa

Identificar qual workflow se aplica e ler o arquivo correspondente:

| Tarefa | Workflow |
|--------|----------|
| Criar algo novo | `.agent/workflows/create.md` |
| Planejar | `.agent/workflows/plan.md` |
| Depurar | `.agent/workflows/debug.md` |
| Melhorar existente | `.agent/workflows/enhance.md` |
| Testar | `.agent/workflows/test.md` |
| Deploy | `.agent/workflows/deploy.md` |
| Orquestrar | `.agent/workflows/orchestrate.md` |
| Brainstorm | `.agent/workflows/brainstorm.md` |
| Pre-visualizar | `.agent/workflows/preview.md` |
| Verificar status | `.agent/workflows/status.md` |
| Design visual | `.agent/workflows/ui-ux-pro-max.md` |

### Etapa 3 — Agente especialista

Ler o agente mais aderente ao assunto. O agente esta em `.agent/agents/{nome}.md` e contem:

- Frontmatter com skills que deve carregar
- Regras especificas do dominio
- Protocolo de atuacao
- Limites de atuacao (o que pode e o que nao pode fazer)

### Etapa 4 — Skills especificas

Ler a `SKILL.md` da skill principal e os arquivos complementares relevantes. Nao ler todos os arquivos da pasta — apenas os que fazem sentido para a tarefa.

### Etapa 5 — Material de apoio

Se necessario, consultar:

- Templates (`.agent/skills/app-builder/templates/`)
- CSVs de referencia visual (`.agent/.shared/ui-ux-pro-max/data/`)
- Scripts validadores (`.agent/skills/{skill}/scripts/`)
- Avaliacoes e exemplos (`n8n-skills/evaluations/`)

### Etapa 6 — Cruzamento final

Antes de responder ou executar, confirmar:

- A regra global esta respeitada?
- A resposta esta em portugues do Brasil?
- Os nomes estao claros?
- A solucao esta consistente com a documentacao lida?
- Nao houve improviso desnecessario?

---

## Quando Reler Obrigatoriamente

O agente deve reler os arquivos corretos sempre que:

- Iniciar uma nova tarefa tecnica
- Mudar de assunto dentro da conversa
- A tarefa envolver outra especialidade
- Houver risco de conflito entre padroes
- Precisar gerar codigo
- Precisar depurar
- Precisar definir arquitetura
- Precisar escolher stack ou template
- Precisar montar workflow
- Precisar validar seguranca, performance ou testes
- Precisar produzir documentacao tecnica

---

## O Que Nunca Fazer

- Responder "de cabeca" quando existir arquivo especializado
- Usar uma unica fonte quando o assunto exigir cruzamento de informacoes
- Ignorar `SKILL.md`, `ARCHITECTURE.md`, `GEMINI.md` ou o agente especialista
- Tratar documentacao de apoio como opcional quando ela for relevante
- Improvisar quando existir referencia concreta no repositorio

---

## Algoritmo Operacional

O agente deve executar mentalmente este fluxo para toda tarefa:

```
1. CLASSIFICAR a tarefa
   → frontend? backend? mobile? banco? n8n? arquitetura?
   → planejamento? debug? performance? seguranca? testes?

2. MONTAR PACOTE DE LEITURA
   → Selecionar caminhos do mapa de roteamento

3. RELER A BASE
   → Ler novamente os arquivos mais relevantes

4. EXTRAIR PRINCIPIOS
   → Regras da area
   → Restricoes
   → Padroes recomendados
   → Anti-padroes
   → Scripts validadores uteis

5. PRODUZIR A SOLUCAO
   → Em portugues do Brasil
   → Com nomes claros
   → Com arquitetura limpa
   → Consistente com a documentacao

6. VALIDAR ANTES DE FINALIZAR
   → Checklist de qualidade
```

---

## Especializacao por Dominio

O agente se especializa por releitura, nao por memorizacao. A cada tarefa de um dominio diferente, ele deve:

1. Consultar o mapa de roteamento (`docs/mapa-de-roteamento.md`)
2. Ler os arquivos do novo dominio
3. Absorver as regras e padroes daquele contexto
4. Aplicar na tarefa atual

Isso garante que o agente mantenha qualidade independente de quantas conversas ou tarefas ja executou.

---

## Ordem de Confianca das Fontes

Quando houver duvida ou conflito entre informacoes:

| Posicao | Fonte |
|---------|-------|
| 1 (maior) | Regra global (`GEMINI.md`) |
| 2 | Arquitetura (`ARCHITECTURE.md`) |
| 3 | Workflow (`.agent/workflows/*.md`) |
| 4 | Agente especialista (`.agent/agents/*.md`) |
| 5 | Skill principal (`SKILL.md`) |
| 6 | Documentos auxiliares |
| 7 | Scripts validadores |
| 8 (menor) | Exemplos e avaliacoes |

---

## O Que Nao Usar Como Fonte Primaria

- Arquivos `.pyc`
- Conteudo de `.git/`
- Arquivos compactados em `dist/`
- Amostras automaticas internas que nao sejam documentacao ou skill oficial

---

## Instrucao Final

Sempre que receber uma tarefa, o agente deve pensar:

> "Qual e a natureza exata desta demanda? Quais arquivos deste repositorio eu preciso reler agora para agir com precisao? Qual especialista devo consultar? Qual skill complementa essa decisao? Estou respeitando as regras globais de idioma, nomenclatura, arquitetura e clareza?"

Se a resposta nao estiver totalmente fundamentada, voltar aos arquivos corretos, reler e so entao prosseguir.
