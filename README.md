<h1 align="center">Hi, I'm Ömer Faruk Koç 👋</h1>

<h3 align="center">
MLOps & AI Platform Engineer
</h3>

<p align="center">
Building production ML platforms, reliable agentic systems, RAG infrastructure,
and distributed data applications.
</p>

<p align="center">
  <a href="https://omerfkoc.dev"><strong>Portfolio</strong></a>
  ·
  <a href="https://linkedin.com/in/omerfkoc">LinkedIn</a>
  ·
  <a href="mailto:omerfkoc98@gmail.com">Email</a>
  ·
  <a href="https://github.com/negativexq?tab=repositories">Repositories</a>
</p>

---

## About

I'm an **MLOps & AI Platform Engineer** with 3+ years of experience building and
operating production machine learning, data, and Generative AI systems in
financial services.

My professional work spans feature and data platforms, ML lifecycle automation,
containerized model serving, monitoring, and on-premises GPU/LLM infrastructure.

More recently, my public engineering work has focused on a harder question:

> **How do you make probabilistic AI systems reliable enough to interact with real software?**

That has led me toward deterministic execution controls, agent evaluation,
failure recovery, safe mutation semantics, retrieval infrastructure, and
observable AI platforms.

### Production experience

- **10+ production ML models** deployed and operated
- Customer-level data and feature pipelines covering approximately **9M customers**
- Reduced a core feature-engineering workflow from **120 → 30 minutes**
- Built an LLM-based call-center intelligence pipeline processing approximately **9,000 recordings daily**
- Worked across **Docker, Kubernetes, Airflow, dbt, MLRun, FastAPI, RAG, LLM serving, monitoring, and CI/CD**

