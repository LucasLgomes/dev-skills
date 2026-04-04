# Regras Totais do Projeto

Este documento consolida todas as regras operacionais do projeto **dev-skills**. Ele serve como referencia centralizada para o comportamento do agente, padroes de codigo, documentacao e execucao.

---

## 1. Idioma e Localizacao

| Regra | Valor |
|-------|-------|
| Idioma de resposta | Portugues do Brasil |
| Idioma de codigo (variaveis, funcoes, classes, comentarios) | Portugues do Brasil |
| Fuso horario padrao | `America/Sao_Paulo` |
| Formato de data/hora em respostas humanas | Padrao brasileiro (dd/mm/aaaa, HH:mm) |

**Excecao:** Palavras-chave da linguagem de programacao (if, return, function, class) permanecem em ingles, pois fazem parte da sintaxe.

---

## 2. Nomenclatura

- Nomes de variaveis, funcoes, classes, arquivos, chaves JSON e identificadores devem estar em portugues brasileiro claro.
- Nao use abreviacoes confusas ou ambiguas.
- So use abreviacoes quando forem universalmente conhecidas (ex: `id`, `url`).
- Prefira nomes longos e claros a nomes curtos e genericos.
- Todo nome deve ser compreensivel por outro desenvolvedor sem esforco extra.

**Exemplos:**

```
// Correto
const listaDeUsuarios = [];
function calcularTotalDoPedido(pedido) {}

// Incorreto
const lstUsr = [];
function calcTP(p) {}
```

---

## 3. Hierarquia de Leitura e Decisao

Antes de qualquer tarefa, o agente deve ler os arquivos na seguinte ordem de prioridade:

| Prioridade | Fonte | Caminho |
|------------|-------|---------|
| P0 | Regras globais | `.agent/rules/GEMINI.md` |
| P1 | Arquitetura do sistema | `.agent/ARCHITECTURE.md` |
| P2 | Agente especialista | `.agent/agents/{agente}.md` |
| P3 | Skill principal | `.agent/skills/{skill}/SKILL.md` |
| P4 | Documentos auxiliares | Arquivos complementares da skill |
| P5 | Scripts e templates | Scripts validadores, exemplos |

**Regra de conflito:** Se houver conflito entre niveis, o nivel de maior prioridade vence.

---

## 4. Regra de Consulta aos Arquivos

O agente **deve** reler os arquivos corretos sempre que:

- Iniciar uma nova tarefa tecnica
- Mudar de assunto dentro da conversa
- A tarefa envolver outra especialidade
- Houver risco de conflito entre padroes
- Precisar gerar codigo, depurar, definir arquitetura, escolher stack, montar workflow, validar seguranca, performance ou testes
- Precisar produzir documentacao tecnica

O agente **nunca deve:**

- Responder apenas "de cabeca" quando existir arquivo especializado sobre o tema
- Usar uma unica fonte quando o assunto exigir cruzamento entre regras, arquitetura, workflow e skill
- Ignorar `SKILL.md`, `ARCHITECTURE.md`, `GEMINI.md` ou o especialista da area
- Tratar documentacao de apoio como opcional quando ela for claramente relevante

---

## 5. Regra de Nao Improvisar

Se existe arquivo especializado sobre o tema, ele tem prioridade absoluta sobre suposicoes.

**Ordem de confianca:**

1. Regra global (`GEMINI.md`)
2. Arquitetura (`ARCHITECTURE.md`)
3. Workflow (`.agent/workflows/*.md`)
4. Agente especialista (`.agent/agents/*.md`)
5. Skill principal (`SKILL.md`)
6. Documentos auxiliares
7. Scripts validadores
8. Exemplos e avaliacoes

---

## 6. Regra de Roteamento por Assunto

Cada tipo de tarefa tem um conjunto especifico de arquivos que devem ser consultados. O mapa completo esta em [`mapa-de-roteamento.md`](mapa-de-roteamento.md).

**Resumo operacional:**

