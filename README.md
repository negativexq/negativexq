<h1 align="center">Hi, I'm Ömer Faruk Koç 👋</h1>

<h3 align="center">
MLOps & AI Platform Engineer
</h3>

<p align="center">
I build and operate production ML platforms, RAG systems, data pipelines and reliability-focused AI infrastructure.
</p>

<p align="center">
  <a href="https://omerfkoc.dev">Portfolio</a>
  ·
  <a href="https://linkedin.com/in/omerfkoc">LinkedIn</a>
  ·
  <a href="mailto:omerfkoc98@gmail.com">Email</a>
  ·
  <a href="https://github.com/negativexq?tab=repositories">Repositories</a>
</p>

---

## About Me

I am an **MLOps & AI Platform Engineer** with more than three years of experience building and operating production AI, machine learning and data systems in the banking industry.

My professional work spans the ML lifecycle from data and feature pipelines through deployment, orchestration, monitoring, data quality and production operations. My public repositories independently explore the engineering problems around reliable AI platforms, retrieval systems, agent infrastructure and distributed applications.

- Deployed and operated **10+ production ML models**
- Contributed to **5 production LLM applications**
- Built data pipelines processing approximately **9 million records per day**
- Worked across **MLflow, Airflow, dbt, Docker, Kubernetes, CI/CD and data quality systems**
- Focused on **MLOps, AI Platform Engineering, RAG reliability, agent infrastructure and distributed systems**

