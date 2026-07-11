# Asikur Rahman

Full-stack engineer in Dhaka. I build multi-tenant SaaS backends — real-time systems, queue-driven pipelines, LLM orchestration, and the billing and access-control layers underneath them.

Currently at **OrangeToolz**, where I've built two products end to end and contributed to two more.

**Stack** — TypeScript · NestJS · Node.js · PostgreSQL · Prisma · Redis · BullMQ · Socket.io · React · Next.js · Docker · Kubernetes
**AI** — OpenRouter (multi-provider orchestration) · MCP · RAG

---

### Built end to end

**[Wagend](https://app.wagend.com)** — Multi-tenant WhatsApp Business CRM

Real-time inbox on Socket.io with the Redis adapter, so sessions and presence survive horizontal scaling instead of being pinned to one node. Chunked CSV ingestion through parallel BullMQ workers. Stripe subscriptions with idempotent webhooks. Four-tier RBAC enforced at the NestJS guard layer.

*AI layer:* RAG-backed smart reply grounded in each tenant's own templates and message history, with MCP tool integration. All inference routed through **OpenRouter rather than hard-coded OpenAI** — model choice, fallback and cost/latency trade-offs are configuration, not a code change.

`NestJS` `Prisma` `MySQL` `Redis` `BullMQ` `Socket.io` `OpenRouter` `MCP` `React` `TypeScript`

**[Dialytics](https://dialytics.awebcode.com)** — AI call transcription & analytics

FFmpeg normalises uploaded recordings; Piscina worker threads run transcription and sentiment analysis off the event loop; results render to Markdown-to-PDF reports delivered via Postmark. Stripe billing, role-based access, waveform playback.

`Node.js` `Express` `Piscina` `FFmpeg` `Sequelize` `MySQL` `Socket.io` `React`

---

### Contributed to

**[Agency Framework](https://app.agencyframework.io)** — Agency operations suite on GoHighLevel

Built the WebUtility, GHL Reports, Plugins and Notifications modules: GHL data synced into reporting dashboards, an extensible plugin system, and a real-time notification layer.

`NestJS` `React` `PostgreSQL` `Redis` `TypeScript`

**[Super Local Fans](https://superlocalfans.com)** — Social CRM & UGC platform

Backend services inside a microservices / micro-frontend architecture on Kubernetes. BullMQ drives scheduled publishing across social platforms; Sentry for error tracking.

`NestJS` `GraphQL` `Apollo` `PostgreSQL` `Kubernetes` `Sentry`

---

### Open source

**[linky](https://github.com/awebcode/linky)** — Real-time chat. One-to-one, groups and channels, presence tracking, typing indicators, read receipts, S3 file sharing.
`Node.js` `Socket.io` `Redis` `AWS S3` `React`

**[trippz](https://github.com/awebcode/trippz)** — Travel-booking REST API. Multi-provider OAuth, Stripe payments, Twilio + SendGrid notifications, rate limiting, full Swagger docs.
`Express` `TypeScript` `Prisma` `PostgreSQL`

---

[awebcode.com](https://awebcode.com) · [LinkedIn](https://linkedin.com/in/awebcode) · asikurrahaman997@gmail.com
