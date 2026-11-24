<h1 align="center">Peerawit Lakhampa</h1>

<p align="center">
  <strong>Full-Stack Web Developer</strong> · Bangkok, Thailand
</p>

<p align="center">
  <a href="https://peerawit-portfolio.netlify.app/">Portfolio</a> ·
  <a href="https://github.com/Mindenry">GitHub</a> ·
  <a href="mailto:peerawitm1xnd@gmail.com">Email</a> ·
  <a href="https://peerawit-portfolio.netlify.app/peerawit-lakhampa-resume.pdf">Resume</a>
</p>

I build full-stack web applications and the systems behind them: interfaces, APIs, data models, background jobs, and the tests and deployment setup that keep the important paths correct. I enjoy problems where software has to hold up outside a demo, whether that means two approvers deciding the same request at once, preventing stock from being oversold during checkout, or keeping an AI model from making a decision it should not make.

I'm currently open to software engineering opportunities.

## About

I'm a full-stack developer based in Bangkok, working mainly with TypeScript and Python. My recent projects are built as monorepos or modular monoliths, with explicit domain boundaries, versioned database migrations, and documented operational limits.

I care about the parts that are easy to skip: authorization enforced on the server, transactions that behave under concurrency, failure paths that are tested, and release notes that say what is not ready. I'm looking for a team where I can keep building systems with real constraints and learn from engineers who have shipped more of them than I have.

## Tech Stack

| Area | Technologies |
| :-- | :-- |
| **Languages** | TypeScript · Python · SQL · HTML/CSS |
| **Frontend** | React · Next.js · Vite · Tailwind CSS · TanStack Query · Radix UI |
| **Backend** | Node.js · NestJS · FastAPI · REST APIs · Prisma · SQLAlchemy · Pydantic · Celery · BullMQ |
| **Database & storage** | PostgreSQL · pgvector · Redis · S3-compatible object storage (SeaweedFS) |
| **Infrastructure & DevOps** | Docker · Docker Compose · nginx · GitHub Actions · Prometheus · Grafana · Alertmanager · n8n |
| **AI & automation** | Ollama · qwen2.5 · bge-m3 |
| **Development tools** | Git · pnpm · Turborepo · Jest · Vitest · Playwright · pytest · Axe · ESLint · Ruff |

## Featured Projects

Two public projects best represent how I work. Both are documented, include real test evidence, and state their limitations instead of hiding them.

### RESOLVE — Invoice exception operations

`Python` `FastAPI` `PostgreSQL + pgvector` `React` `Docker`

An invoice exception platform built around the work that happens after a problem is detected: collecting evidence, proposing a resolution, and getting a human decision that can be audited later. A deterministic parser handles PDFs, Office files, CSVs, and scans; ten versioned rules classify exceptions; and a local LLM investigates through hybrid retrieval. Every AI citation is checked against a real document, page, chunk, or case before it is shown, and the model has no tools or write access.

- **Engineering highlights:** modular monolith with explicit domain modules; approval decisions claimed with a conditional `UPDATE` so concurrent requests cannot both succeed; transactional outbox for n8n events; idempotent execution; audit trail and role-based permissions.
- **Quality evidence:** 137 backend tests, 10 Playwright end-to-end tests over HTTPS, plus documented acceptance and security checks.
- **Readiness:** v1.0.0 portfolio/demo release. It is not production-ready, and the repository documents why.

[Repository](https://github.com/Mindenry/resolve-invoice-ops) · [Architecture overview](https://github.com/Mindenry/resolve-invoice-ops/blob/main/portfolio/PROJECT_OVERVIEW.md) · [Release notes](https://github.com/Mindenry/resolve-invoice-ops/releases/tag/v1.0.0) · [Case study](https://peerawit-portfolio.netlify.app/projects/resolve)

### DAYSHIFT — Fashion commerce and retail operations

`TypeScript` `Next.js` `NestJS` `PostgreSQL` `Prisma` `Redis`

A full-stack Thai fashion commerce platform: a bilingual Thai/English storefront, a staff operations portal, a NestJS commerce API, and a BullMQ worker in one pnpm/Turborepo monorepo. Checkout is server-authoritative: prices are calculated in integer cents, inventory is reserved atomically with expiry, and payment webhooks are HMAC-verified and idempotent. Refunds are serialised per order, and order transitions follow a controlled state machine with permission checks.

- **Engineering highlights:** modular monolith with transactional inventory and order invariants; granular RBAC and ownership checks; structured API errors with request IDs; a shared design system across storefront and admin; Playwright purchase and admin flows plus Axe accessibility scans.
- **Quality evidence:** Jest unit tests, Node integration, exchange, smoke, and workflow suites, with a documented test matrix.
- **Readiness:** portfolio/demo ready, not production-ready. Payments, shipping, and email use sandbox or local adapters.

[Repository](https://github.com/Mindenry/DAYSHIFT) · [Architecture](https://github.com/Mindenry/DAYSHIFT/blob/main/docs/ARCHITECTURE.md) · [Testing](https://github.com/Mindenry/DAYSHIFT/blob/main/docs/TESTING.md) · [Case study](https://peerawit-portfolio.netlify.app/projects/dayshift)

### Other selected work

| Repository | What it covers | Stack |
| :-- | :-- | :-- |
| [NEXORA POS](https://github.com/Mindenry/nexora-pos) | Thai retail POS with inventory, PromptPay, and operations | TypeScript |
| [Bloome](https://github.com/Mindenry/bloome-flower-studio) | Premium flower e-commerce platform | Next.js · TypeScript · Kysely |
| [Team Connect Hub](https://github.com/Mindenry/team-connect-hub) | Meetings, chat, tasks, files, and reporting in a React demo with an in-browser mock API | React · TypeScript |

## Engineering Interests

- **Full-stack application development** — building the product surface, API, and data model as one coherent system.
- **Backend architecture and API design** — domain boundaries, transactional workflows, and contracts that stay understandable.
- **Database design** — schema modelling, versioned migrations, and integrity under concurrent writes.
- **Authentication and authorization** — sessions, role permissions, and tenant isolation.
- **Application security** — webhook verification, input validation, and least-privilege access.
- **Automated testing** — unit, integration, end-to-end, accessibility, and failure-path checks.
- **Deployment and infrastructure** — containerised environments, observability, and backup/restore.
- **AI integration with human oversight** — retrieval-grounded assistance that explains and recommends, but does not decide.

## Connect

- **Portfolio** — [peerawit-portfolio.netlify.app](https://peerawit-portfolio.netlify.app/) — project case studies and engineering notes
- **GitHub** — [github.com/Mindenry](https://github.com/Mindenry)
- **Email** — [peerawitm1xnd@gmail.com](mailto:peerawitm1xnd@gmail.com)
- **Resume** — [PDF](https://peerawit-portfolio.netlify.app/peerawit-lakhampa-resume.pdf)