- Frontend → `frontend-specialist.md` + `frontend-design/SKILL.md`
- Backend → `backend-specialist.md` + `api-patterns/SKILL.md`
- Banco de dados → `database-architect.md` + `database-design/SKILL.md`
- Mobile → `mobile-developer.md` + `mobile-design/SKILL.md`
- Testes → `test-engineer.md` + `testing-patterns/SKILL.md`
- Seguranca → `security-auditor.md` + `vulnerability-scanner/SKILL.md`
- Performance → `performance-optimizer.md` + `performance-profiling/SKILL.md`
- DevOps → `devops-engineer.md` + `deployment-procedures/SKILL.md`
- n8n → `n8n-skills/skills/.../SKILL.md`

---

## 7. Regra de Validacao Antes de Concluir

Antes de finalizar qualquer resposta ou implementacao, o agente deve verificar:

1. A resposta esta em portugues brasileiro?
2. Os nomes estao claros e sem abreviacoes confusas?
3. A resposta respeita as regras globais?
4. Os arquivos corretos foram consultados?
5. Nao houve improviso desnecessario?
6. A solucao esta consistente com a documentacao lida?

---

## 8. Regras de Qualidade de Codigo

Sempre priorizar:

- Simplicidade real
- Legibilidade
- Codigo pronto para producao
- Organizacao clara entre camadas
- Sem reinventar a roda
- Sem complexidade desnecessaria
- Acessibilidade e semantica quando houver HTML
- Seguranca por padrao
- Validacao de entrada
- Tratamento de erro adequado
- Consistencia com o padrao ja existente

**Arquitetura minima esperada:**

```
entrada → validacao → servico/regra → resposta estruturada
```

**Contrato JSON preferencial:**

```json
{
  "ok": true,
  "mensagem": "Texto descritivo",
  "dados": {}
}
```

**Comentarios em codigo:**

- Comentarios minimos
- Comente o **porque**, nao o obvio
- Evite comentarios excessivos

---

## 9. Regras de Documentacao

Ao criar qualquer documento:

- Seja especifico e conectado ao que existe no projeto
- Use titulos claros e ordem logica
- Deixe facil de escanear (scan-friendly)
- Evite repeticao inutil
- Nao esconda informacao critica
- Nao escreva conteudo generico so para preencher
- Escreva como documentacao real de produto

---

## 10. Regras de Git e Organizacao

- Mensagens de commit em portugues do Brasil
- Mensagens claras e descritivas
- Commits atomicos (uma mudanca logica por commit)
- Nao commitar arquivos sensiveis (`.env`, credenciais)
- Manter a estrutura de pastas coerente
- Nao criar arquivos desnecessarios
- Atualizar `ARCHITECTURE.md` quando adicionar agentes, skills ou workflows

---

## 11. Regra de Consistencia Visual e Textual

- Todo texto voltado ao usuario final deve ser em portugues do Brasil
- Manter padrao visual consistente entre documentos
- Nao misturar estilos de formatacao
- Tabelas devem ser legiveis
- Titulos devem ser claros e diretos
- Nao usar emojis em excesso

---

## 12. Decisoes Nao Especificadas

Quando existir decisao importante sem especificacao:

1. Nao inventar arbitrariamente
2. Avaliar opcoes disponiveis
3. Explicar trade-offs
4. Propor a melhor direcao com justificativa tecnica

---

## 13. Protocolo de Classificacao de Requisicoes

Toda requisicao deve ser classificada antes de qualquer acao:

| Tipo | Gatilho | Acao |
|------|---------|------|
| Pergunta | "o que e", "como funciona", "explique" | Resposta textual |
| Investigacao | "analise", "liste arquivos", "visao geral" | Analise sem criar arquivo |
| Codigo simples | "corrija", "adicione", "mude" (arquivo unico) | Edicao inline |
| Codigo complexo | "construa", "crie", "implemente", "refatore" | Plano obrigatorio |
| Design/UI | "design", "UI", "pagina", "dashboard" | Plano + agente especialista |
| Comando slash | /create, /orchestrate, /debug | Fluxo especifico do comando |

---

## 14. Porta Socratica

Para tarefas complexas, o agente deve parar e perguntar antes de executar:

- Funcionalidade nova → Minimo 3 perguntas estrategicas
- Correcao de bug → Confirmar entendimento + perguntas de impacto
- Requisicao vaga → Perguntar proposito, usuarios e escopo
- Orquestracao completa → Parar subagentes ate usuario confirmar plano

**Nunca assumir. Se 1% estiver incerto, perguntar.**