> Detailed case studies, architecture diagrams, and engineering evidence:
> **[omerfkoc.dev](https://omerfkoc.dev)**

---

## Featured Engineering

### 1. [Agentic Customer Service Platform](https://github.com/negativexq/agentic-customer-service-platform)

**Building AI agents that can fail safely.**

A production-oriented agent platform built around one principle:

> **The LLM proposes; deterministic software decides what may execute.**

LLM outputs are treated as untrusted semantic proposals. Real-world mutations
remain behind server-owned grounding, target validation, business policy,
persisted confirmation, idempotency, and audit controls.

**Prospective live-model evidence**

29 unsafe semantic proposals  
→ 26 deterministic guard interventions  
→ 3 unsafe executable survivors  
→ 0 unsafe executions

- **540** measured executions across 180 bilingual scenarios × 3 repetitions
- **0 unsafe executions**
- **0 confirmation bypasses**
- **0 unauthorized mutations**
- **0 duplicate mutations**
- Unsafe executable survivors reduced **15 → 3 (-80%)** through deterministic hardening

The project also includes hybrid RAG, persistent memory, human-in-the-loop
workflows, resilience controls, OpenTelemetry tracing, PostgreSQL persistence,
and an operator console.

`Python` · `FastAPI` · `LangGraph` · `PostgreSQL` · `Qdrant` · `OpenTelemetry` · `React`

---

### 2. [Knowledge Base RAG](https://github.com/negativexq/knowledge-base-rag)

A reliability-oriented multi-source RAG platform covering ingestion,
synchronization, retrieval, reranking, citation integrity, evaluation, and
observable index lifecycle management.

Key engineering areas:

- Dense + sparse hybrid retrieval
- Reciprocal Rank Fusion
- Cross-encoder reranking
- Qdrant reconciliation
- Citation integrity
- Versioned re-indexing
- Partial-write and cancellation recovery
- OpenTelemetry / Jaeger
- DeepEval and bilingual retrieval experiments
- **448-test suite**

`Python` · `FastAPI` · `Qdrant` · `OpenTelemetry` · `Jaeger` · `DeepEval` · `Docker`

---

### 3. [ModelOps Control Plane](https://github.com/negativexq/modelops-control-plane)

An ML release control plane for deciding when a model version is safe to receive
production traffic.

Key engineering areas:

- Weighted canary routing
- Policy-driven evaluation
- Automated promotion and rollback
- Fault injection
- Optimistic concurrency control
- Auditable deployment timelines
- Worker-driven release automation
- **10% → 25% → 50% → 100%** progressive promotion

`Python` · `FastAPI` · `SQLAlchemy` · `Next.js` · `TypeScript` · `Docker Compose`

---

### 4. [Real-Time Commerce Platform](https://github.com/negativexq/real-time-commerce-platform)

A Kafka-based distributed system focused on correctness under at-least-once
delivery and measured performance limits.

Key engineering areas:

- At-least-once processing
- Idempotent consumers
- Transactional persistence
- Transactional outbox
- Bounded retries and DLQ
- Redis coordination
- PostgreSQL query optimization
- Prometheus / Grafana observability

A query-plan-driven optimization reduced a critical PostgreSQL lookup from
approximately **10.9 ms → 0.25 ms**. The isolated local
Kafka → processor → persistence path sustained approximately **742 events/s**.

`Kafka` · `PostgreSQL` · `Redis` · `FastAPI` · `Prometheus` · `Grafana` · `Docker Compose`

---

## More Work

### [Repo Context Forge](https://github.com/negativexq/repo-context-forge)

A local-first MCP repository intelligence and agent platform for deterministic,
source-grounded code analysis within strict read-only boundaries.

Key engineering areas:

- **40 configured tools across six MCP servers**
- Python AST symbol and call analysis
- Dependency and reference analysis
- Source-grounded context generation
- Validated tool arguments
- Bounded local agent execution
- Filesystem and path containment
- Restricted read-only Git subprocess access
- Deterministic repository intelligence workflows

`Python` · `MCP` · `FastMCP` · `Python AST` · `Ollama` · `Git` · `Docker` · `Typer`

---

### [dbt Feature Lineage](https://github.com/negativexq/dbt-feature-lineage)

A local-first dbt analysis tool for understanding model dependencies,
cross-model column lineage, downstream impact, and SQL transformation flow
without requiring a live warehouse connection.

Key engineering areas:

- dbt manifest analysis
- Compiled SQL analysis
- Static SQL / YAML fallback
- Cross-model column lineage
- Upstream and downstream tracing
- Direct vs transitive impact analysis
- Model DAG construction
- Query-flow visualization

`Python` · `dbt Core` · `sqlglot` · `NetworkX` · `Streamlit` · `Typer` · `Docker`

---

## Engineering Focus

### Reliable Agentic Systems

I focus on keeping probabilistic model behavior behind explicit software
boundaries rather than allowing models to directly own execution authority.

Current areas include:

- Structured model outputs
- Deterministic grounding
- Target admissibility
- Business-policy enforcement
- Human-in-the-loop confirmation
- Idempotent mutation semantics
- Failure recovery
- Persistent agent state
- Agent evaluation
- Runtime observability

The goal is not to make LLMs incapable of making mistakes.

The goal is to make those mistakes **non-authoritative**.

---

### AI / ML Platform Engineering

My platform work focuses on the systems around models rather than only the
models themselves:

- Feature platforms
- Model lifecycle automation
- Model serving
- Canary deployments
- Promotion and rollback
- Evaluation gates
- Containerized workloads
- CI/CD
- Monitoring
- On-premises GPU infrastructure
- Reproducible deployment workflows

---

### Retrieval & RAG Reliability

I treat retrieval as an engineered subsystem rather than a single vector-search
call.

Areas I work on include:

- Hybrid dense + sparse retrieval
- Reciprocal Rank Fusion
- Reranking
- Citation integrity
- Retrieval evaluation
- Index synchronization
- Versioned re-indexing
- Failure recovery
- Qdrant lifecycle management
- Cross-lingual retrieval behavior
- Observability

---

### Distributed Systems

I also build systems where correctness depends on failure semantics and state
transitions rather than only application logic.

Areas include:

- Kafka
- At-least-once delivery
- Idempotency
- Transactional outbox
- Retry and DLQ strategies
- PostgreSQL transactions
- Redis coordination
- Concurrency control
- Performance profiling
- Query-plan-driven optimization

---

## Engineering Stack

### AI / Agentic Systems

`LangGraph` · `LangChain` · `RAG` · `Qdrant` · `Structured Outputs` · `Evaluation` · `MCP` · `Ollama` · `llama.cpp` · `Hugging Face`

### MLOps / AI Platform

`MLRun` · `Docker` · `Kubernetes` · `GitHub Actions` · `FastAPI` · `Model Serving` · `Feature Stores` · `Canary Deployment`

### Data / Distributed Systems

`Apache Airflow` · `dbt` · `Apache Kafka` · `PostgreSQL` · `Oracle` · `Trino` · `Redis` · `SQL`

### Observability / Reliability

`OpenTelemetry` · `Jaeger` · `Prometheus` · `Grafana` · `Great Expectations` · `Deepchecks`

### Infrastructure

`Azure` · `On-Premises GPU` · `Linux` · `Git` · `Docker Compose`

---

## How I Think About AI Engineering

The model is only one component of an AI system.

Production reliability also depends on:

- What inputs the model is allowed to trust
- What outputs the application is allowed to execute
- How business state is validated
- How retries interact with writes
- How confirmations are persisted
- How retrieval evidence is bounded
- How failures are classified
- How behavior is evaluated
- How runtime decisions are observed
- How deployment changes are promoted or rolled back

That is the engineering layer I am most interested in.

> **Nondeterministic model behavior inside deterministic software boundaries.**

---

## Portfolio

For full project case studies, architecture diagrams, engineering evidence,
benchmarks, and project relationships:

### [omerfkoc.dev](https://omerfkoc.dev)

You can also explore all repositories directly from my
[GitHub profile](https://github.com/negativexq?tab=repositories).

---

<p align="center">
  <strong>AI, data, and distributed systems — built with evidence.</strong>
</p>

<p align="center">
  <a href="https://omerfkoc.dev">Portfolio</a>
  ·
  <a href="https://linkedin.com/in/omerfkoc">LinkedIn</a>
  ·
  <a href="mailto:omerfkoc98@gmail.com">Email</a>
</p>
