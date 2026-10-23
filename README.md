<!-- Goes at github.com/kenmwara/kenmwara/README.md — source of truth: github-showcase/PROFILE_README.md (fetch the live file before editing).
     The card blocks are GENERATED: edit brand/cards.json, run brand/render.py then brand/build_readme.py, and copy brand/out/*.png
     to kenmwara/kenmwara/assets/brand/. Everything outside the BEGIN/END markers is hand-written. -->

<!-- BEGIN hero -->
<img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/hero.png?v=3bafdf5d" width="100%" alt="Ken Kariuki. Security operations, Vancouver, BC: threat hunting, Active Directory, detection engineering. Cybersecurity Engineer (Intern) at LOG(N) Pacific; HarvardX CS for Cybersecurity; WGU B.S. Cybersecurity starts January 2027.">
<!-- END hero -->

<p align="center"><i>Threat hunting with KQL in Microsoft Defender and Sentinel, an Active Directory domain of my own,<br>and the security operations guarding a live-money trading system.</i></p>

<p align="center">
  <img src="https://img.shields.io/badge/Cyber_Range-Cybersecurity_Engineer_(Intern)-C8102E?style=flat-square&labelColor=14202e" alt="Cyber Range: Cybersecurity Engineer (Intern)">
  <img src="https://img.shields.io/badge/WGU-B.S._Cybersecurity_%C2%B7_starts_Jan_2027-1f6f8b?style=flat-square&labelColor=14202e" alt="WGU B.S. Cybersecurity, starts January 2027">
</p>

### Hi, I'm Ken 👋

I build and secure systems that have to hold up at 3 AM, when nobody is watching. I'm a Cybersecurity Engineer (Intern) with LOG(N) Pacific's Cyber Range: threat hunting with KQL in Microsoft Defender and Sentinel, Windows hardening against DISA STIGs, Tenable vulnerability management, and an on-prem Active Directory domain of my own. The same habits guard the live-money trading system I run, out of Vancouver, BC.

Every project below is a write-up: what I found, how I found it, and the evidence. Each card wears a Maasai shuka, and the colour of the cloth says what kind of work it is: **blue** for identity, **red** for threat hunting and detection, **orange** for hardening, **purple** for the systems I run.

---

### 🔐 Security projects

**Identity and Active Directory**

<!-- BEGIN cards:identity -->
<a href="https://github.com/kenmwara/active-directory-lab"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/card-ad-lab.png?v=38db5fc6" width="100%" alt="Active Directory Lab: A Windows Server 2025 domain controller and a domain-joined Windows 11 client on Hyper-V, with five Group Policies proven on the client. 999 users in the domain."></a>

<img src="https://img.shields.io/badge/Windows_Server_2025-1f4ea6?style=flat-square" alt="Windows Server 2025"> <img src="https://img.shields.io/badge/AD_DS_%C2%B7_DNS_%C2%B7_DHCP-1f4ea6?style=flat-square" alt="AD DS · DNS · DHCP"> <img src="https://img.shields.io/badge/Group_Policy-1f4ea6?style=flat-square" alt="Group Policy"> <img src="https://img.shields.io/badge/Windows_LAPS-1f4ea6?style=flat-square" alt="Windows LAPS"> <img src="https://img.shields.io/badge/PowerShell-1f4ea6?style=flat-square" alt="PowerShell">

An on-prem domain on my own laptop: a domain controller running AD DS, DNS, DHCP and NAT, a Windows 11 client joined to it, 999 users in department OUs, and five Group Policies, each one proven on the client (lockout and password rules, Windows LAPS, a USB storage block, a Finance-only drive map and logon auditing). Includes the drive map that failed without a single error, and the security filtering that fixed it. [Read it →](https://github.com/kenmwara/active-directory-lab)
<!-- END cards:identity -->

**Threat hunting and detection**

<!-- BEGIN cards:hunt -->
<a href="https://github.com/kenmwara/threat-hunt-harborlight"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/card-harborlight.png?v=4a116bc4" width="100%" alt="Harborlight: Akira ransomware at a dental practice, traced from a phishing ISO to the domain controller. 46/46 flags · first to finish."></a>

<img src="https://img.shields.io/badge/Akira_ransomware-C8102E?style=flat-square" alt="Akira ransomware"> <img src="https://img.shields.io/badge/KQL-C8102E?style=flat-square" alt="KQL"> <img src="https://img.shields.io/badge/Sysmon-C8102E?style=flat-square" alt="Sysmon"> <img src="https://img.shields.io/badge/Microsoft_Defender-C8102E?style=flat-square" alt="Microsoft Defender"> <img src="https://img.shields.io/badge/7_detection_rules_tested-C8102E?style=flat-square" alt="7 detection rules tested">

A live community hunt on an Akira ransomware intrusion at a dental and insurance practice: a phishing ISO on one workstation, a UAC bypass, LSASS access, the user's own password reused over admin shares to the file server and the domain controller, MEGA exfiltration, and backdoors still beaconing thirteen hours after encryption. Traced in Microsoft Defender with KQL over Sysmon, with seven detection rules tested on the data and the change that closes each gap. [Read it →](https://github.com/kenmwara/threat-hunt-harborlight)

<a href="https://github.com/kenmwara/threat-hunt-meridian"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/card-meridian.png?v=b804f706" width="100%" alt="Meridian: A compromised Linux web server: path traversal, a reused service-account password and a root backdoor. 16/16 flags · full marks."></a>

<img src="https://img.shields.io/badge/Linux_%C2%B7_Apache_%C2%B7_PHP-C8102E?style=flat-square" alt="Linux · Apache · PHP"> <img src="https://img.shields.io/badge/KQL-C8102E?style=flat-square" alt="KQL"> <img src="https://img.shields.io/badge/Azure_Log_Analytics-C8102E?style=flat-square" alt="Azure Log Analytics"> <img src="https://img.shields.io/badge/Path_traversal-C8102E?style=flat-square" alt="Path traversal"> <img src="https://img.shields.io/badge/SUID_backdoor-C8102E?style=flat-square" alt="SUID backdoor">

A live community hunt on a compromised Linux web server: four recon tools, a path-traversal read of the database config, a reused service-account password over SSH, and a root backdoor the automated defences flagged but never removed. Traced from raw web, auth and audit logs in Azure Log Analytics with KQL, with a timeline, detection gaps and recommendations. 1,675 / 1,675, on time. [Read it →](https://github.com/kenmwara/threat-hunt-meridian)

<a href="https://github.com/kenmwara/threat-hunt-tor"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/card-tor.png?v=0a303113" width="100%" alt="Unauthorized Tor: A portable Tor Browser on a lab endpoint, hunted back out of Defender telemetry and an investigation package. 3 Tor relays traced on 443."></a>

<img src="https://img.shields.io/badge/Defender_for_Endpoint-C8102E?style=flat-square" alt="Defender for Endpoint"> <img src="https://img.shields.io/badge/KQL-C8102E?style=flat-square" alt="KQL"> <img src="https://img.shields.io/badge/Investigation_package-C8102E?style=flat-square" alt="Investigation package"> <img src="https://img.shields.io/badge/MITRE_ATT%26CK-C8102E?style=flat-square" alt="MITRE ATT&CK">

I generated the activity on my own lab VM, then hunted it back out of Microsoft Defender for Endpoint with KQL and a Defender investigation package: the download, the portable install, and a Tor circuit through three relays on port 443. Written up as an analyst's report, with the detection gaps it exposed (port rules, software inventory and DNS logs all miss portable Tor). [Read it →](https://github.com/kenmwara/threat-hunt-tor)

<a href="https://github.com/kenmwara/tbot-security"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/card-tbot-security.png?v=162c3a50" width="100%" alt="T BOT Security Ops: Intrusion detection, a SIEM and a SOAR console with playbooks, guarding a live-money trading system. LIVE guarding production."></a>

<img src="https://img.shields.io/badge/SIEM-C8102E?style=flat-square" alt="SIEM"> <img src="https://img.shields.io/badge/SOAR_playbooks-C8102E?style=flat-square" alt="SOAR playbooks"> <img src="https://img.shields.io/badge/fail2ban_%C2%B7_UFW-C8102E?style=flat-square" alt="fail2ban · UFW"> <img src="https://img.shields.io/badge/Cloudflare_Workers-C8102E?style=flat-square" alt="Cloudflare Workers"> <img src="https://img.shields.io/badge/Nightly_red_team-C8102E?style=flat-square" alt="Nightly red team">

The detection and response stack guarding the live trading system below: intrusion detection, a SIEM on the same event store, and a SOAR console where incidents are worked from open to resolved. It catches a misused exchange key by reconciling the exchange's own fills against the bot's log, and a nightly red team from GitHub Actions attacks the system from outside with a mutation-tested harness, so a check that cannot fail never counts as a pass. [Read it →](https://github.com/kenmwara/tbot-security)
<!-- END cards:hunt -->

**Vulnerability management and hardening**

<!-- BEGIN cards:harden -->
<a href="https://github.com/kenmwara/vulnerability-management-program"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/card-vm-program.png?v=315afb3a" width="100%" alt="Vulnerability Management: A written policy, a credentialed baseline and four remediation rounds on a Windows Server 2025 lab, each verified by rescan. −90% 20 findings → 2."></a>

<img src="https://img.shields.io/badge/Tenable-d9581a?style=flat-square" alt="Tenable"> <img src="https://img.shields.io/badge/Credentialed_scans-d9581a?style=flat-square" alt="Credentialed scans"> <img src="https://img.shields.io/badge/PowerShell-d9581a?style=flat-square" alt="PowerShell"> <img src="https://img.shields.io/badge/Windows_Server_2025-d9581a?style=flat-square" alt="Windows Server 2025"> <img src="https://img.shields.io/badge/Accepted_risk-d9581a?style=flat-square" alt="Accepted risk">

One full cycle of a vulnerability management program, from no policy to a remediated server: a written policy, a credentialed Tenable baseline, four PowerShell remediation rounds each verified by rescan, and a documented accepted risk for what was left. Critical 2 → 0, High 2 → 0. [Read it →](https://github.com/kenmwara/vulnerability-management-program)

<a href="https://github.com/kenmwara/windows-11-stig-remediation"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/card-stig.png?v=689843e4" width="100%" alt="Windows 11 STIG: Ten DISA STIG findings on a Windows 11 lab VM, each remediated with PowerShell and verified by a credentialed compliance scan. 10/10 failed → passed."></a>

<img src="https://img.shields.io/badge/DISA_STIG-d9581a?style=flat-square" alt="DISA STIG"> <img src="https://img.shields.io/badge/PowerShell-d9581a?style=flat-square" alt="PowerShell"> <img src="https://img.shields.io/badge/Tenable_compliance_audit-d9581a?style=flat-square" alt="Tenable compliance audit"> <img src="https://img.shields.io/badge/Windows_11_25H2-d9581a?style=flat-square" alt="Windows 11 25H2">

Ten DISA Windows 11 STIG findings (audit policy, event log sizes, SEHOP, the Secondary Logon service and more), each remediated with one PowerShell script and verified failed → passed by a credentialed Tenable compliance scan. [Read it →](https://github.com/kenmwara/windows-11-stig-remediation)
<!-- END cards:harden -->

---

### 🚀 Systems I run

<!-- BEGIN cards:systems -->
<a href="https://github.com/kenmwara/tbot"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/card-tbot.png?v=cd39ed53" width="100%" alt="T BOT: An autonomous trading platform that has to earn every lane it runs, its books reconciled to the exchange every night. 17 logged risk gates."></a>

<img src="https://img.shields.io/badge/Python-6b2d93?style=flat-square" alt="Python"> <img src="https://img.shields.io/badge/Risk_gates-6b2d93?style=flat-square" alt="Risk gates"> <img src="https://img.shields.io/badge/Nightly_reconciliation-6b2d93?style=flat-square" alt="Nightly reconciliation"> <img src="https://img.shields.io/badge/Cloudflare-6b2d93?style=flat-square" alt="Cloudflare"> <img src="https://img.shields.io/badge/DigitalOcean-6b2d93?style=flat-square" alt="DigitalOcean">

One rules-based live strategy, 24/7, behind 17 logged risk gates. Every lane is billed for its own exchange fees and Claude spend and goes live only when its record earns it. The books are rebuilt every night from the exchange's own records and must close to its reported cash within $5. Rebuilt from git and the secrets vault to live trading in one evening after a total server loss (Sept 2026). Live demo: [tbot.trade/demo](https://tbot.trade/demo). [Read it →](https://github.com/kenmwara/tbot)

<a href="https://github.com/kenmwara/jobscout-app"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/card-jobscout.png?v=b67f41eb" width="100%" alt="JobScout: Real postings scored live by Claude with the reasoning shown, and native Android and iOS clients on one guarded API. LIVE jobscout.page."></a>

<img src="https://img.shields.io/badge/Claude-6b2d93?style=flat-square" alt="Claude"> <img src="https://img.shields.io/badge/Kotlin_%C2%B7_Compose-6b2d93?style=flat-square" alt="Kotlin · Compose"> <img src="https://img.shields.io/badge/Swift_%C2%B7_SwiftUI-6b2d93?style=flat-square" alt="Swift · SwiftUI"> <img src="https://img.shields.io/badge/Cloudflare_Workers-6b2d93?style=flat-square" alt="Cloudflare Workers"> <img src="https://img.shields.io/badge/Codemagic_CI-6b2d93?style=flat-square" alt="Codemagic CI">

An AI job-search copilot, shipped as a product. The public demo at [jobscout.page](https://jobscout.page) scores the pipeline's real daily sweep live with Claude and shows the reasoning, with the deterministic gate verdicts underneath as receipts, behind a per-visitor rate limit and a daily budget breaker. A second market at [nairobi.jobscout.page](https://nairobi.jobscout.page) re-gates the same sweep for a hire based in Kenya. [Read it →](https://github.com/kenmwara/jobscout-app)

<a href="https://github.com/kenmwara/unified-ops-dashboard"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/card-ops.png?v=c89c0e06" width="100%" alt="Unified Ops Dashboard: One dashboard every product reports into: an append-only event store on Cloudflare D1, Workers and Pages. LIVE behind Cloudflare Access."></a>

<img src="https://img.shields.io/badge/Cloudflare_D1-6b2d93?style=flat-square" alt="Cloudflare D1"> <img src="https://img.shields.io/badge/Workers-6b2d93?style=flat-square" alt="Workers"> <img src="https://img.shields.io/badge/Pages-6b2d93?style=flat-square" alt="Pages"> <img src="https://img.shields.io/badge/Access-6b2d93?style=flat-square" alt="Access"> <img src="https://img.shields.io/badge/Email_Routing-6b2d93?style=flat-square" alt="Email Routing">

One dashboard, every product, a single Cloudflare-native data plane: D1, Workers, Pages and Email Routing wired into an append-only event store, behind Cloudflare Access. The platform every other product reports into. [Read it →](https://github.com/kenmwara/unified-ops-dashboard)
<!-- END cards:systems -->

**Also running:**
- **[T BOT Web Studio](https://studio.tbot.trade)** &mdash; a web studio for small-business sites: designed in Chat, shipped by Code on Cloudflare Pages, link-checked and console-clean before every ship. Latest: [Sacred Earth](https://sacred-earth.pages.dev), a Uganda travel brand's field-guide site.
- **S-Ryder** &mdash; the operating app for a one-bike delivery business in Nairobi, running its real deliveries: dispatch, a no-login tracking link for the client, proof-of-delivery photos, fleet and money views, on one Cloudflare Worker and D1, with thirteen checks on every push.
- **[tbot-client](https://github.com/kenmwara/tbot-client)** &mdash; open-source Python client from T BOT's original signal-feed model, placing orders against a subscriber's own broker.

The full portfolio is at [tbot.trade/portfolio](https://tbot.trade/portfolio).

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
- **Numbers are labeled, never fabricated.** Measured from logs, modeled from stated assumptions, or absent — every public figure says which. The [T BOT demo page](https://tbot.trade/demo) publishes the actual gating chain; opacity in a trading product is a red flag, not a feature.
- **Ship the smallest thing that works, then watch it for a week before adding the next thing.**

---

### 📫 Connect

[LinkedIn](https://linkedin.com/in/kenmwara) &nbsp;·&nbsp; [X](https://x.com/Ken_Mwara) &nbsp;·&nbsp; [Portfolio](https://tbot.trade/portfolio) &nbsp;·&nbsp; Vancouver, BC

Open to interesting conversations — threat hunting and detection engineering, Active Directory, LLM orchestration in production, or what it takes to trust a system you are not watching.
