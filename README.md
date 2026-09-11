# Platform reliability engineer working on payment and ingestion systems.
## @ChelseyWissman

I build durable APIs, queues, workers, and pipelines for payment and ingestion workloads.
I own failure modes around schemas, retries, caches, indexes, and operational recovery.
My priorities are bounded blast radius, clear ownership, and recoverable deployments.
I accept conservative integration costs when they make failure modes easier to reason about.
### 🛠 Tech & Infrastructure

- **Core:** TypeScript, Node.js, PostgreSQL, Prisma
- **Data:** Kafka, ClickHouse, Redis
- **Infra:** Docker, Terraform, Kubernetes
- **Tooling:** OpenTelemetry, Prometheus, GitHub Actions
### ⚙️ Engineering Areas


- Idempotent payment APIs, RPC contracts, and outbox-based event delivery.
- Kafka schema evolution, dead-letter routing, and replay-safe worker design.
- PostgreSQL indexing, cache invalidation, and ClickHouse ingestion pipelines.
- Kubernetes deployment gates, traces, metrics, and incident response.
### 🔭 Current Focus


- Reducing duplicate payments by enforcing idempotency across APIs, queues, and workers.
- Shrinking migration windows with PostgreSQL online changes and reversible rollbacks.
- Improving trace correlation across RPCs, workers, and Kafka event boundaries.
- Tightening rate limits where cache misses could overload payment providers.
### 📌 Engineering Notes

- Tests should cover boundary values, partial failures, and retry behavior together.
- API and schema boundaries need explicit contracts, not implicit assumptions.
- Migrations should be small, observable, and safe to roll back.
- Errors need structured context; retries need deadlines, budgets, and backoff.
### 🧭 How I Work

- Keep the common path boring and isolate recovery behind explicit boundaries.
- Prefer bounded concurrency and idempotent operations over fragile coordination.
- Make operational state visible before increasing automation.

_I prefer systems that fail quietly, recover predictably, and leave enough evidence to investigate.*