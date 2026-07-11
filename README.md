# Asikur Rahman

Full-stack engineer in Dhaka. I build multi-tenant SaaS backends — real-time systems, queue-driven pipelines, fleet telemetry, LLM orchestration, and the billing and access-control layers underneath them.

Currently at **OrangeToolz**, where I've built two products end to end and contributed to two more.

**Stack** — TypeScript · JavaScript · PHP · NestJS · Node.js · PostgreSQL · Prisma · Redis · BullMQ · Socket.io · React · Next.js · Docker · Kubernetes
**AI** — OpenRouter (multi-provider orchestration) · MCP · RAG

---

### Built end to end

**[Wagend](https://app.wagend.com)** — Multi-tenant WhatsApp Business CRM

Real-time inbox on Socket.io with the Redis adapter, so sessions and presence survive horizontal scaling instead of being pinned to one node. Chunked CSV ingestion through parallel BullMQ workers. Stripe subscriptions with idempotent webhooks. Four-tier RBAC enforced at the NestJS guard layer.

*AI layer:* RAG-backed smart reply grounded in each tenant's own templates and message history, with MCP tool integration. All inference routed through **OpenRouter rather than hard-coded OpenAI** — model choice, fallback and cost/latency trade-offs are configuration, not a code change.

`NestJS` `Prisma` `MySQL` `Redis` `BullMQ` `Socket.io` `OpenRouter` `MCP` `React` `TypeScript`

**WP Activity Logs** — Fleet telemetry across 1,000+ WordPress sites

A PHP/WordPress plugin that streams core activity, content changes and lorem ipsum detection from every site into a central service in real time, and flags broken integrations (Instagram Feed, Business Reviews) before clients notice them. The fleet telemetry is exposed over **MCP**, so an AI agent can query site health directly.

`PHP` `WordPress` `MCP` `Python`

---

### Contributed to

**[Agency Framework](https://app.agencyframework.io)** — Agency operations suite on GoHighLevel

Built the backend services — WebUtility, GHL Reports, Plugins and Notifications — syncing GoHighLevel data into reporting dashboards via an extensible plugin system with a real-time notification layer. Integrated those APIs into the management dashboard, so agencies run every client site from one place: per-site analytics and health scores, content diffs, and licence / domain expiry tracking across the fleet.

`NestJS` `React` `PostgreSQL` `Redis` `TypeScript`

**[Super Local Fans](https://superlocalfans.com)** — Social CRM & UGC platform

Backend services inside a microservices / micro-frontend architecture on Kubernetes. BullMQ drives scheduled publishing across social platforms; Sentry for error tracking.

`NestJS` `GraphQL` `Apollo` `PostgreSQL` `Kubernetes` `Sentry`

---

### Prototypes

**Dialytics** — AI call transcription & analytics. FFmpeg normalisation, Piscina worker threads running transcription and sentiment analysis off the event loop, Markdown-to-PDF reporting via Postmark. *Not currently deployed.*
`Node.js` `Express` `Piscina` `FFmpeg` `MySQL`

---

### Open source

**[linky](https://github.com/awebcode/linky)** — Real-time chat. One-to-one, groups and channels, presence tracking, typing indicators, read receipts, S3 file sharing.
`Node.js` `Socket.io` `Redis` `AWS S3` `React`

**[trippz](https://github.com/awebcode/trippz)** — Travel-booking REST API. Multi-provider OAuth, Stripe payments, Twilio + SendGrid notifications, rate limiting, full Swagger docs.
`Express` `TypeScript` `Prisma` `PostgreSQL`

---

[awebcode.com](https://awebcode.com) · [LinkedIn](https://linkedin.com/in/awebcode) · asikurrahaman997@gmail.com
