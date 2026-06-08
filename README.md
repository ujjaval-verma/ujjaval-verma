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

### ▸ [agentic-cab-rides](https://github.com/ujjaval-verma/agentic-cab-rides) — *A prototype AI agent that books rides end-to-end*

<div align="center">
  <img src="https://raw.githubusercontent.com/ujjaval-verma/agentic-cab-rides/main/docs/assets/demo.gif" alt="Booking a ride end-to-end with the agent" width="760"/>
</div>

Native Anthropic SDK tool use (no LangChain) over a swappable marketplace
adapter — swapping Uber for Lyft is a new adapter; swapping for a non-ride
marketplace is a new intent variant.

**Stack:** `Python` · `FastAPI` · `Pydantic v2` · `Anthropic SDK`

Demonstrates security as a first-class concern — structural confirmation gates
that can't self-approve and fingerprint-verified drafts — and correct
distributed semantics via a replayable four-phase action log
(requested → verified → executed → outcome).

## Find me

[LinkedIn](https://linkedin.com/in/ujjavalverma) · [Toptal Profile](https://www.toptal.com/resume/ujjaval-verma)