> For architecture diagrams, engineering evidence, project relationships and detailed case studies, visit **[omerfkoc.dev](https://omerfkoc.dev)**.

---

## Featured Projects

### 1. [ModelOps Control Plane](https://github.com/negativexq/modelops-control-plane)

An ML release control plane for controlled model deployments with weighted canary routing, policy-driven evaluation, automated promotion and rollback, and an auditable deployment state machine.

Key engineering areas:

- Weighted canary routing
- Deployment state machine
- Policy engine
- Automated promotion and rollback
- SQLAlchemy optimistic concurrency control
- Real-stack CI verification
- Injected failure scenarios
- Backend validation with strict typing and integration testing

`Python` · `FastAPI` · `SQLAlchemy` · `Next.js` · `TypeScript` · `Locust` · `Docker Compose`

---

### 2. [Knowledge Base RAG](https://github.com/negativexq/knowledge-base-rag)

A reliability-oriented RAG platform with multi-source ingestion, incremental synchronization, hybrid retrieval, reranking, citation integrity and observable index repair.

Key engineering areas:

- PDF, Markdown and Notion ingestion
- Incremental synchronization
- Dense + sparse hybrid retrieval
- Native RRF fusion
- Cross-encoder reranking
- Citation-aware generation
- Citation integrity validation
- Versioned re-indexing
- Cancellation safety
- Qdrant / registry reconciliation
- Schema migration
- OpenTelemetry tracing and Jaeger inspection
- RAG evaluation and reranker experiments

The project also includes a bilingual reranker investigation across mono-lingual and cross-lingual retrieval configurations.

`Python` · `FastAPI` · `Qdrant` · `Ollama` · `OpenTelemetry` · `Jaeger` · `DeepEval` · `Docker Compose`

<sub>Knowledge Base RAG evolved from an earlier focused single-PDF [Production RAG Platform](https://github.com/negativexq/production-rag-platform) experiment.</sub>

---

### 3. [Repo Context Forge](https://github.com/negativexq/repo-context-forge)

A local-first MCP repository intelligence and agent platform for deterministic, source-grounded code analysis within strict read-only boundaries.

Key engineering areas:

- Six local MCP servers
- 40 configured tools
- Deterministic repository analysis
- Symbol, reference and dependency analysis
- Source-grounded context packs
- Task-specific evidence generation
- Bounded local Ollama agent
- Validated tool arguments
- Filesystem and path containment
- Restricted read-only Git subprocess boundary
- Read-only process security model

`Python` · `MCP` · `FastMCP` · `Python AST` · `Ollama` · `Git` · `Docker` · `Typer`

---

### 4. [Real-Time Commerce Platform](https://github.com/negativexq/real-time-commerce-platform)

A Kafka-based distributed commerce system focused on at-least-once correctness, transactional persistence, bounded failure handling, observability and measured performance limits.

Key engineering areas:

- At-least-once delivery
- Idempotent consumers
- Transactional outbox
- Bounded retries
- Dead-letter queue
- Partition-scoped ordering
- PostgreSQL transactional persistence
- Redis coordination
- Prometheus / Grafana observability
- Query-plan-driven optimization
- Performance boundary testing

The documented **~742 evt/s** service rate is an **isolated local benchmark**, not a production-capacity claim.

`Kafka` · `PostgreSQL` · `Redis` · `FastAPI` · `Prometheus` · `Grafana` · `Docker Compose`

---

### 5. [dbt Feature Lineage](https://github.com/negativexq/dbt-feature-lineage)

A local-first dbt analysis tool for model dependencies, cross-model column lineage, downstream impact and SQL transformation flow without requiring a live warehouse connection.

Key engineering areas:

- `target/manifest.json` analysis
- Compiled SQL analysis when available
- Static SQL / YAML fallback
- Cross-model column lineage
- Upstream and downstream tracing
- Direct vs transitive impact analysis
- Model DAG construction
- Query-flow visualization

`Python` · `dbt Core` · `sqlglot` · `NetworkX` · `Streamlit` · `Typer` · `Docker`

---

## Current Engineering Directions

I keep demonstrated capabilities separate from topics that I am actively exploring or planning. These areas extend the engineering problems already present in my current projects.

### Agent Orchestration — Learning

Exploring stateful agent workflows with explicit control flow instead of hiding orchestration inside prompts.

Focus areas:

- LangGraph
- Stateful workflows
- Branching
- Retries
- Failure recovery
- Human-in-the-loop
- Checkpointing
- Workflow observability

**Evidence target:** build and validate a production-style agent workflow with explicit state transitions, tracing and reproducible failure scenarios.

---

### Agentic Memory — Learning

Investigating how short-term workflow state and persistent memory can be separated, retrieved and compacted while keeping agent behavior inspectable and bounded.

Focus areas:

- Short-term state
- Long-term memory
- Episodic memory
- Semantic memory
- Retrieval
- Retention policies
- Memory compaction
- Memory lifecycle

**Evidence target:** add persistent memory to an agent workflow and evaluate retrieval relevance, retention behavior, compaction and failure cases.

---

### Context Engineering for RAG — Learning

Extending existing retrieval and reranking work into systematic context construction.

Retrieval answers:

> Which evidence do we find?

Context engineering answers:

> Which retrieved evidence should enter the model context, in what order, and within what budget?

Focus areas:

- Context construction
- Chunk selection
- Context ordering
- Context budgeting
- Redundancy reduction
- Diversity-aware selection
- Coverage-aware selection
- MMR
- Metadata-aware context
- Context compression
- Source-grounded context
- Context-window management

**Evidence target:** compare naive top-k retrieval with diversity-aware and coverage-aware context construction using answer quality, source coverage, context size and latency.

---

### GraphRAG — Learning

Exploring when explicit entities and relationships improve retrieval compared with vector-only approaches, especially for multi-hop and relationship-heavy questions.

Focus areas:

- Neo4j
- Knowledge graphs
- Entity extraction
- Relationship modeling
- Graph traversal
- Multi-hop retrieval
- Vector + graph retrieval
- Metadata filtering

**Evidence target:** build a Neo4j-backed GraphRAG experiment and compare it against conventional hybrid RAG on the same evaluation set.

---

### LLM / RAG Evaluation — Extending Existing Work

The current portfolio already includes retrieval evaluation, bilingual reranker experiments, citation integrity checks and observable RAG workflows. The next step is turning these into repeatable benchmark suites.

Focus areas:

- Recall@K
- MRR
- nDCG
- Reranker evaluation
- Citation integrity
- Grounding / faithfulness
- Context efficiency
- Latency
- Regression testing
- Versioned evaluation datasets

**Evidence target:** create a versioned evaluation dataset and automated benchmark comparing retrieval and context-construction configurations across quality, grounding, context size and latency metrics.

---

### Terraform — Planned

Planning to move existing local platform projects toward reproducible infrastructure provisioning.

Focus areas:

- Infrastructure as Code
- Reusable modules
- Remote state
- Environment separation
- CI validation
- Cloud deployment

**Evidence target:** provision an existing portfolio platform with reusable Terraform modules, remote state and separate environments.

---

### AI Platform on Kubernetes — Planned

Extending existing containerized AI systems toward production orchestration rather than treating Kubernetes as an isolated technology exercise.

Focus areas:

- Model serving
- Application workloads
- Health checks
- Autoscaling
- Rollout strategies
- Resource requests and limits
- GPU scheduling
- Service networking
- Configuration and secrets
- Workload isolation
- Observability

**Evidence target:** deploy an existing ModelOps or RAG workload on Kubernetes with health checks, resource controls, rollout strategy and observable service behavior.

---

### AI Platform Observability — Learning

Extending existing observability work toward AI-platform-specific signals across model serving, retrieval, agent execution and release automation.

Focus areas:

- Distributed tracing
- Model-serving metrics
- Retrieval latency
- Token usage
- Agent traces
- Tool-call traces
- Rollout metrics
- Failure classification
- SLIs / SLOs
- Evaluation telemetry

**Evidence target:** define and validate an observable AI service workflow with end-to-end traces, platform metrics, failure classification and explicit SLIs.

---

## Engineering Stack

### AI / ML Platform

`Python` · `FastAPI` · `MLflow` · `Docker` · `Kubernetes` · `GitHub Actions` · `scikit-learn`

### Retrieval / GenAI

`Qdrant` · `Ollama` · `RAG` · `OpenTelemetry` · `Jaeger` · `DeepEval`

### Data & Streaming

`Kafka` · `PostgreSQL` · `Oracle` · `Trino` · `dbt` · `Airflow` · `SQL Server`

### Engineering

`Git` · `Linux` · `Bash` · `CI/CD` · `REST APIs`

> Technologies listed above reflect current professional or public-project evidence. Planned and learning technologies remain in the roadmap section until they have demonstrated evidence.

---

## GitHub Statistics

<p align="center">
  <img
    src="https://github-readme-stats.vercel.app/api?username=negativexq&show_icons=true&theme=default&hide_border=true"
    alt="Ömer Faruk Koç GitHub statistics"
    height="165"
  />
  <img
    src="https://github-readme-stats.vercel.app/api/top-langs/?username=negativexq&layout=compact&theme=default&hide_border=true"
    alt="Most used languages"
    height="165"
  />
</p>

---

<p align="center">
  <a href="https://omerfkoc.dev"><strong>omerfkoc.dev</strong></a>
</p>
