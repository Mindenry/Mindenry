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

I build full-stack web applications and the systems behind them: interfaces, APIs, data models, background jobs, and the tests that keep the important paths correct. I like problems that have to hold up outside a demo, such as concurrent approvals, inventory that stays correct under concurrent checkout, and AI that recommends without deciding.

Currently open to software engineering opportunities.

## About

I'm a full-stack developer based in Bangkok, working mainly in TypeScript and Python. My projects are built as monorepos or modular monoliths with clear domain boundaries, versioned migrations, and documented limits. I care about server-side authorization, concurrency, tested failure paths, and release notes that say what is not ready. I'm looking for a team where I can keep learning from engineers who have shipped more than I have.

## Tech Stack

| Area | Core technologies |
| :-- | :-- |
| **Languages** | TypeScript · Python · SQL |
| **Frontend** | React · Next.js · Tailwind CSS |
| **Backend** | Node.js · NestJS · FastAPI · Prisma · SQLAlchemy · Celery · BullMQ |
| **Data & infrastructure** | PostgreSQL · pgvector · Redis · Docker · GitHub Actions |
| **AI & automation** | Ollama · n8n |
| **Testing** | Playwright · Jest · Vitest · pytest · Axe |

## Featured Projects

Two public projects best represent how I work. Both are documented, tested, and explicit about what is not production-ready.

### RESOLVE — Invoice exception operations

`Python` `FastAPI` `PostgreSQL + pgvector` `React`

An invoice exception platform for the work after detection: deterministic parsing and ten versioned rules find problems, a local LLM gathers evidence through hybrid retrieval, and every citation is checked against a real record. Approvals are human-only and concurrency-safe, with an audit trail; the model cannot approve or execute.

- **Testing:** 130+ backend tests, 10 Playwright end-to-end tests, plus documented acceptance and security checks.
- **Status:** v1.0.0 portfolio/demo release; not production-ready.

[Repository](https://github.com/Mindenry/resolve-invoice-ops) · [Architecture](https://github.com/Mindenry/resolve-invoice-ops/blob/main/portfolio/PROJECT_OVERVIEW.md) · [Release notes](https://github.com/Mindenry/resolve-invoice-ops/releases/tag/v1.0.0) · [Case study](https://peerawit-portfolio.netlify.app/projects/resolve)

### DAYSHIFT — Fashion commerce and retail operations

`TypeScript` `Next.js` `NestJS` `PostgreSQL` `Prisma` `Redis`

A bilingual Thai/English commerce platform with a storefront, staff operations portal, NestJS API, and BullMQ worker. Checkout is server-authoritative: prices are computed in integer cents, inventory is reserved atomically, payment webhooks are HMAC-verified and idempotent, and order transitions follow a controlled state machine. Refunds for the same order are serialised, and the integration suite asserts exactly one success when two requests try to refund the same return concurrently.

- **Testing:** Jest unit tests; integration, smoke, and workflow suites; Playwright; and Axe accessibility checks.
- **Status:** Portfolio/demo ready; not production-ready. Payments, shipping, and email use sandbox or local adapters.

[Repository](https://github.com/Mindenry/DAYSHIFT) · [Architecture](https://github.com/Mindenry/DAYSHIFT/blob/main/docs/ARCHITECTURE.md) · [Testing](https://github.com/Mindenry/DAYSHIFT/blob/main/docs/TESTING.md) · [Case study](https://peerawit-portfolio.netlify.app/projects/dayshift)

### Other selected work

- **[NEXORA POS](https://github.com/Mindenry/nexora-pos)** — Thai retail POS with inventory, PromptPay QR, and RBAC. `React` `Express` `PostgreSQL`
- **[Bloome](https://github.com/Mindenry/bloome-flower-studio)** — Bilingual flower storefront with transactional checkout and admin. `Next.js` `TypeScript` `Kysely`
- **[Team Connect Hub](https://github.com/Mindenry/team-connect-hub)** — Collaboration workspace demo with an in-browser mock API. `React` `TypeScript`

## Engineering Interests

- Full-stack application development
- Backend architecture and API design
- Database design and data integrity
- Authentication and authorization
- Application security
- Automated testing
- Deployment and infrastructure
- AI integration with human oversight

## Connect

- **Portfolio** — [peerawit-portfolio.netlify.app](https://peerawit-portfolio.netlify.app/) — case studies and engineering notes
- **GitHub** — [github.com/Mindenry](https://github.com/Mindenry)
- **Email** — [peerawitm1xnd@gmail.com](mailto:peerawitm1xnd@gmail.com)
- **Resume** — [PDF](https://peerawit-portfolio.netlify.app/peerawit-lakhampa-resume.pdf)
