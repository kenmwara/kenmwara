<!-- Goes at github.com/kenmwara/kenmwara/README.md — source of truth: github-showcase/PROFILE_README.md (fetch the live file before editing; ship via SHIP.md Step 3).
     Screenshots are served from tbot.trade/portfolio/img/* (tbot-platform dashboard/portfolio-img/) and the public jobscout-app repo. -->

### Hi, I'm Ken 👋

I build systems that have to hold up at 3 AM, when nobody is watching: a portfolio of products out of Vancouver, BC, plus a small web studio for client sites. I build, ship, and run automated systems end-to-end — strategy, code, Cloudflare infrastructure, native mobile, payments, content, analytics, customer ops.

Most of what I work on makes money rather than stars, so my public footprint is selective. The repos below are showcases — architecture, decisions, and screenshots — without the moats (strategy logic, conversion copy, customer lists). Every live product is linked and pictured; the full portfolio page is at [tbot.trade/portfolio](https://tbot.trade/portfolio).

---

### 🚀 What I'm operating

**[T BOT](https://github.com/kenmwara/tbot)** &mdash; autonomous trading on Kalshi prediction markets, live 24/7 on weather contracts behind a 14-layer guard chain with fifteen codified disciplines. Every lane is billed for its own exchange fees and Claude spend and recalibrated when it does not pay: a Claude prediction lane and four other surfaces (forex, macro, equities, crypto) were retired on the evidence and stay on the dashboard for scrutiny. The books are rebuilt every night from the exchange's own records and must close to its reported cash within $5. Copy-trade subscriber pilot with Stripe billing. Rebuilt from git + the secrets vault to live trading in one evening after a total server loss (Sept 2026). Live demo: [tbot.trade/demo](https://tbot.trade/demo).

<a href="https://tbot.trade/portfolio"><img src="https://tbot.trade/portfolio/img/tbot-dash.jpg?v=20260926" width="300" alt="T BOT surface roster: ST weather live on Kalshi; LT, STK, CRYPTO, FX and the Claude lane retired on evidence"></a>&nbsp;&nbsp;<a href="https://tbot.trade/demo"><img src="https://tbot.trade/portfolio/img/tbot-demo.jpg?v=20260926" width="300" alt="tbot.trade/demo — trading signals delivered to your phone: one live Kalshi weather surface, 15% on realized profit only, $0 custody"></a>

**[JobScout](https://github.com/kenmwara/jobscout-app)** &mdash; AI job-search copilot, shipped as a product. Public demo at [jobscout.page](https://jobscout.page): the pipeline's real daily sweep scored live by Claude with the reasoning shown, the deterministic gate verdicts underneath as receipts — behind a per-visitor rate limit and a daily budget breaker that degrades honestly instead of pretending. It carries **its own design system**: the mark is a bearing rose, and a posting's fit lights its eight bearings. The same guarded API has **fully native** Android (Kotlin · Jetpack Compose) and iOS (Swift · SwiftUI) clients that draw that rose from identical geometry — both green in Codemagic CI, both auto-built on push. The private pipeline behind it sweeps ~1,800 postings a day and applies to jobs as me — a human clicks every Submit. September 2026: a **resume helper** whose every line must trace to the candidate's own profile, a signed Android build in Google Play's closed test, and a second market — [nairobi.jobscout.page](https://nairobi.jobscout.page), the same sweep re-gated for a hire based in Kenya, with the question most "remote" postings dodge answered first.

<a href="https://jobscout.page"><img src="https://tbot.trade/portfolio/img/jobscout-canada.jpg" width="300" alt="jobscout.page — “Find the work made for you.”: type a job title or attach a résumé, then pick remote, hybrid or on site"></a>&nbsp;&nbsp;<a href="https://nairobi.jobscout.page/#browse"><img src="https://tbot.trade/portfolio/img/jobscout-kenya.jpg" width="300" alt="nairobi.jobscout.page — “Browse by what the feed actually knows”: today’s Kenya sweep of 357 postings, split by sector"></a>&nbsp;&nbsp;<a href="https://github.com/kenmwara/jobscout-app"><img src="https://raw.githubusercontent.com/kenmwara/jobscout-app/main/docs/img/native/android-02-scoring.jpg" width="110" alt="JobScout on Android — live scoring: the bearing rose lit to each fit"></a>

**[T BOT Web Studio](https://studio.tbot.trade)** &mdash; a web studio with its own front door at [studio.tbot.trade](https://studio.tbot.trade): a live canvas point-cloud, a numbers section that states the studio's actual record rather than adjectives, and a commission flow. Client sites are designed in Chat and shipped by Code on Cloudflare Pages — fixed-price builds plus a recurring care plan. Latest: [Sacred Earth](https://sacred-earth.pages.dev), a Uganda travel brand's field-guide site — a scroll-driven descent down Uganda over a canvas point-cloud of the country, eight stations from Wagagai at 4,321 m to the Nile, each pinned and figure-led as you fall through it. Self-hosted fonts, every ship link-checked and console-clean before it goes live.

<a href="https://studio.tbot.trade"><img src="https://tbot.trade/portfolio/img/studio.jpg" width="330" alt="T BOT Studio — “A different approach to the web” beside a drifting point-cloud rendered live on canvas"></a>&nbsp;&nbsp;<a href="https://sacred-earth.pages.dev"><img src="https://tbot.trade/portfolio/img/sacred-earth.jpg" width="330" alt="Sacred Earth — the Descent: walked down from 4,321 metres, over a canvas point-cloud of Uganda"></a>

**S-Ryder** &mdash; the operating app for a one-bike delivery business in Nairobi, running its real deliveries. One Cloudflare Worker and D1 behind an installable web app, with four views behind two PINs (the rider’s opens only the rider screen): the dispatcher books a job and gets a tracking link, the rider starts a shift and closes each delivery with a proof-of-delivery photo, Fleet shows where the bike is and when it is due a service, and Money gives the week's numbers and each client's statement. The client opens the link with no login and watches the delivery on a map, updated every minute. The rider's phone reports only while a shift is on, and a delivery taken with no signal is kept and sent once. Thirteen checks run on every push. They cover the business end to end, what a rider PIN can and cannot open, tap targets and offline delivery, and a claims check that fails if the app states something it has not measured. *(Screenshots: sample data, not real clients.)*

<img src="https://tbot.trade/portfolio/img/s-ryder-client.jpg" width="170" alt="S-Ryder client link — “On the way”: booked, picked up at 14:12, the rider’s route across Nairobi to Karen on a map">&nbsp;&nbsp;<img src="https://tbot.trade/portfolio/img/s-ryder-rider.jpg" width="170" alt="S-Ryder rider view — start shift, then each delivery closed with “Delivered · photo”">&nbsp;&nbsp;<img src="https://tbot.trade/portfolio/img/s-ryder-fleet.jpg" width="330" alt="S-Ryder Fleet — where the bike is now, today’s movement, and odometer, service and insurance position">

**[Unified Ops Dashboard](https://github.com/kenmwara/unified-ops-dashboard)** &mdash; one dashboard, every product, single Cloudflare-native data plane. D1 + Workers + Pages + Email Routing wired into an append-only event store, behind Cloudflare Access. The platform every other product reports into.

<a href="https://github.com/kenmwara/unified-ops-dashboard"><img src="https://tbot.trade/portfolio/img/ops.jpg" width="440" alt="ops.tbot.trade — fleet health pills, flags, scheduler queue, one tile per product, per-project System health cards"></a>

**[T BOT Security Operations](https://github.com/kenmwara/tbot-security)** &mdash; intrusion detection, a SIEM on the same event store, and a SOAR console with response playbooks, guarding the live-money trading system. It catches a misused exchange key by reconciling the exchange's own fills against the bot's log, and a nightly red team from GitHub Actions attacks the system from outside with a mutation-tested harness, so a check that cannot fail never counts as a pass.

<a href="https://github.com/kenmwara/tbot-security"><img src="https://raw.githubusercontent.com/kenmwara/tbot-security/main/docs/soar-incidents.png" width="330" alt="SOAR Incidents — detections grouped by family, day and source IP, each worked from open to resolved with a note"></a>&nbsp;&nbsp;<a href="https://github.com/kenmwara/tbot-security"><img src="https://raw.githubusercontent.com/kenmwara/tbot-security/main/docs/soar-live.png" width="330" alt="SIEM Live logs — SSH, firewall, fail2ban and web security events streaming in as they happen, with source IP and country"></a>

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

Open to interesting conversations — algo trading, LLM orchestration in production, native + edge app architecture, or what it takes to trust a system you are not watching.
