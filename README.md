<!-- Goes at github.com/kenmwara/kenmwara/README.md — source of truth: github-showcase/PROFILE_README.md (fetch the live file before editing).
     GENERATED blocks: edit brand/cards.json or brand/sections.json, run brand/render.py then brand/build_readme.py, and copy
     brand/out/*.png to kenmwara/kenmwara/assets/brand/. Everything outside the BEGIN/END markers is hand-written.
     House style (Ken, 23 Oct 2026): a fast glimpse must say exactly what I do. Clear, direct, highlighted, a pop of colour;
     details live behind the "→" links, never on the profile. -->

<!-- BEGIN hero -->
<a href="https://linkedin.com/in/kenmwara"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/hero.png?v=66394861f7" width="100%" alt="Ken Kariuki. Security operations, Vancouver, BC: threat hunting, Active Directory, detection engineering."></a>
<!-- END hero -->

<p align="center"><b>Cybersecurity Engineer (Intern) at LOG(N) Pacific's Cyber Range · Vancouver, BC</b><br>
I trace attacks through security logs, lock down the systems that control who can log in, and keep live systems running at 3 AM, when nobody is watching.</p>

<p align="center">
  <a href="https://github.com/kenmwara/kenmwara#ai"><img src="https://img.shields.io/badge/AI_agent_security-1f6f8b?style=for-the-badge" alt="AI agent security"></a> <b>→</b>
  <a href="https://github.com/kenmwara/kenmwara#hunt"><img src="https://img.shields.io/badge/Threat_hunts-A8323D?style=for-the-badge" alt="Threat hunts"></a> <b>→</b>
  <a href="https://github.com/kenmwara/kenmwara#identity"><img src="https://img.shields.io/badge/Identity_%26_AD-2F4C80?style=for-the-badge" alt="Identity and Active Directory"></a> <b>→</b>
  <a href="https://github.com/kenmwara/kenmwara#harden"><img src="https://img.shields.io/badge/Hardening-B4623C?style=for-the-badge" alt="Hardening and fixing weaknesses"></a> <b>→</b>
  <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/Systems_I_run-5D3D79?style=for-the-badge" alt="Systems I run"></a>
</p>

<p align="center"><sub>One path through the work: secure the AI, hunt what gets in, build and harden what it targets, then run it live. Every project name opens its full report.</sub></p>

<!-- BEGIN section:ai -->
<a name="ai"></a><a href="https://github.com/kenmwara/kenmwara#ai"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/section-ai.png?v=2a84efce3e" width="100%" alt="AI agent security"></a>

<sub>Start here. AI helpers now get real access to company systems, so each test asks what stops one when someone tries to trick it.</sub>

| Project | What it is | Result |
|---|---|---|
| **[Securing an AI Agent in AD](https://github.com/kenmwara/securing-ai-agents-ad)**<br><sub>Prompt injection · Claude Code · Active Directory · OWASP AI risks</sub> | An AI helpdesk assistant allowed to manage user accounts, tested 13 ways to see what stops it when someone tries to trick it | 13 attack tests · hidden commands never fooled it · one gap open, fix in progress · [Read the assessment →](https://github.com/kenmwara/securing-ai-agents-ad) |
| **[Echo Leaks](https://github.com/kenmwara/threat-hunt-echo-leaks)**<br><sub>Prompt injection · Microsoft 365 Copilot · KQL · Entra ID</sub> | Hidden instructions in a Word file made Microsoft 365 Copilot read 13 confidential files and try to send them out | All 17 questions answered · a perfect 1,600, on time · [Read the report →](https://github.com/kenmwara/threat-hunt-echo-leaks) |
<!-- END section:ai -->

<!-- BEGIN section:hunt -->
<a name="hunt"></a><a href="https://github.com/kenmwara/kenmwara#hunt"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/section-hunt.png?v=a588a0f858" width="100%" alt="Threat hunts"></a>

<sub>Each hunt traces an attack through Microsoft's security logs, from the first sign to the last move, and ends with a written incident report. <a href="https://github.com/kenmwara/threat-hunts">All four on one page →</a></sub>

| Project | What it is | Result |
|---|---|---|
| **[Harborlight](https://github.com/kenmwara/threat-hunt-harborlight)**<br><sub>Ransomware · KQL · Sysmon · Microsoft Defender</sub> | Akira ransomware at a dental practice, traced from one phishing download to the server that controls every login | All 46 questions answered · 4,060 of 4,190 points, on time · [Read the report →](https://github.com/kenmwara/threat-hunt-harborlight) |
| **[Echo Leaks](https://github.com/kenmwara/threat-hunt-echo-leaks)**<br><sub>Prompt injection · Microsoft 365 Copilot · KQL · Entra ID</sub> | Hidden instructions in a Word file made Microsoft 365 Copilot read 13 confidential files and try to send them out | All 17 questions answered · a perfect 1,600, on time · [Read the report →](https://github.com/kenmwara/threat-hunt-echo-leaks) |
| **[Meridian](https://github.com/kenmwara/threat-hunt-meridian)**<br><sub>Linux · Apache · PHP · KQL · Azure Log Analytics · Incident report</sub> | A hacked Linux web server: a website flaw leaked a password, the attacker took full control, and a backdoor was still running at the end | All 16 questions answered · full marks, on time · [Read the report →](https://github.com/kenmwara/threat-hunt-meridian) |
| **[Unauthorized Tor](https://github.com/kenmwara/threat-hunt-tor)**<br><sub>Defender for Endpoint · KQL · Evidence package · MITRE ATT&CK</sub> | Hidden web browsing on a test computer, traced through Microsoft Defender's logs and an evidence package | Tor caught on a test computer · its traffic traced through 3 hiding hops · [Read the report →](https://github.com/kenmwara/threat-hunt-tor) |

<p><a href="https://github.com/kenmwara/threat-hunt-harborlight"><img src="https://raw.githubusercontent.com/kenmwara/threat-hunt-harborlight/main/images/scorecard.png" width="49%" alt="threat-hunt-harborlight key takeaways"></a> <a href="https://github.com/kenmwara/threat-hunt-echo-leaks"><img src="https://raw.githubusercontent.com/kenmwara/threat-hunt-echo-leaks/main/images/scorecard.png" width="49%" alt="threat-hunt-echo-leaks key takeaways"></a> <a href="https://github.com/kenmwara/threat-hunt-meridian"><img src="https://raw.githubusercontent.com/kenmwara/threat-hunt-meridian/main/images/scorecard.png" width="49%" alt="threat-hunt-meridian key takeaways"></a> <a href="https://github.com/kenmwara/threat-hunt-tor"><img src="https://raw.githubusercontent.com/kenmwara/threat-hunt-tor/main/images/scorecard.png" width="49%" alt="threat-hunt-tor key takeaways"></a></p>
<!-- END section:hunt -->

<!-- BEGIN section:identity -->
<a name="identity"></a><a href="https://github.com/kenmwara/kenmwara#identity"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/section-identity.png?v=d285923821" width="100%" alt="Identity & Active Directory"></a>

<sub>The systems attackers go after: a company network built from scratch and locked down with company-wide rules.</sub>

| Project | What it is | Result |
|---|---|---|
| **[Active Directory Lab](https://github.com/kenmwara/active-directory-lab)**<br><sub>Windows Server 2025 · Active Directory · Group Policy · Windows LAPS</sub> | A small company network built from scratch: a Windows server managing 999 users, a work PC, and five company rules, each tested | 999 users · five company rules, each tested on the work PC · [See the lab →](https://github.com/kenmwara/active-directory-lab) |
<!-- END section:identity -->

<!-- BEGIN section:harden -->
<a name="harden"></a><a href="https://github.com/kenmwara/kenmwara#harden"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/section-harden.png?v=159587e7b4" width="100%" alt="Hardening & fixing weaknesses"></a>

<sub>Closing the gaps before anyone finds them: every fix proven by a fresh scan.</sub>

| Project | What it is | Result |
|---|---|---|
| **[Vulnerability Management](https://github.com/kenmwara/vulnerability-management-program)**<br><sub>Tenable · Scans with a login · PowerShell · Windows Server 2025</sub> | A Windows server taken from 20 security weaknesses to 2 in four rounds of fixes, each proven by a fresh scan | 20 weaknesses → 2 (−90 %) · nothing critical or high left · [See the work →](https://github.com/kenmwara/vulnerability-management-program) |
| **[Windows 11 STIG](https://github.com/kenmwara/windows-11-stig-remediation)**<br><sub>DISA STIG · PowerShell · Tenable compliance scan · Windows 11</sub> | Ten Windows 11 security settings that failed the US Defense Department's checklist, each fixed with a script and passed on a fresh scan | 10 of 10 settings fixed · failed → passed · [See the work →](https://github.com/kenmwara/windows-11-stig-remediation) |
<!-- END section:harden -->

<!-- BEGIN section:systems -->
<a name="systems"></a><a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/section-systems.png?v=7543386c2c" width="100%" alt="Systems I run"></a>

<sub>The same discipline on live systems: production platforms I run and watch every day.</sub>

| Project | What it is | Result |
|---|---|---|
| **[T BOT](https://github.com/kenmwara/tbot)**<br><sub>Python · Safety checks · Nightly book check · Cloudflare</sub> | A trading robot that trades real money on its own, every trade checked 17 ways, its books matched to the exchange every night | Real money, 24/7 · 17 safety checks on every trade · books matched to the exchange nightly · [See the system →](https://github.com/kenmwara/tbot) |
| **[T BOT Security Ops](https://github.com/kenmwara/tbot-security)**<br><sub>Intrusion detection · Security log (SIEM) · One-click responses · Cloudflare</sub> | The security system that watches a live trading robot overnight: it spots break-in attempts, keeps one record, and responds in seconds | Live · no logins but the owner's since Sep 2026 · attacked by its own test every night · [See the stack →](https://github.com/kenmwara/tbot-security) |
| **[JobScout](https://github.com/kenmwara/jobscout-app)**<br><sub>Claude · Kotlin · Compose · Swift · SwiftUI · Cloudflare Workers</sub> | Real job posts scored by AI against a résumé, with its reasons shown, on the web, Android and iPhone | Live at jobscout.page · web, Android and iPhone · [See the system →](https://github.com/kenmwara/jobscout-app) |
| **[Unified Ops Dashboard](https://github.com/kenmwara/unified-ops-dashboard)**<br><sub>Cloudflare D1 · Workers · Pages · Access</sub> | One private dashboard where every product reports its sales, sign-ups and errors, kept in a record nothing can edit | Live · every product reports into one dashboard · [See the system →](https://github.com/kenmwara/unified-ops-dashboard) |
<!-- END section:systems -->

**Also running:** [T BOT Web Studio](https://studio.tbot.trade) (small-business sites, shipped on Cloudflare Pages) · **S-Ryder** (the live operating app for a Nairobi delivery business) · [tbot-client](https://github.com/kenmwara/tbot-client) (open-source subscriber client) · the full portfolio at [tbot.trade/portfolio](https://tbot.trade/portfolio)

<!-- BEGIN section:toolkit -->
<a name="toolkit"></a><a href="https://github.com/kenmwara/kenmwara#toolkit"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/section-toolkit.png?v=af67a51ac8" width="100%" alt="Toolkit"></a>

**AI security** &nbsp; <a href="https://github.com/kenmwara/kenmwara#ai"><img src="https://img.shields.io/badge/MCP-1f6f8b?style=flat-square&labelColor=14202e" alt="MCP"></a> <a href="https://github.com/kenmwara/kenmwara#ai"><img src="https://img.shields.io/badge/Claude_Code-1f6f8b?style=flat-square&labelColor=14202e" alt="Claude Code"></a> <a href="https://github.com/kenmwara/kenmwara#ai"><img src="https://img.shields.io/badge/OWASP_LLM_Top_10-1f6f8b?style=flat-square&labelColor=14202e" alt="OWASP LLM Top 10"></a> <a href="https://github.com/kenmwara/kenmwara#ai"><img src="https://img.shields.io/badge/MITRE_ATLAS-1f6f8b?style=flat-square&labelColor=14202e" alt="MITRE ATLAS"></a>

**Hunt & detect** &nbsp; <a href="https://github.com/kenmwara/kenmwara#hunt"><img src="https://img.shields.io/badge/Microsoft_Defender_for_Endpoint-A8323D?style=flat-square&labelColor=14202e" alt="Microsoft Defender for Endpoint"></a> <a href="https://github.com/kenmwara/kenmwara#hunt"><img src="https://img.shields.io/badge/Microsoft_Sentinel-A8323D?style=flat-square&labelColor=14202e" alt="Microsoft Sentinel"></a> <a href="https://github.com/kenmwara/kenmwara#hunt"><img src="https://img.shields.io/badge/KQL-A8323D?style=flat-square&labelColor=14202e" alt="KQL"></a> <a href="https://github.com/kenmwara/kenmwara#hunt"><img src="https://img.shields.io/badge/Sysmon-A8323D?style=flat-square&labelColor=14202e" alt="Sysmon"></a> <a href="https://github.com/kenmwara/kenmwara#hunt"><img src="https://img.shields.io/badge/Wireshark-A8323D?style=flat-square&labelColor=14202e" alt="Wireshark"></a> <a href="https://github.com/kenmwara/kenmwara#hunt"><img src="https://img.shields.io/badge/Nmap-A8323D?style=flat-square&labelColor=14202e" alt="Nmap"></a>

**Identity** &nbsp; <a href="https://github.com/kenmwara/kenmwara#identity"><img src="https://img.shields.io/badge/Active_Directory-2F4C80?style=flat-square&labelColor=14202e" alt="Active Directory"></a> <a href="https://github.com/kenmwara/kenmwara#identity"><img src="https://img.shields.io/badge/Group_Policy-2F4C80?style=flat-square&labelColor=14202e" alt="Group Policy"></a> <a href="https://github.com/kenmwara/kenmwara#identity"><img src="https://img.shields.io/badge/Windows_LAPS-2F4C80?style=flat-square&labelColor=14202e" alt="Windows LAPS"></a> <a href="https://github.com/kenmwara/kenmwara#identity"><img src="https://img.shields.io/badge/PowerShell-2F4C80?style=flat-square&labelColor=14202e" alt="PowerShell"></a>

**Harden** &nbsp; <a href="https://github.com/kenmwara/kenmwara#harden"><img src="https://img.shields.io/badge/Tenable-B4623C?style=flat-square&labelColor=14202e" alt="Tenable"></a> <a href="https://github.com/kenmwara/kenmwara#harden"><img src="https://img.shields.io/badge/DISA_STIGs-B4623C?style=flat-square&labelColor=14202e" alt="DISA STIGs"></a>

**Build & run** &nbsp; <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/Python-5D3D79?style=flat-square&labelColor=14202e" alt="Python"></a> <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/TypeScript-5D3D79?style=flat-square&labelColor=14202e" alt="TypeScript"></a> <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/Kotlin-5D3D79?style=flat-square&labelColor=14202e" alt="Kotlin"></a> <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/Swift-5D3D79?style=flat-square&labelColor=14202e" alt="Swift"></a> <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/SQL-5D3D79?style=flat-square&labelColor=14202e" alt="SQL"></a> <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/Cloudflare-5D3D79?style=flat-square&labelColor=14202e" alt="Cloudflare"></a> <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/DigitalOcean-5D3D79?style=flat-square&labelColor=14202e" alt="DigitalOcean"></a> <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/Claude_API-5D3D79?style=flat-square&labelColor=14202e" alt="Claude API"></a>
<!-- END section:toolkit -->

<!-- BEGIN section:credentials -->
<a name="credentials"></a><a href="https://github.com/kenmwara/kenmwara#credentials"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/section-credentials.png?v=118c6f219f" width="100%" alt="Credentials"></a>

<a href="https://credentials.edx.org/credentials/89cc10e390654c709f8e9d902fffe419/"><img src="https://img.shields.io/badge/HarvardX-CS_for_Cybersecurity_%C2%B7_2026-A8323D?style=flat-square&labelColor=14202e" alt="HarvardX: CS for Cybersecurity · 2026"></a> <a href="https://cs50.harvard.edu/certificates/02ad8b9a-e117-4d13-98c0-1a7f2d028974"><img src="https://img.shields.io/badge/Harvard_CS50-Cybersecurity_%C2%B7_2026-A8323D?style=flat-square&labelColor=14202e" alt="Harvard CS50: Cybersecurity · 2026"></a> <a href="https://credentials.edx.org/credentials/c9bb24239a3044629308c0dde14aa3ca/"><img src="https://img.shields.io/badge/HarvardX-CS_for_AI_%C2%B7_2026-A8323D?style=flat-square&labelColor=14202e" alt="HarvardX: CS for AI · 2026"></a> <a href="https://cs50.harvard.edu/certificates/8c4ed10c-bec1-4bc1-bea1-a611b22489a0"><img src="https://img.shields.io/badge/Harvard_CS50-AI_with_Python_%C2%B7_2026-A8323D?style=flat-square&labelColor=14202e" alt="Harvard CS50: AI with Python · 2026"></a> <a href="https://www.credential.net/718b441f-b5a6-4c99-8582-d68bd00dba11"><img src="https://img.shields.io/badge/UBC-Ethical_Hacking_%C2%B7_2025-A8323D?style=flat-square&labelColor=14202e" alt="UBC: Ethical Hacking · 2025"></a> <a href="https://kenmwara.com/timetable/"><img src="https://img.shields.io/badge/WGU-B.S._Cybersecurity_%C2%B7_enrolled%2C_starts_Jan_2027-1f6f8b?style=flat-square&labelColor=14202e" alt="WGU: B.S. Cybersecurity · enrolled, starts Jan 2027"></a>
<!-- END section:credentials -->

<!-- BEGIN section:principles -->
<a name="principles"></a><a href="https://github.com/kenmwara/kenmwara#principles"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/section-principles.png?v=8d678e6cd2" width="100%" alt="How I work"></a>
<!-- END section:principles -->

- **Keep systems apart.** One failing never takes another down.
- **Never overwrite the record.** A history you can check beats a total you can't.
- **Label every number.** Measured, modeled or absent. Never made up.
- **Ship small, then watch.** A week of watching before the next thing.

<p align="center">
  <a href="https://linkedin.com/in/kenmwara"><img src="https://img.shields.io/badge/LinkedIn-kenmwara-1f6f8b?style=flat-square&labelColor=14202e" alt="LinkedIn: kenmwara"></a>
  <a href="https://tbot.trade/portfolio"><img src="https://img.shields.io/badge/Portfolio-tbot.trade-1f6f8b?style=flat-square&labelColor=14202e" alt="Portfolio: tbot.trade"></a>
  <a href="https://x.com/Ken_Mwara"><img src="https://img.shields.io/badge/X-Ken__Mwara-1f6f8b?style=flat-square&labelColor=14202e" alt="X: Ken_Mwara"></a>
  <a href="mailto:ken@tbot.trade"><img src="https://img.shields.io/badge/Email-ken%40tbot.trade-1f6f8b?style=flat-square&labelColor=14202e" alt="Email: ken@tbot.trade"></a>
</p>
<p align="center"><sub>Open to conversations on threat hunting, detection engineering and Active Directory.</sub></p>
