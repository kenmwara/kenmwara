<!-- Goes at github.com/kenmwara/kenmwara/README.md -->

### Hi, I'm Ken 👋

Solo operator running a seven-product portfolio out of Vancouver, BC. I build, ship, and run automated systems end-to-end — strategy, code, Cloudflare infrastructure, payments, content, analytics, customer ops.

Most of what I work on makes money rather than stars, so my public footprint is selective. The repos below are showcases — architecture, decisions, and screenshots — without the moats (strategy logic, conversion copy, customer lists).

---

### 🚀 What I'm operating

**[T BOT](https://github.com/kenmwara/tbot)** &mdash; multi-surface algorithmic trading platform on Kalshi prediction markets — live ST weather surface plus macro/equities/crypto lanes in paper validation (surfaces earn live capital by proving an edge; forex was retired on evidence in June 2026). AI prediction pipeline (Claude ensemble), 10-gate risk chain, copy-trade subscriber pilot with Stripe billing. Live demo: [tbot.trade/demo](https://tbot.trade/demo).

**[Unified Ops Dashboard](https://github.com/kenmwara/unified-ops-dashboard)** &mdash; one dashboard, six products, single Cloudflare-native data plane. D1 + Workers + Pages + Email Routing wired into an append-only event store. The platform every other product reports into.

**[tbot-client](https://github.com/kenmwara/tbot-client)** &mdash; open-source Python client that runs on subscriber machines and places orders against the subscriber's own broker (the original signal-feed model; the live pilot now runs a server-side copy-trade engine with encrypted per-subscriber API keys).

**[OddsEdge](https://github.com/kenmwara/oddsedge)** &mdash; AI sports-intelligence subscription — "an AI analyst in your inbox every morning." A daily Claude-written brief delivered over email + Telegram, free-teaser → paid-full tiers, with an auto-graded public track record. Niche-agnostic engine (a new vertical is one JSON config + a cron line), Cloudflare-native, autonomous on a droplet, Whop-billed. Live: [oddsedge.win](https://oddsedge.win).

**[Maasai Explained — AI film studio](https://github.com/kenmwara/maasai-explained-pipeline)** &mdash; multi-channel autonomous documentary studio (Maasai Explained + The Collapse Files): evidence-driven research Brain, audio-first assembly, letter-by-letter frame proofreading, measured multi-model supply chain (Gemini Omni Flash, nano-banana-2, Veo 3).

**[Canadian PR Mastery](https://github.com/kenmwara/canadian-pr-mastery)** &mdash; $497 CAD info product helping skilled workers navigate the Canadian permanent residency process. Cloudflare Pages, Stripe, quiz-driven autoresponder Worker.

**[The Reinvention Blueprint](https://github.com/kenmwara/reinvention-blueprint)** &mdash; info product on career and life reinvention. Cloudflare Pages + Resend sequencing + Workers-based lead capture.

**[Lean Body Blueprint](https://github.com/kenmwara/lean-body-blueprint)** &mdash; $97 fitness funnel for 9-to-5 workers. Landing page, Stripe checkout, 5-episode video sequence, YouTube remarketing.

**[n8n × Claude Sonnet pipeline](https://github.com/kenmwara/n8n_anthropic_claudesonnet4)** &mdash; scheduled video-generation pipeline orchestrated through n8n with Anthropic Claude Sonnet 4 as the reasoning model.

---

### 🛠 What I work with

| Domain | Tools |
|---|---|
| **Languages** | Python, TypeScript/JavaScript, Bash, SQL |
| **Web** | FastAPI, Node, Cloudflare Workers, vanilla HTML/CSS/JS where the framework would be overkill |
| **Cloud / Infra** | Cloudflare (Workers, Pages, D1, R2, KV, Email Routing, Cache Rules, DNS), DigitalOcean, systemd, PM2 |
| **AI / LLMs** | Anthropic Claude, OpenAI, Google Gemini, DeepSeek, n8n for orchestration |
| **Brokers / Markets** | Kalshi API, OANDA v20, Interactive Brokers (ibeam) |
| **Payments / Email** | Stripe Payment Links, Resend, Cloudflare Email Routing |
| **Data** | Cloudflare D1 (SQLite at the edge), append-only JSONL with fcntl locks, no heavy ORM dependencies |

---

### 📍 Operating principles

- **Surface isolation as primary architecture.** A failure on one product never cascades. Trading FX going down can't hurt Canadian PR sign-ups; Lean Body Blueprint can't drain Reinvention Blueprint's email sender reputation.
- **Append-only audit logs beat mutable state.** Forward-only debuggability wins over database snapshots almost every time. D1 + JSONL covers more ground than people assume.
- **Cloudflare-native by default.** One vendor for DNS, edge, Workers, D1, R2, Pages, email routing. Operational simplicity at six-product scale beats best-of-breed sprawl.
- **Trust earned by transparency, not NDA.** The [T BOT demo page](https://tbot.trade/demo) publishes the actual gating chain, signal pipeline, and callback architecture. Opacity in a trading product is a red flag, not a feature.
- **Ship the smallest thing that works, then watch it for a week before adding the next thing.**

---

### 📫 Connect

[LinkedIn](https://linkedin.com/in/kenmwara) &nbsp;·&nbsp; [X](https://x.com/Ken_Mwara) &nbsp;·&nbsp; [YouTube](https://youtube.com/@kenmwara3955) &nbsp;·&nbsp; Vancouver, BC

Open to interesting conversations — algo trading, multi-tenant signal delivery, Cloudflare-native ops architecture, or how to run seven products as a solo operator without losing your mind.
