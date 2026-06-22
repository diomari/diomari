# Hi, I'm Diomari 👋

I'm a product-minded full-stack engineer building AI-enabled products,
serverless systems, developer tools, and fast frontend experiences.

I like working at the intersection of product, architecture, and implementation:
turning ambiguous ideas into scoped systems, shipping the smallest useful loop,
and then hardening it with clear boundaries, tests, documentation, and operational
visibility.

- 🌐 Portfolio: [diom.dev](https://diom.dev)
- 💻 GitHub: [github.com/diomari](https://github.com/diomari)
- 🔗 LinkedIn: [linkedin.com/in/diomari](https://linkedin.com/in/diomari)
- ✉️ Email: [hello@diom.dev](mailto:hello@diom.dev)

## What I build

I focus on practical software that connects product value with strong technical
foundations:

- **AI product systems** — grounded assistants, AI agent workflows, human-in-the-loop approvals, retrieval, evaluation, cost controls, and safe automation.
- **Cloudflare-native apps** — Workers, Hono, D1, R2, Queues, Durable Objects, Workflows, Workers AI, AI Gateway, and serverless deployment patterns.
- **Developer tools** — CLIs, coding-agent packages, project scanners, workflow helpers, and tools that improve engineering feedback loops.
- **Frontend products** — React, Astro, React Native, Expo, polished UI, performance-minded animation, accessibility, and maintainable component systems.
- **Product engineering** — scoping, architecture, requirements clarification, milestone planning, async communication, documentation, and code review.

## Current themes

A lot of my recent work explores how engineers can use AI without giving up
judgment, maintainability, or user trust.

I keep coming back to a few principles:

- AI features should solve a workflow problem, not just add a chatbot.
- Human approval is a system concern, not a button on top of an unsafe process.
- Serverless architecture is strongest when each primitive has a clear job.
- Good developer tools make context, constraints, and uncertainty visible.
- Small, well-scoped loops beat impressive demos that cannot be operated.
- Documentation and async writing are infrastructure for remote teams.

## Featured projects


### JigSpot

**Offline-first fishing app for offshore anglers.**

JigSpot is a React Native app for Filipino anglers who fish offshore, where
signal is unreliable and generic maps do not show the seafloor detail needed for
jigging and bottom fishing.

- **Stack:** React Native, Expo, MapLibre, Cloudflare Workers, D1, TypeScript.
- **Product:** Offline bathymetric maps, GPS trip tracking, spot saving, catch logging, trusted-circle sharing, and conditions history.
- **Offline-first:** The phone is the source of truth during a trip; cloud sync is for sharing and backup.
- **Maps:** Vector depth contours, structure edges, target-depth highlighting, and examine-area tools for depth/slope/fishability.
- **Backend:** 100% serverless Cloudflare API for sync, sharing, feature gates, and account/product flows.
- **Premium model:** Features such as offline downloads, premium maps, broadcast, and spot limits are gated server-side.

**Key idea:** For field apps, the riskiest loop is often offline behavior. The
product has to keep working exactly when the network disappears.

---

### Gorgi

**A one-line-to-embed grounded AI chat widget for websites.**

Gorgi is a multi-tenant AI assistant that answers from a site's own content
instead of behaving like a generic chatbot. A business signs up, adds a knowledge
source, drops one script tag onto its site, and visitors get grounded answers
with cost controls and tenant isolation.

- **Stack:** Cloudflare Workers, Hono, Workers AI, D1, React, TypeScript.
- **Product loop:** Create a site, add knowledge, embed one script, ask grounded questions, control usage.
- **Frontend:** React dashboard for client/site setup and source management.
- **Embed:** Tiny Shadow DOM widget designed to avoid leaking styles into host pages.
- **Backend:** Edge API for tenant validation, origin checks, quota checks, retrieval, answer generation, and usage tracking.
- **Data model:** D1 stores metadata, site configuration, source references, and usage counters.
- **Isolation:** Every request carries tenant/site context so one site never sees another site's content.

**Key idea:** Embeddable AI products should be boring on purpose: small payload,
strict tenant boundaries, clear quotas, and predictable integration.


---

### Brief Context

**A lightweight handoff tool for AI coding agents.**

Brief Context solves cold-start AI coding sessions by generating a compact
`PROJECT_CONTEXT.md` that Pi, Claude Code, Codex, and terminal workflows can read
before editing a repository.

- **Repo:** [github.com/diomari/brief-ctx](https://github.com/diomari/brief-ctx)
- **Type:** Developer tool / coding-agent package.
- **Stack:** TypeScript, Node.js, pnpm, Node test runner, Pi extension API.
- **Scope:** CLI, Pi extension, prompt templates, Claude Code and Codex adapters, scanner heuristics, cache writing, tests, and package metadata.
- **Core design:** Host-agnostic TypeScript core handles detection, rendering, output path safety, cache writing, and orchestration.
- **Output:** Writes `PROJECT_CONTEXT.md` and `.pi/brief.json` for stable detection data and change hints.
- **Safety:** Avoids real environment files, ignores noisy/generated directories, caps reads and walks, rejects unsafe output paths, and reports unknowns instead of inventing architecture.
- **Validation:** Typecheck, tests, and `npm pack --dry-run` in CI.

**Key idea:** Agent tooling does not always need more intelligence. Sometimes the
best feature is a small, factual, safe handoff before the first prompt.


## Tools and technologies I use often

### Languages and runtimes

- TypeScript
- JavaScript
- Node.js
- React
- React Native
- Astro

### Frontend

- React
- Vite
- Astro Content Collections
- Tailwind CSS
- Vanilla CSS design tokens
- GSAP
- ScrollTrigger
- Lenis
- MapLibre
- Expo

### Backend and serverless

- Cloudflare Workers
- Hono
- D1
- R2
- Queues
- Durable Objects
- Durable Workflows
- Workers AI
- AI Gateway
- Wrangler

### Data, validation, and product infrastructure

- Drizzle
- Zod
- TanStack Query
- Auth/product flow design
- Usage metering and quota checks
- Tenant isolation
- Approval workflows
- Audit trails
- CSV export and admin tooling

### Developer tooling

- CLI design
- npm package publishing
- GitHub Actions
- Typecheck/test/package validation
- AI coding agent workflows
- Project scanning and generated context
- Documentation and decision records


## My portfolio site

My portfolio is also a project I maintain carefully.

- **Site:** [diom.dev](https://diom.dev)
- **Stack:** Astro 6, TypeScript, Astro View Transitions, GSAP, ScrollTrigger, Lenis, vanilla CSS, Content Collections, Shiki, Web3Forms, Cloudflare Pages.
- **Content:** Markdown-powered projects and blog posts.
- **Priorities:** Performance, lean bundle size, polished interaction, and durable content structure.
- **Extra:** Local/free article narration pipeline using Piper/Kokoro experiments and publish tooling.


