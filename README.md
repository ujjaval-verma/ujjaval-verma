# Ujjaval Verma

Full-stack engineer at [Toptal](https://www.toptal.com/resume/ujjaval-verma), based in Toronto.
I build production systems across the stack — distributed Go services, Rails and Node web apps,
Electron desktop apps with macOS native integration, Kubernetes-native platforms, and AI/LLM pipelines.
Most of that work has been in payments and platform infrastructure at scale.

I own the delivery side too: CI/CD and GitOps (ArgoCD, Helm, Kustomize, Terraform/OpenTofu),
multi-region active-active deployments, and the observability (Prometheus, Grafana, Datadog) that keeps
them honest — shipped end-to-end through to launch.

I lead the engineers who build alongside me without ever stepping away from the code. Rigour and human
investment aren't a trade-off: I roll up my sleeves, lead by example, and grow the people I mentor and
manage. As a fractional CTO, technical lead, or founding engineer, I close the gap between ambitious product
vision and production-grade execution, and I measure my impact in systems that outlast the sprint.

## Selected impact

- **AI National** — Built an agentic quote-comparison engine; cut LLM token usage **50–60%** and manual processing effort **75%**.
- **Teachable** — Led Stripe integration saving **~$2.5M/yr** in Forex fees; a rules-driven fraud-API cache cut external calls **85%** (~$500K/yr).
- **BenefitBay** — Automated payroll and employee-data syncs, saving **50,000+ hours/yr** across four large accounts.
- **PhonePe** — Spearheaded the direct NPCI **BBPS** integration, now clearing **2M+ transactions (₹1B+) daily** and adding **₹500M+/yr** in profitability.
- **Expedia** — Built next-gen payment services processing **97% of Expedia's transactions**, cutting annual hardware cost **25%**.

## Stack

**Languages:** Go · Ruby · Python · TypeScript · Java  
**Backend:** Ruby on Rails · Spring Boot · Express.js · Fastify  
**Frontend:** React · Next.js · Tailwind CSS  
**AI / LLMs:** Claude · MCP · RAG  
**Platform & DevOps:** Kubernetes · ArgoCD · Helm · Terraform · Docker · AWS · GCP · GitHub Actions  
**Observability:** Prometheus · Grafana · Datadog · Sentry  
**Data:** PostgreSQL · MySQL · Redis · Elasticsearch · Kafka  
**Payments:** Stripe · Finch Connect · NPCI BBPS  

## Things I care about in code

- Correct distributed systems semantics — state machines that distinguish transient failures from terminal ones  
- Security as a design constraint from the start, not an audit afterthought — most of my work has handled payments and PII  
- Documentation as code — architecture docs committed alongside the system they describe  
- Systems built to be operated — GitOps, health checks, and rollback paths, not just a green test suite  
- Tests that survive refactors  

## Featured projects

Three recent open-source projects — documented, tested, and architected to survive change — where I put the above into practice.

### ▸ [agentic-cab-rides](https://github.com/ujjaval-verma/agentic-cab-rides) — *A booking agent whose tools can't self-approve*

<div align="center">
  <img src="https://raw.githubusercontent.com/ujjaval-verma/agentic-cab-rides/main/docs/assets/demo.gif" alt="An AI agent booking a ride end-to-end, pausing at a confirmation gate" width="760"/>
</div>

A prototype AI agent that books rides end-to-end. The interesting part: state-mutating tools
(`confirm_booking`, `cancel_booking`) can't approve themselves — every gated call routes through a
confirmation channel the agent doesn't control, and fingerprints reject any tampered draft before it
reaches the provider. Every attempt lands in an append-only, replayable action log
(`requested → verified → executed → outcome`), over a swappable provider port proven by a second, non-ride adapter.

**Stack:** `Python` · `FastAPI` · `Pydantic` · `Typer` · `uv` · `pytest`

### ▸ [slide-ai](https://github.com/ujjaval-verma/slide-ai) — *Deck-as-code for agents*

<div align="center">
  <img src="https://raw.githubusercontent.com/ujjaval-verma/slide-ai/main/docs/assets/editor-live.gif" alt="Editing deck source on the left; the slide recompiles live on the right" width="760"/>
</div>

Agents author technical slide decks in a Markdown/YAML DSL over HTTP; the platform compiles them through
LaTeX Beamer (Tectonic) into validated PDFs and hands back machine-readable diagnostics, so the agent
self-corrects from compiler errors instead of guessing. A strictly one-direction pipeline
(source → compile → validate), with a design record and dated ADRs committed alongside the system.

**Stack:** `TypeScript` · `Fastify` · `React` · `LaTeX` · `pnpm`

### ▸ [skills](https://github.com/ujjaval-verma/skills) — *A composable harness of reusable, repo-agnostic AgentSkills*

<div align="center">
  <img src="https://raw.githubusercontent.com/ujjaval-verma/skills/main/docs/assets/social-card.jpg" alt="Skills harness: ship one slice, ship it right" width="760"/>
</div>

Markdown playbooks an LLM coding agent loads on demand — each is a `SKILL.md` encoding one workflow (when to
invoke it, what discipline to apply, what artifact to produce), with some bundling helper scripts or reference
docs the agent pulls in only when needed. They layer rather than overlap, so the agent picks the highest layer
that fits and delegates downward — discipline that persists across context resets, where the agent's own
working memory does not.

**Stack:** `Markdown` · `AgentSkills` · `SKILL.md`

## Trusted by clients

Rated 10/10 by past Toptal clients, including Clamshell.ai, BenefitBay, and Teachable — independently
verifiable through Toptal. The feedback repeats the same themes across employers: ownership, attention to
detail, speed of execution, and clear communication.

## Find me

[LinkedIn](https://linkedin.com/in/ujjavalverma) · [Toptal Profile](https://www.toptal.com/resume/ujjaval-verma)
