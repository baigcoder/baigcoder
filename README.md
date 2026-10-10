<div align="center">

<h1><img src="assets/profile-hero.svg" alt="Muhammad Hassan Baig, Full-Stack AI Engineer, at the centre of a network of technologies he uses: TypeScript, React, Node.js, PostgreSQL, Redis, LLM and RAG, and Docker." width="100%"></h1>

**Muhammad Hassan Baig** · Full-Stack AI Engineer

Engineering AI-powered products, reliable backend systems and intelligent developer tools.

[Portfolio](https://hassan-baigo-portfolio.vercel.app/) · [Best work](#best-work) · [TrueVibe case study](#truevibe-a-case-study) · [Repositories](https://github.com/baigcoder?tab=repositories)

[![TrueVibe last commit](https://img.shields.io/github/last-commit/baigcoder/TrueVibe?label=TrueVibe%20last%20commit&style=flat-square&color=55D6FF&labelColor=101725)](https://github.com/baigcoder/TrueVibe/commits)
[![Wakeel last commit](https://img.shields.io/github/last-commit/baigcoder/lawyer-agency?label=Wakeel%20last%20commit&style=flat-square&color=8775FF&labelColor=101725)](https://github.com/baigcoder/lawyer-agency/commits)
[![Followers](https://img.shields.io/github/followers/baigcoder?label=followers&style=flat-square&color=55D6FF&labelColor=101725)](https://github.com/baigcoder?tab=followers)

</div>

I work across the stack: React and Next.js interfaces, Node.js and TypeScript backends, and the data, queue and AI layers behind them. What interests me most is the unglamorous engineering that makes AI features trustworthy: validated model output, idempotent queues, tenant isolation, and graceful degradation when a provider fails.

## Best work

<div align="center">
<a href="https://github.com/baigcoder/TrueVibe"><img src="assets/showcase-truevibe.svg" alt="TrueVibe: social platform that scores media authenticity with a Python AI service. React, Express, MongoDB, FastAPI. Demo and source." width="400"></a>
<a href="https://github.com/baigcoder/lawyer-agency"><img src="assets/showcase-wakeel.svg" alt="Wakeel: multi-tenant AI front desk for law firms with lawyer handoff briefs. NestJS, Next.js, Postgres, pgvector. Source." width="400"></a>
<a href="https://github.com/baigcoder/hire-os"><img src="assets/showcase-hireos.svg" alt="HIRE.OS: resume analysis, AI assessments and WebRTC interviews in one platform. React, Node, MongoDB, Supabase. Demo and source." width="400"></a>
<a href="https://github.com/baigcoder/rivulet"><img src="assets/showcase-rivulet.svg" alt="Rivulet: media library and BitTorrent player for desktop and Android TV. TypeScript, embedded mpv. Site and source." width="400"></a>
<a href="https://github.com/baigcoder/brewns"><img src="assets/showcase-brewns.svg" alt="Brewns: coffee house site with three.js product views and receipt ordering. Next.js 16, three.js. Site and source." width="400"></a>
<a href="https://github.com/baigcoder/grizzly"><img src="assets/showcase-grizzly.svg" alt="Grizzly: real-time 3D product site where you pick up, turn and crack open the can. React, Three.js, GSAP. Source." width="400"></a>
</div>

| Project | Source | Live link |
| --- | --- | --- |
| TrueVibe | [baigcoder/TrueVibe](https://github.com/baigcoder/TrueVibe) | [true-vibe.vercel.app](https://true-vibe.vercel.app/) |
| Wakeel | [baigcoder/lawyer-agency](https://github.com/baigcoder/lawyer-agency) | none yet |
| HIRE.OS | [baigcoder/hire-os](https://github.com/baigcoder/hire-os) | [hire-os.vercel.app](https://hire-os.vercel.app) |
| Rivulet | [baigcoder/rivulet](https://github.com/baigcoder/rivulet) | [rivulet-beige.vercel.app](https://rivulet-beige.vercel.app) |
| Brewns | [baigcoder/brewns](https://github.com/baigcoder/brewns) | [brewns-chi.vercel.app](https://brewns-chi.vercel.app) |
| Grizzly | [baigcoder/grizzly](https://github.com/baigcoder/grizzly) | none listed |

Live links come from each repository's metadata or README. I haven't load-tested or benchmarked any of these.

### More builds

- **[CreatorVerse](https://github.com/baigcoder/creatorverse):** full-stack creator learning platform. [Live](https://creatorverse-web-two.vercel.app)
- **[Nexus POS](https://github.com/baigcoder/nexus-pos):** point-of-sale app in TypeScript. [Live](https://nexus-pos-nine.vercel.app)
- **[Pure CV Builder](https://github.com/baigcoder/pure-cv-builder):** CV builder in TypeScript. [Live](https://pure-cv-builder-frontend.vercel.app)
- **[Shopping Expense Tracker](https://github.com/baigcoder/shopping-expense-tracker):** expense tracker in TypeScript. [Live](https://shopping-expense-trackerfrontend.vercel.app)
- **[Humza Portfolio](https://github.com/baigcoder/humza-portfolio):** corporate financial advisory site. [Live](https://humza-portfolio-xi.vercel.app)
- **[Pakistan Luxury Dresscode](https://github.com/baigcoder/pakistan-luxury-dresscode):** TypeScript web app. [Live](https://pakistan-luxury-dresscode.vercel.app)

## TrueVibe: a case study

<div align="center">
<a href="https://github.com/baigcoder/TrueVibe"><img src="assets/truevibe-architecture.svg" alt="TrueVibe architecture: a React and Vite client, a Node.js and Express API with MongoDB, Redis, BullMQ and Socket.IO, and a separate Python FastAPI AI service. An evidence-fusion step exists on the dev branch only." width="640"></a>
</div>

**Problem.** On social platforms, manipulated media is easy to post and hard to judge. TrueVibe is built around one question: can you trust what you're looking at?

**Approach.** Uploaded media goes to a separate Python service that produces a trust verdict, so the interface can show authenticity signals instead of leaving users to guess. Real-time features run on the Node API.

**Engineering contribution.** On the `dev` branch, an evidence-fusion step only supports a "fake" verdict when independent forensic signals (FFT, eye, colour and noise, edge, mouth, temporal) corroborate the primary model's score. The aim is that no single over-confident model decides alone. That module is **not on `main`**.

**Stack, verified in the repository.**
- *Client:* React 19, Vite, TypeScript, TanStack Router and Query, Tailwind CSS, Framer Motion.
- *API:* Node.js, Express, MongoDB, Redis with BullMQ, Socket.IO, Zod, Helmet.
- *AI service:* FastAPI, PyTorch and `transformers` (CPU build), OpenCV, image and video analysis, PDF report.
- *Delivery:* Docker Compose, GitHub Actions CI, Vercel and Railway configuration.

**Status, stated plainly.** I built this myself. I haven't published accuracy numbers or benchmarks, and the repository has no Kubernetes manifests. I don't claim production traffic, horizontal scaling or security guarantees.

[Source](https://github.com/baigcoder/TrueVibe) · [Live app](https://true-vibe.vercel.app/) · [Changelog](https://github.com/baigcoder/TrueVibe/blob/HEAD/CHANGELOG.md)

<details>
<summary><strong>Wakeel</strong>: AI front desk for law firms</summary>

**Problem.** Pakistani law firms run intake, fees and documents through WhatsApp, and partners re-read long chats.<br>
**Approach.** A multi-tenant WhatsApp front desk where an AI handles intake, scheduling and document requests, then hands a structured brief to a lawyer. It never gives legal advice, and a web dashboard serves the staff.<br>
**Contribution.** PostgreSQL row-level security with `FORCE`; ack-fast webhooks with idempotent queue consumers; per-conversation locking; a deterministic fallback for every model call; and Urdu and Roman Urdu handling for voice replies.<br>
**Stack.** TypeScript, NestJS, Next.js, PostgreSQL with pgvector, Redis, BullMQ, Prisma.<br>
**Status.** Phases 1–15 are in the repository. Its README lists hosting, backups and alerting as next steps, so I don't present it as deployed.

</details>

<details>
<summary><strong>HIRE.OS</strong>: AI recruitment platform</summary>

**Problem.** Hiring spans resume screening, assessment and interviewing, usually across separate tools.<br>
**Approach.** One platform with a resume analyser, AI-generated assessments with proctoring signals, WebRTC interviews, and recruiter and candidate dashboards.<br>
**Contribution.** Per-feature model selection with a fallback model, and live dashboards on Supabase Realtime.<br>
**Stack.** React, Node.js, Express, MongoDB, Redis, Supabase.

</details>

## Technical stack

Used in my projects:

| Area | Tools |
| --- | --- |
| Languages and frontend | TypeScript, JavaScript, Python, SQL; React, Next.js, Vite, Tailwind CSS, TanStack Query and Router, Framer Motion, three.js, GSAP |
| Backend and APIs | Node.js, Express, NestJS, REST, Socket.IO, WebRTC, Zod |
| Databases and caching | PostgreSQL (RLS, pgvector), MongoDB, Redis, BullMQ, Prisma, Mongoose, Supabase |
| Applied AI and LLMs | OpenAI-compatible and Gemini APIs, RAG with pgvector, PyTorch and `transformers` inference, FastAPI model services, speech-to-text and text-to-speech |
| Infrastructure and automation | Docker and Compose, nginx, GitHub Actions, Vercel, Railway |

Still learning, so not claimed as experience: LangGraph, CrewAI, MCP, Unsloth, Kubernetes, AWS.

## Engineering focus

- **Agents and orchestration:** LangGraph, CrewAI, and MCP servers.
- **LLM applications:** retrieval quality, evaluation, and fine-tuning with Hugging Face and Unsloth.
- **Distributed systems:** event-driven design, queues and idempotency.
- **Platform:** Kubernetes and AWS, plus developer automation.

> Understand the problem → Design the system → Implement → Test → Deploy → Observe → Improve

## GitHub activity

<div align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/baigcoder/baigcoder/output/github-contribution-grid-snake-dark.svg">
  <img alt="Contribution graph animated as a snake eating contribution cells" src="https://raw.githubusercontent.com/baigcoder/baigcoder/output/github-contribution-grid-snake.svg">
</picture>
</div>

## Contact

Open to collaborating on AI products, SaaS, backend engineering, developer tooling and open source. Reach me through my [portfolio](https://hassan-baigo-portfolio.vercel.app/) or an issue on any repository above.

<!-- Add a verified LinkedIn URL and public email here when ready. -->

<div align="center">
<sub>Built with intent: real software, honest engineering, better systems each time.</sub>
</div>
