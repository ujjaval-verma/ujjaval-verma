# Ujjaval Verma

Full-stack engineer at [Toptal](https://www.toptal.com/resume/ujjaval-verma), based in Toronto.
I build production systems across the stack — distributed Go services, Electron desktop apps
with macOS native integration, Rails web apps, and AI/LLM pipelines.
Lately I've been building open-source AI projects with the same engineering discipline — documented, tested, and architected to survive change.

## Stack

**Languages:** Go · Ruby · Python · Java · TypeScript · JavaScript · C#  
**Backend:** Ruby on Rails · Spring Boot · Dropwizard · Express.js · Flask  
**Frontend:** React · Next.js · Tailwind CSS · Stimulus · Hotwire · Backbone.js  
**AI / LLMs:** Claude · OpenAI · Agentic AI · MCP · RAG · Context Engineering  
**Cloud & Infra:** AWS · GCP · Azure · Docker · Kubernetes · Terraform · Apache Kafka · Firebase  
**Databases:** PostgreSQL · MySQL · Redis · MongoDB · DynamoDB · Elasticsearch · HBase  
**Payments:** Stripe API · Finch Connect · NPCI BBPS  
**Testing:** RSpec · Go table-driven tests · JUnit · Mockito  

## Things I care about in code

- Correct distributed systems semantics — state machines that distinguish transient failures from terminal ones  
- Security as a first-class concern, not a checkbox  
- Documentation as code — architecture docs committed alongside the system they describe  
- Tests that survive refactors  

## Featured projects

Two recent open-source projects where I put the above into practice.

### ▸ [slide-ai](https://github.com/ujjaval-verma/slide-ai) — *Deck-as-code for agents*

<div align="center">
  <img src="https://raw.githubusercontent.com/ujjaval-verma/slide-ai/main/docs/assets/editor-live.gif" alt="Editing deck source on the left; the slide recompiles live on the right" width="760"/>
</div>

Agents author technical slides in a Markdown/YAML DSL over HTTP; the platform
compiles them through LaTeX Beamer (Tectonic) into validated PDFs with
machine-readable diagnostics, so agents self-correct.

**Stack:** `TypeScript` · `Fastify` · `React` · `LaTeX`

Demonstrates docs-as-code (a design record and dated ADRs committed alongside
the system), a strictly one-direction pipeline (source → compile → validate, no
back-edges), and diagnostics that tell a fixable layout error apart from a hard
failure.

### ▸ [skills](https://github.com/ujjaval-verma/skills) — *A composable harness of reusable, repo-agnostic AgentSkills*

<div align="center">
  <img src="https://raw.githubusercontent.com/ujjaval-verma/skills/main/docs/assets/social-card.jpg" alt="Skills harness: ship one slice, ship it right" width="760"/>
</div>

Single-file Markdown playbooks an LLM coding agent loads on demand — each encodes
a workflow (when to invoke it, what discipline to apply, what artifact to
produce). They layer rather than overlap, so an agent picks the highest layer
that fits and delegates downward.

**Stack:** `Markdown` · `AgentSkills` · `SKILL.md`

Demonstrates discipline that survives context resets — the playbooks persist
where an agent's working memory does not — organised across engineering,
product, and productivity categories with composition rules that keep skills
from colliding.

## Find me

[LinkedIn](https://linkedin.com/in/ujjavalverma) · [Toptal Profile](https://www.toptal.com/resume/ujjaval-verma)
