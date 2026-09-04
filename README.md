<!-- Goes at github.com/kenmwara/kenmwara/README.md — source of truth: github-showcase/PROFILE_README.md (fetch the live file before editing; ship via SHIP.md Step 3) -->

### Hi, I'm Ken 👋

Solo operator running a multi-product portfolio out of Vancouver, BC — plus a small web studio for client sites. I build, ship, and run automated systems end-to-end — strategy, code, Cloudflare infrastructure, native mobile, payments, content, analytics, customer ops.

Most of what I work on makes money rather than stars, so my public footprint is selective. The repos below are showcases — architecture, decisions, and screenshots — without the moats (strategy logic, conversion copy, customer lists). The live products are linked; the portfolio page with screenshots is at [tbot.trade/portfolio](https://tbot.trade/portfolio).

---

### 🚀 What I'm operating

**[T BOT](https://github.com/kenmwara/tbot)** &mdash; multi-surface algorithmic trading platform on Kalshi prediction markets — live ST weather surface plus macro/equities/crypto lanes in paper validation (surfaces earn live capital by proving an edge; forex was retired on evidence in June 2026). AI prediction pipeline (Claude ensemble), a 14-layer guard chain with fifteen codified disciplines, copy-trade subscriber pilot with Stripe billing. Rebuilt from git + the secrets vault to live trading in one evening after a total server loss (Sept 2026). Live demo: [tbot.trade/demo](https://tbot.trade/demo).

**[JobScout](https://github.com/kenmwara/jobscout-app)** &mdash; AI job-search copilot, shipped as a product. Public demo at [jobscout.tbot.trade](https://www.jobscout.tbot.trade): the pipeline's real daily sweep, deterministic eligibility gates, then live Claude scoring on a bearing dial with the reasoning shown and the cost on screen — behind a per-visitor rate limit and a daily budget breaker that degrades honestly. The same guarded API has **fully native** Android (Kotlin · Jetpack Compose) and iOS (Swift · SwiftUI) clients, both built in Codemagic CI. The private pipeline behind it sweeps ~1,400 postings a day and applies to jobs as me — a human clicks every Submit.

**[Unified Ops Dashboard](https://github.com/kenmwara/unified-ops-dashboard)** &mdash; one dashboard, six products, single Cloudflare-native data plane. D1 + Workers + Pages + Email Routing wired into an append-only event store, behind Cloudflare Access. The platform every other product reports into.

**[tbot-client](https://github.com/kenmwara/tbot-client)** &mdash; open-source Python client that runs on subscriber machines and places orders against the subscriber's own broker (the original signal-feed model; the live pilot now runs a server-side copy-trade engine with encrypted per-subscriber API keys).

**[OddsEdge](https://github.com/kenmwara/oddsedge)** &mdash; AI sports-intelligence subscription — "an AI analyst in your inbox every morning." A daily Claude-written brief delivered over email + Telegram, free-teaser → paid-full tiers, with an auto-graded public track record. Niche-agnostic engine (a new vertical is one JSON config + a cron line), Cloudflare-native, autonomous on a droplet, Whop-billed. Live: [oddsedge.win](https://oddsedge.win).

**[Content Studio — AI film studio](https://github.com/kenmwara/maasai-explained-pipeline)** &mdash; a two-channel autonomous documentary studio: **[Zamani](https://youtube.com/@ZamaniHistory)** ("Africa, before you were told" — a film every Sunday) and **[The Fortune Files](https://youtube.com/@fortunefiles_HQ)** (the full arc of money & power from court records and filings — every Thursday). Evidence-driven research Brain, audio-first assembly, letter-by-letter frame proofreading, a measured multi-model supply chain (Gemini, Veo 3, Kie), and a pre-render validator that gates every film.

**T BOT Web Studio** &mdash; client sites designed in Chat and shipped by Code on Cloudflare Pages — e.g. [Sacred Earth](https://sacred-earth.pages.dev), a Uganda travel brand's field-guide site: a scroll-driven altitude sweep over a canvas point-cloud of the country, 15 self-contained pages from one builder, self-hosted fonts, zero runtime network calls.

**[Canadian PR Mastery](https://github.com/kenmwara/canadian-pr-mastery)** &mdash; $497 CAD info product helping skilled workers navigate the Canadian permanent residency process. Cloudflare Pages, Stripe, quiz-driven autoresponder Worker.

**[The Reinvention Blueprint](https://github.com/kenmwara/reinvention-blueprint)** &mdash; info product on career and life reinvention. Cloudflare Pages + Resend sequencing + Workers-based lead capture.

**[Lean Body Blueprint](https://github.com/kenmwara/lean-body-blueprint)** &mdash; $97 fitness funnel for 9-to-5 workers. Landing page, Stripe checkout, 5-episode video sequence, YouTube remarketing.

**[n8n × Claude Sonnet pipeline](https://github.com/kenmwara/n8n_anthropic_claudesonnet4)** &mdash; scheduled video-generation pipeline orchestrated through n8n with Anthropic Claude Sonnet 4 as the reasoning model.

---

### 🛠 What I work with

| Domain | Tools |
|---|---|
| **Languages** | Python, TypeScript/JavaScript, Kotlin, Swift, Bash, SQL |
| **Web** | FastAPI, Node, Cloudflare Workers, vanilla HTML/CSS/JS where the framework would be overkill |
| **Mobile** | Kotlin + Jetpack Compose, Swift + SwiftUI, Capacitor, Codemagic CI |
| **Cloud / Infra** | Cloudflare (Workers, Pages, D1, R2, KV, Email Routing, Access, Cache Rules, DNS), DigitalOcean, systemd, PM2 |
| **AI / LLMs** | Anthropic Claude, OpenAI, Google Gemini, DeepSeek, n8n for orchestration |
| **Brokers / Markets** | Kalshi API, OANDA v20, Interactive Brokers (ibeam) |
| **Payments / Email** | Stripe Payment Links, Whop, Resend, Cloudflare Email Routing |
| **Data** | Cloudflare D1 (SQLite at the edge), append-only JSONL with fcntl locks, no heavy ORM dependencies |

---

### 📍 Operating principles

- **Surface isolation as primary architecture.** A failure on one product never cascades. A trading lane going down can't hurt Canadian PR sign-ups; Lean Body Blueprint can't drain Reinvention Blueprint's email sender reputation.
- **Append-only audit logs beat mutable state.** Forward-only debuggability wins over database snapshots almost every time. D1 + JSONL covers more ground than people assume.
- **Cloudflare-native by default.** One vendor for DNS, edge, Workers, D1, R2, Pages, email routing, access control. Operational simplicity at portfolio scale beats best-of-breed sprawl.
- **Numbers are labeled, never fabricated.** Measured from logs, modeled from stated assumptions, or absent — every public figure says which. The [T BOT demo page](https://tbot.trade/demo) publishes the actual gating chain and signal pipeline; opacity in a trading product is a red flag, not a feature.
- **Ship the smallest thing that works, then watch it for a week before adding the next thing.**

---

### 📫 Connect

[LinkedIn](https://linkedin.com/in/kenmwara) &nbsp;·&nbsp; [X](https://x.com/Ken_Mwara) &nbsp;·&nbsp; [YouTube](https://youtube.com/@ZamaniHistory) &nbsp;·&nbsp; [Portfolio](https://tbot.trade/portfolio) &nbsp;·&nbsp; Vancouver, BC

Open to interesting conversations — algo trading, LLM orchestration in production, native + edge app architecture, or how to run a dozen products as a solo operator without losing your mind.
