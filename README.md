<!-- Goes at github.com/kenmwara/kenmwara/README.md — source of truth: github-showcase/PROFILE_README.md (fetch the live file before editing; ship via SHIP.md Step 3).
     Screenshots are served from tbot.trade/portfolio/img/* (tbot-platform dashboard/portfolio-img/) and the public jobscout-app repo. -->

### Hi, I'm Ken 👋

I build and secure systems that have to hold up at 3 AM, when nobody is watching. I'm a Cybersecurity Engineer (Intern) with LOG(N) Pacific's Cyber Range: threat hunting with KQL in Microsoft Defender and Sentinel, Windows hardening against DISA STIGs, Tenable vulnerability management, and an on-prem Active Directory domain of my own. The same habits guard the live-money trading system I run, out of Vancouver, BC.

The repos below are write-ups: what I found, how I found it, and the evidence, plus the architecture of the systems I run (without strategy logic or customer data). The full portfolio is at [tbot.trade/portfolio](https://tbot.trade/portfolio).

---

### 🧭 Start here

| Area | Repos |
|---|---|
| **Cybersecurity** | [Active Directory Home Lab](https://github.com/kenmwara/active-directory-lab) · [Threat Hunt: Harborlight](https://github.com/kenmwara/threat-hunt-harborlight) · [Threat Hunt: Meridian](https://github.com/kenmwara/threat-hunt-meridian) · [Threat Hunt: Tor](https://github.com/kenmwara/threat-hunt-tor) · [Vulnerability Management Program](https://github.com/kenmwara/vulnerability-management-program) · [Windows 11 STIG Remediation](https://github.com/kenmwara/windows-11-stig-remediation) ([all of them](https://github.com/kenmwara?tab=repositories&q=topic%3Acybersecurity)) |
| **Systems I run** | [T BOT](https://github.com/kenmwara/tbot) · [JobScout](https://github.com/kenmwara/jobscout-app) · [Unified Ops Dashboard](https://github.com/kenmwara/unified-ops-dashboard) · [T BOT Security Operations](https://github.com/kenmwara/tbot-security) · [tbot-client](https://github.com/kenmwara/tbot-client) |

---

### 🔐 Cybersecurity projects

Hands-on security work: an on-prem Active Directory domain of my own, and the LOG(N) Pacific Cyber Range on Azure lab machines with Microsoft Defender for Endpoint, Microsoft Sentinel, KQL and Tenable.

**Identity and Active Directory**

<a href="https://github.com/kenmwara/active-directory-lab"><img src="https://raw.githubusercontent.com/kenmwara/active-directory-lab/main/images/readme-hero.png" width="720" alt="The rules in Group Policy Management; a Finance user gets the F: drive and an HR user does not; gpresult for the HR user shows Finance Drive Map, Filtering: Denied (Security)"></a>

- **[Active Directory Home Lab](https://github.com/kenmwara/active-directory-lab)** &mdash; an on-prem domain on my own laptop with Hyper-V: a Windows Server 2025 domain controller (AD DS, DNS, DHCP, NAT), a domain-joined Windows 11 client, 999 users in department OUs, and five Group Policies, each proven on the client: lockout and password policy, Windows LAPS, a USB storage block, a Finance-only drive map and logon auditing. Includes the drive map that failed without a single error, and the security filtering that fixed it.

**Vulnerability management**
- **[Vulnerability Management Program](https://github.com/kenmwara/vulnerability-management-program)** &mdash; one full cycle on a Windows Server 2025 lab: a written policy, a credentialed Tenable baseline, four PowerShell remediation rounds each verified by rescan, and a documented accepted risk. 20 findings → 2 (−90 %).
- **[Windows 11 STIG Remediation](https://github.com/kenmwara/windows-11-stig-remediation)** &mdash; ten DISA Windows 11 STIG findings remediated with PowerShell, each one verified failed → passed by a credentialed Tenable scan.

**Threat hunting and security operations**
- **[Threat Hunt: Harborlight](https://github.com/kenmwara/threat-hunt-harborlight)** &mdash; 46/46 flags, first to finish: a live community hunt on an Akira ransomware intrusion at a dental and insurance practice: a phishing ISO on one workstation, a UAC bypass, LSASS access, the user's own password reused over admin shares to the file server and the domain controller, MEGA exfiltration, and backdoors still beaconing thirteen hours after encryption. Traced in Microsoft Defender with KQL over Sysmon, with seven detection rules tested on the data and the change that closes each gap. 46 of 46 flags, on time.
- **[Threat Hunt: Meridian](https://github.com/kenmwara/threat-hunt-meridian)** &mdash; 16/16 flags, full marks: a live community hunt on a compromised Linux web server: recon, a path-traversal read of the database config, a reused service-account password, and a root backdoor the automated defences flagged but never removed. Traced from raw logs in Azure Log Analytics with KQL, with a timeline, detection gaps and recommendations. 16 of 16 flags, on time.
- **[Threat Hunt: Unauthorized Tor Browser Usage](https://github.com/kenmwara/threat-hunt-tor)** &mdash; generated the activity on a lab VM, then hunted it back out of Defender for Endpoint telemetry with KQL and a Defender investigation package, and wrote it up as an analyst's report.
- **[T BOT Security Operations](https://github.com/kenmwara/tbot-security)** &mdash; the detection and response stack guarding the live trading system (below): intrusion detection, a SIEM and a SOAR console with playbooks.

---

### 🚀 What I'm operating

**[T BOT](https://github.com/kenmwara/tbot)** &mdash; an autonomous trading platform: one rules-based live strategy, 24/7, behind 17 logged risk gates and fifteen codified disciplines. Every lane is billed for its own exchange fees and Claude spend, and goes live only when its record earns it; forex, equities, crypto and macro integrations are built into the same engine. The books are rebuilt every night from the exchange's own records and must close to its reported cash within $5. Copy-trade subscriber pilot with Stripe billing. Rebuilt from git + the secrets vault to live trading in one evening after a total server loss (Sept 2026). Live demo: [tbot.trade/demo](https://tbot.trade/demo).

<a href="https://tbot.trade/demo"><img src="https://tbot.trade/portfolio/img/tbot-demo-card.png?v=2" width="300" alt="tbot.trade/demo: the real T BOT operator dashboard on synthetic data"></a>&nbsp;&nbsp;<a href="https://tbot.trade/demo"><img src="https://tbot.trade/portfolio/img/tbot-demo.jpg?v=20260926d" width="300" alt="T BOT Emergency controls: every lane with Go live or To paper and Restart and review; every action asks first"></a>

**[JobScout](https://github.com/kenmwara/jobscout-app)** &mdash; AI job-search copilot, shipped as a product. Public demo at [jobscout.page](https://jobscout.page): the pipeline's real daily sweep scored live by Claude with the reasoning shown, the deterministic gate verdicts underneath as receipts — behind a per-visitor rate limit and a daily budget breaker that degrades honestly instead of pretending. It carries **its own design system**: the mark is a bearing rose, and a posting's fit lights its eight bearings. The same guarded API has **fully native** Android (Kotlin · Jetpack Compose) and iOS (Swift · SwiftUI) clients that draw that rose from identical geometry — both green in Codemagic CI, both auto-built on push. The private pipeline behind it sweeps ~1,800 postings a day and applies to jobs as me — a human clicks every Submit. September 2026: a **resume helper** whose every line must trace to the candidate's own profile, a signed Android build in Google Play's closed test, and a second market — [nairobi.jobscout.page](https://nairobi.jobscout.page), the same sweep re-gated for a hire based in Kenya, with the question most "remote" postings dodge answered first.

<a href="https://jobscout.page"><img src="https://tbot.trade/portfolio/img/jobscout-canada.jpg" width="300" alt="jobscout.page — “Find the work made for you.”: type a job title or attach a résumé, then pick remote, hybrid or on site"></a>&nbsp;&nbsp;<a href="https://nairobi.jobscout.page/#browse"><img src="https://tbot.trade/portfolio/img/jobscout-kenya.jpg" width="300" alt="nairobi.jobscout.page — “Browse by what the feed actually knows”: today’s Kenya sweep of 357 postings, split by sector"></a>&nbsp;&nbsp;<a href="https://github.com/kenmwara/jobscout-app"><img src="https://raw.githubusercontent.com/kenmwara/jobscout-app/main/docs/img/native/android-02-scoring.jpg" width="110" alt="JobScout on Android — live scoring: the bearing rose lit to each fit"></a>

**[T BOT Web Studio](https://studio.tbot.trade)** &mdash; a web studio with its own front door at [studio.tbot.trade](https://studio.tbot.trade): a live canvas point-cloud, a numbers section that states the studio's actual record rather than adjectives, and a commission flow. Client sites are designed in Chat and shipped by Code on Cloudflare Pages — fixed-price builds plus a recurring care plan. Latest: [Sacred Earth](https://sacred-earth.pages.dev), a Uganda travel brand's field-guide site — a scroll-driven descent down Uganda over a canvas point-cloud of the country, eight stations from Wagagai at 4,321 m to the Nile, each pinned and figure-led as you fall through it. Self-hosted fonts, every ship link-checked and console-clean before it goes live.

<a href="https://studio.tbot.trade"><img src="https://tbot.trade/portfolio/img/studio.jpg" width="330" alt="T BOT Studio — “A different approach to the web” beside a drifting point-cloud rendered live on canvas"></a>&nbsp;&nbsp;<a href="https://sacred-earth.pages.dev"><img src="https://tbot.trade/portfolio/img/sacred-earth.jpg" width="330" alt="Sacred Earth — the Descent: walked down from 4,321 metres, over a canvas point-cloud of Uganda"></a>

**S-Ryder** &mdash; the operating app for a one-bike delivery business in Nairobi, running its real deliveries. One Cloudflare Worker and D1 behind an installable web app, with four views behind two PINs (the rider’s opens only the rider screen): the dispatcher books a job and gets a tracking link, the rider starts a shift and closes each delivery with a proof-of-delivery photo, Fleet shows where the bike is and when it is due a service, and Money gives the week's numbers and each client's statement. The client opens the link with no login and watches the delivery on a map, updated every minute. The rider's phone reports only while a shift is on, and a delivery taken with no signal is kept and sent once. Thirteen checks run on every push. They cover the business end to end, what a rider PIN can and cannot open, tap targets and offline delivery, and a claims check that fails if the app states something it has not measured. *(Screenshots: sample data, not real clients.)*

<img src="https://tbot.trade/portfolio/img/s-ryder-client.jpg" width="170" alt="S-Ryder client link — “On the way”: booked, picked up at 14:12, the rider’s route across Nairobi to Karen on a map">&nbsp;&nbsp;<img src="https://tbot.trade/portfolio/img/s-ryder-rider.jpg" width="170" alt="S-Ryder rider view — start shift, then each delivery closed with “Delivered · photo”">&nbsp;&nbsp;<img src="https://tbot.trade/portfolio/img/s-ryder-fleet.jpg" width="330" alt="S-Ryder Fleet — where the bike is now, today’s movement, and odometer, service and insurance position">

**[Unified Ops Dashboard](https://github.com/kenmwara/unified-ops-dashboard)** &mdash; one dashboard, every product, single Cloudflare-native data plane. D1 + Workers + Pages + Email Routing wired into an append-only event store, behind Cloudflare Access. The platform every other product reports into.

<a href="https://github.com/kenmwara/unified-ops-dashboard"><img src="https://tbot.trade/portfolio/img/ops.jpg" width="440" alt="ops.tbot.trade — fleet health pills, flags, scheduler queue, one tile per product, per-project System health cards"></a>

**[T BOT Security Operations](https://github.com/kenmwara/tbot-security)** &mdash; intrusion detection, a SIEM on the same event store, and a SOAR console with response playbooks, guarding the live-money trading system. It catches a misused exchange key by reconciling the exchange's own fills against the bot's log, and a nightly red team from GitHub Actions attacks the system from outside with a mutation-tested harness, so a check that cannot fail never counts as a pass.

<a href="https://github.com/kenmwara/tbot-security"><img src="https://raw.githubusercontent.com/kenmwara/tbot-security/main/docs/soar-map.png" width="440" alt="SOAR attack map: 24 hours of traffic the server refused, by country, with the SSH, firewall, web and fail2ban split and the top network per country (real counts, no addresses)"></a>&nbsp;&nbsp;<a href="https://github.com/kenmwara/tbot-security"><img src="https://raw.githubusercontent.com/kenmwara/tbot-security/main/docs/soar-incidents.png" width="330" alt="SOAR Incidents — detections grouped by family, day and source IP, each worked from open to resolved with a note"></a>

**[tbot-client](https://github.com/kenmwara/tbot-client)** &mdash; open-source Python client that runs on subscriber machines and places orders against the subscriber's own broker (the original signal-feed model; the live pilot now runs a server-side copy-trade engine with encrypted per-subscriber API keys).

---

### 🛠 What I work with

| Domain | Tools |
|---|---|
| **Security** | Microsoft Defender for Endpoint, Microsoft Sentinel, KQL, Sysmon, Tenable, DISA STIGs, PowerShell, Active Directory + Group Policy, Wireshark, Nmap |
| **Languages** | Python, TypeScript/JavaScript, Kotlin, Swift, Bash, SQL |
| **Web** | FastAPI, Node, Cloudflare Workers, vanilla HTML/CSS/JS where the framework would be overkill |
| **Mobile** | Kotlin + Jetpack Compose, Swift + SwiftUI, Capacitor, Codemagic CI |
| **Cloud / Infra** | Cloudflare (Workers, Pages, D1, R2, KV, Email Routing, Access, Cache Rules, DNS), DigitalOcean, systemd, PM2 |
| **AI / LLMs** | Anthropic Claude, OpenAI, Google Gemini, DeepSeek |
| **Brokers / Markets** | Prediction-market exchange API, OANDA v20, Interactive Brokers (ibeam) |
| **Payments / Email** | Stripe Payment Links, Whop, Resend, Cloudflare Email Routing |
| **Data** | Cloudflare D1 (SQLite at the edge), append-only JSONL with fcntl locks, no heavy ORM dependencies |

---

### 🎓 Credentials

- **[HarvardX Professional Certificate in Computer Science for Cybersecurity](https://credentials.edx.org/credentials/89cc10e390654c709f8e9d902fffe419/)** (2026): CS50x + CS50's Introduction to Cybersecurity
- **[CS50's Introduction to Cybersecurity](https://cs50.harvard.edu/certificates/02ad8b9a-e117-4d13-98c0-1a7f2d028974)**, Harvard CS50 certificate (2026, five assignments and a final project)
- **[HarvardX Professional Certificate in Computer Science for Artificial Intelligence](https://credentials.edx.org/credentials/c9bb24239a3044629308c0dde14aa3ca/)** (2026): CS50x + CS50 AI
- **[CS50's Introduction to Artificial Intelligence with Python](https://cs50.harvard.edu/certificates/8c4ed10c-bec1-4bc1-bea1-a611b22489a0)**, Harvard CS50 certificate (2026, twelve projects)
- **[Ethical Hacking Certification Training](https://www.credential.net/718b441f-b5a6-4c99-8582-d68bd00dba11)**, UBC Extended Learning, University of British Columbia (2025, verified digital credential)
- **B.S. Cybersecurity and Information Assurance**, Western Governors University: enrolled; starting January 2027, expected completion December 2027

### 📍 Operating principles

- **Surface isolation as primary architecture.** A failure on one system never cascades: a trading lane going down can't touch the job-search product or the ops dashboard.
- **Append-only audit logs beat mutable state.** Forward-only debuggability wins over database snapshots almost every time. D1 + JSONL covers more ground than people assume.
- **Cloudflare-native by default.** One vendor for DNS, edge, Workers, D1, R2, Pages, email routing, access control. Operational simplicity at portfolio scale beats best-of-breed sprawl.
- **Numbers are labeled, never fabricated.** Measured from logs, modeled from stated assumptions, or absent — every public figure says which. The [T BOT demo page](https://tbot.trade/demo) publishes the actual gating chain and signal pipeline; opacity in a trading product is a red flag, not a feature.
- **Ship the smallest thing that works, then watch it for a week before adding the next thing.**

---

### 📫 Connect

[LinkedIn](https://linkedin.com/in/kenmwara) &nbsp;·&nbsp; [X](https://x.com/Ken_Mwara) &nbsp;·&nbsp; [Portfolio](https://tbot.trade/portfolio) &nbsp;·&nbsp; Vancouver, BC

Open to interesting conversations — algo trading, LLM orchestration in production, native + edge app architecture, or what it takes to trust a system you are not watching.
