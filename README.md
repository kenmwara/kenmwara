<!-- Goes at github.com/kenmwara/kenmwara/README.md — source of truth: github-showcase/PROFILE_README.md (fetch the live file before editing; ship via SHIP.md Step 3).
     Screenshots are served from tbot.trade/portfolio/img/* (tbot-platform dashboard/portfolio-img/) and the public jobscout-app repo. -->

### Hi, I'm Ken 👋

Solo operator running a multi-product portfolio out of Vancouver, BC — plus a small web studio for client sites. I build, ship, and run automated systems end-to-end — strategy, code, Cloudflare infrastructure, native mobile, payments, content, analytics, customer ops.

Most of what I work on makes money rather than stars, so my public footprint is selective. The repos below are showcases — architecture, decisions, and screenshots — without the moats (strategy logic, conversion copy, customer lists). Every live product is linked and pictured; the full portfolio page is at [tbot.trade/portfolio](https://tbot.trade/portfolio).

---

### 🚀 What I'm operating

**[T BOT](https://github.com/kenmwara/tbot)** &mdash; multi-surface algorithmic trading platform on Kalshi prediction markets — live ST weather surface plus macro/equities/crypto lanes in paper validation (surfaces earn live capital by proving an edge; forex was retired on evidence in June 2026). AI prediction pipeline (Claude ensemble), a 14-layer guard chain with fifteen codified disciplines, copy-trade subscriber pilot with Stripe billing. Rebuilt from git + the secrets vault to live trading in one evening after a total server loss (Sept 2026). Live demo: [tbot.trade/demo](https://tbot.trade/demo).

<a href="https://tbot.trade/portfolio"><img src="https://tbot.trade/portfolio/img/tbot-dash.jpg" width="300" alt="tbot.trade operator dashboard — one card per surface, health, labeled revenue projection"></a>&nbsp;&nbsp;<a href="https://tbot.trade/demo"><img src="https://tbot.trade/portfolio/img/tbot-demo.jpg" width="300" alt="tbot.trade/demo — algorithmic trading signals delivered to your phone; 15% on realized profit only, $0 custody"></a>

**[JobScout](https://github.com/kenmwara/jobscout-app)** &mdash; AI job-search copilot, shipped as a product. Public demo at [jobscout.tbot.trade](https://www.jobscout.tbot.trade): the pipeline's real daily sweep scored live by Claude with the reasoning shown, the deterministic gate verdicts underneath as receipts — behind a per-visitor rate limit and a daily budget breaker that degrades honestly instead of pretending. It carries **its own design system**: the mark is a bearing rose, and a posting's fit lights its eight bearings. The same guarded API has **fully native** Android (Kotlin · Jetpack Compose) and iOS (Swift · SwiftUI) clients that draw that rose from identical geometry — both green in Codemagic CI, both auto-built on push. The private pipeline behind it sweeps ~1,400 postings a day and applies to jobs as me — a human clicks every Submit.

<a href="https://www.jobscout.tbot.trade"><img src="https://raw.githubusercontent.com/kenmwara/jobscout-app/main/docs/img/00-landing.png" width="440" alt="JobScout — the live demo: pick a candidate, then watch real postings scored by Claude with the reasoning shown"></a>&nbsp;&nbsp;<a href="https://github.com/kenmwara/jobscout-app"><img src="https://raw.githubusercontent.com/kenmwara/jobscout-app/main/docs/img/native/android-02-scoring.jpg" width="150" alt="JobScout on Android — live scoring: the bearing rose lit to each fit, the route band, and the reasoning both ways"></a>

**T BOT Web Studio** &mdash; client sites designed in Chat and shipped by Code on Cloudflare Pages — fixed-price builds plus a recurring care plan. Latest: [Sacred Earth](https://sacred-earth.pages.dev), a Uganda travel brand's field-guide site — a scroll-driven descent down Uganda over a canvas point-cloud of the country — eight stations from Wagagai at 4,321 m to the Nile, each pinned and figure-led as you fall through it. Self-hosted fonts, every ship link-checked and console-clean before it goes live.

<a href="https://sacred-earth.pages.dev"><img src="https://tbot.trade/portfolio/img/sacred-earth.jpg" width="440" alt="Sacred Earth — the Descent: walked down from 4,321 metres, over a canvas point-cloud of Uganda"></a>

**[Unified Ops Dashboard](https://github.com/kenmwara/unified-ops-dashboard)** &mdash; one dashboard, six products, single Cloudflare-native data plane. D1 + Workers + Pages + Email Routing wired into an append-only event store, behind Cloudflare Access. The platform every other product reports into.

<a href="https://github.com/kenmwara/unified-ops-dashboard"><img src="https://tbot.trade/portfolio/img/ops.jpg" width="440" alt="ops.tbot.trade — fleet health pills, flags, scheduler queue, one tile per product, per-project System health cards"></a>

**[tbot-client](https://github.com/kenmwara/tbot-client)** &mdash; open-source Python client that runs on subscriber machines and places orders against the subscriber's own broker (the original signal-feed model; the live pilot now runs a server-side copy-trade engine with encrypted per-subscriber API keys).

**[OddsEdge](https://github.com/kenmwara/oddsedge)** &mdash; AI sports-intelligence subscription — "an AI analyst in your inbox every morning." A daily Claude-written brief delivered over email + Telegram, free-teaser → paid-full tiers, with an auto-graded public track record. Niche-agnostic engine (a new vertical is one JSON config + a cron line), Cloudflare-native, autonomous on a droplet, Whop-billed. Live: [oddsedge.win](https://oddsedge.win).

<a href="https://oddsedge.win"><img src="https://tbot.trade/portfolio/img/oddsedge.jpg" width="440" alt="oddsedge.win — an AI analyst for sports value betting: best price vs fair, the edge quantified, no invented picks"></a>

**[Content Studio — AI film studio](https://github.com/kenmwara/maasai-explained-pipeline)** &mdash; a two-channel autonomous documentary studio: **[Zamani](https://youtube.com/@ZamaniHistory)** ("Africa, before you were told" — a film every Sunday) and **[The Fortune Files](https://youtube.com/@fortunefiles_HQ)** (the full arc of money & power from court records and filings — every Thursday). Evidence-driven research Brain, audio-first assembly, letter-by-letter frame proofreading, a measured multi-model supply chain (Gemini, Veo 3, Kie), and a pre-render validator that gates every film.

<a href="https://youtube.com/@ZamaniHistory"><img src="https://tbot.trade/portfolio/img/zamani.jpg" width="300" alt="Zamani on YouTube — a new film every Sunday"></a>&nbsp;&nbsp;<a href="https://youtube.com/@fortunefiles_HQ"><img src="https://tbot.trade/portfolio/img/fortunefiles.jpg" width="300" alt="The Fortune Files on YouTube — a new file every Thursday"></a>

**[Canadian PR Mastery](https://github.com/kenmwara/canadian-pr-mastery)** &mdash; $497 CAD info product helping skilled workers navigate the Canadian permanent residency process. Cloudflare Pages, Stripe, quiz-driven autoresponder Worker. Live: [canadianprmastery.com](https://canadianprmastery.com).

**[The Reinvention Blueprint](https://github.com/kenmwara/reinvention-blueprint)** &mdash; info product on career and life reinvention. Cloudflare Pages + Resend sequencing + Workers-based lead capture. Live: [the-reinvention-blueprint.com](https://the-reinvention-blueprint.com).

**[Lean Body Blueprint](https://github.com/kenmwara/lean-body-blueprint)** &mdash; $97 fitness funnel for 9-to-5 workers. Landing page, Stripe checkout, 5-episode video sequence, YouTube remarketing. Live: [theleanbodyblueprint.com](https://theleanbodyblueprint.com).

<a href="https://canadianprmastery.com"><img src="https://tbot.trade/portfolio/img/cpr.jpg" width="200" alt="Canadian PR Mastery — episode 1 opener"></a>&nbsp;<a href="https://the-reinvention-blueprint.com"><img src="https://tbot.trade/portfolio/img/reinvention.jpg" width="200" alt="The Reinvention Blueprint — landing page"></a>&nbsp;<a href="https://theleanbodyblueprint.com"><img src="https://tbot.trade/portfolio/img/lbb.jpg" width="200" alt="Lean Body Blueprint — the 3-rule system landing page"></a>

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
