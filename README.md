<!-- Goes at github.com/kenmwara/kenmwara/README.md — source of truth: github-showcase/PROFILE_README.md (fetch the live file before editing).
     GENERATED blocks: edit brand/cards.json or brand/sections.json, run brand/render.py then brand/build_readme.py, and copy
     brand/out/*.png to kenmwara/kenmwara/assets/brand/. Everything outside the BEGIN/END markers is hand-written.
     House style (Ken, 23 Oct 2026): a fast glimpse must say exactly what I do. Clear, direct, highlighted, a pop of colour;
     details live behind the "→" links, never on the profile. -->

<!-- BEGIN hero -->
<a href="https://linkedin.com/in/kenmwara"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/hero.png?v=66394861" width="100%" alt="Ken Kariuki. Security operations, Vancouver, BC: threat hunting, Active Directory, detection engineering."></a>
<!-- END hero -->

<p align="center"><b>Cybersecurity Engineer (Intern) at LOG(N) Pacific's Cyber Range · Vancouver, BC</b><br>
I hunt threats, run identity and harden systems. And I keep live systems running at 3 AM, when nobody is watching.</p>

<p align="center">
  <a href="https://github.com/kenmwara/kenmwara#ai"><img src="https://img.shields.io/badge/AI_agent_security-1f6f8b?style=for-the-badge" alt="AI agent security"></a> <b>→</b>
  <a href="https://github.com/kenmwara/kenmwara#hunt"><img src="https://img.shields.io/badge/Threat_hunting_%26_detection-A8323D?style=for-the-badge" alt="Threat hunting and detection"></a> <b>→</b>
  <a href="https://github.com/kenmwara/kenmwara#identity"><img src="https://img.shields.io/badge/Identity_%26_AD-2F4C80?style=for-the-badge" alt="Identity and Active Directory"></a> <b>→</b>
  <a href="https://github.com/kenmwara/kenmwara#harden"><img src="https://img.shields.io/badge/Hardening-B4623C?style=for-the-badge" alt="Hardening and vulnerability management"></a> <b>→</b>
  <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/Systems_I_run-5D3D79?style=for-the-badge" alt="Systems I run"></a>
</p>

<p align="center"><sub>One path through the work: secure the AI, hunt what gets in, build and harden what it targets, then run it live. Every project name opens its full report.</sub></p>

<!-- BEGIN section:ai -->
<a name="ai"></a><a href="https://github.com/kenmwara/kenmwara#ai"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/section-ai.png?v=c11124e7" width="100%" alt="AI agent security"></a>

<sub>Start here. AI agents now hold real permissions, so each test asks which control stops one when it is manipulated.</sub>

| Project | What it is | Result |
|---|---|---|
| **[Securing an AI Agent in AD](https://github.com/kenmwara/securing-ai-agents-ad)**<br><sub>Prompt injection · MCP · Active Directory · OWASP LLM · Agentic</sub> | An AI helpdesk agent with delegated rights in Active Directory, tested with prompt injection and misuse to find which control contains it | 13 attack tests · injection never moved the agent · one open gap, v2 in progress · [Read the assessment →](https://github.com/kenmwara/securing-ai-agents-ad) |
| **[Echo Leaks](https://github.com/kenmwara/threat-hunt-echo-leaks)**<br><sub>Prompt injection · Microsoft 365 Copilot · KQL · Entra ID</sub> | A prompt-injection attack on Microsoft 365 Copilot that read 13 confidential files and tried to carry them out | 17/17 flags · a perfect 1,600/1,600, on time · [Read the report →](https://github.com/kenmwara/threat-hunt-echo-leaks) |
<!-- END section:ai -->

<!-- BEGIN section:hunt -->
<a name="hunt"></a><a href="https://github.com/kenmwara/kenmwara#hunt"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/section-hunt.png?v=d5a1a652" width="100%" alt="Threat hunting & detection"></a>

<sub>When something gets through: each hunt rebuilds the attack from Defender and Sentinel telemetry, start to finish.</sub>

| Project | What it is | Result |
|---|---|---|
| **[Harborlight](https://github.com/kenmwara/threat-hunt-harborlight)**<br><sub>Akira ransomware · KQL · Sysmon · Microsoft Defender</sub> | Akira ransomware at a dental practice, traced from a phishing ISO to the domain controller | 46/46 flags · 4,060 / 4,190, on time · [Read the report →](https://github.com/kenmwara/threat-hunt-harborlight) |
| **[Meridian](https://github.com/kenmwara/threat-hunt-meridian)**<br><sub>Linux · Apache · PHP · KQL · Azure Log Analytics · Path traversal</sub> | A compromised Linux web server: path traversal, a reused service-account password and a root backdoor | 16/16 flags · 1,675/1,675, full marks · [Read the report →](https://github.com/kenmwara/threat-hunt-meridian) |
| **[Unauthorized Tor](https://github.com/kenmwara/threat-hunt-tor)**<br><sub>Defender for Endpoint · KQL · Investigation package · MITRE ATT&CK</sub> | A portable Tor Browser on a lab endpoint, hunted back out of Defender telemetry and an investigation package | Tor caught on a lab endpoint · 3 relays traced on port 443 · [Read the report →](https://github.com/kenmwara/threat-hunt-tor) |
| **[T BOT Security Ops](https://github.com/kenmwara/tbot-security)**<br><sub>SIEM · SOAR playbooks · fail2ban · UFW · Cloudflare Workers</sub> | Intrusion detection, a SIEM and a SOAR console with playbooks, guarding a live-money trading system | Live · intrusion detection, SIEM and SOAR · red-teamed nightly · [See the stack →](https://github.com/kenmwara/tbot-security) |
<!-- END section:hunt -->

<!-- BEGIN section:identity -->
<a name="identity"></a><a href="https://github.com/kenmwara/kenmwara#identity"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/section-identity.png?v=b307454c" width="100%" alt="Identity & Active Directory"></a>

<sub>What attackers go after: a Windows domain built from scratch and locked down with Group Policy.</sub>

| Project | What it is | Result |
|---|---|---|
| **[Active Directory Lab](https://github.com/kenmwara/active-directory-lab)**<br><sub>Windows Server 2025 · AD DS · DNS · DHCP · Group Policy · Windows LAPS</sub> | A Windows Server 2025 domain controller and a domain-joined Windows 11 client on Hyper-V, with five Group Policies proven on the client | 999 users · five Group Policies, each proven on the client · [See the lab →](https://github.com/kenmwara/active-directory-lab) |
<!-- END section:identity -->

<!-- BEGIN section:harden -->
<a name="harden"></a><a href="https://github.com/kenmwara/kenmwara#harden"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/section-harden.png?v=a178ff3b" width="100%" alt="Hardening & vuln management"></a>

<sub>Closing the gaps before anyone finds them: every fix verified by a fresh scan.</sub>

| Project | What it is | Result |
|---|---|---|
| **[Vulnerability Management](https://github.com/kenmwara/vulnerability-management-program)**<br><sub>Tenable · Credentialed scans · PowerShell · Windows Server 2025</sub> | A written policy, a credentialed baseline and four remediation rounds on a Windows Server 2025 lab, each verified by rescan | 20 findings → 2 (−90 %) · Critical and High to zero · [See the work →](https://github.com/kenmwara/vulnerability-management-program) |
| **[Windows 11 STIG](https://github.com/kenmwara/windows-11-stig-remediation)**<br><sub>DISA STIG · PowerShell · Tenable compliance audit · Windows 11 25H2</sub> | Ten DISA STIG findings on a Windows 11 lab VM, each remediated with PowerShell and verified by a credentialed compliance scan | 10 of 10 STIG findings · failed → passed · [See the work →](https://github.com/kenmwara/windows-11-stig-remediation) |
<!-- END section:harden -->

<!-- BEGIN section:systems -->
<a name="systems"></a><a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/section-systems.png?v=6b0c144e" width="100%" alt="Systems I run"></a>

<sub>The same discipline on live systems: production platforms I run and monitor every day.</sub>

| Project | What it is | Result |
|---|---|---|
| **[T BOT](https://github.com/kenmwara/tbot)**<br><sub>Python · Risk gates · Nightly reconciliation · Cloudflare</sub> | An autonomous trading platform that has to earn every lane it runs, its books reconciled to the exchange every night | Live money, 24/7 · 17 logged risk gates · books closed to the exchange nightly · [See the system →](https://github.com/kenmwara/tbot) |
| **[JobScout](https://github.com/kenmwara/jobscout-app)**<br><sub>Claude · Kotlin · Compose · Swift · SwiftUI · Cloudflare Workers</sub> | Real postings scored live by Claude with the reasoning shown, and native Android and iOS clients on one guarded API | Live at jobscout.page · web, Android and iOS · [See the system →](https://github.com/kenmwara/jobscout-app) |
| **[Unified Ops Dashboard](https://github.com/kenmwara/unified-ops-dashboard)**<br><sub>Cloudflare D1 · Workers · Pages · Access</sub> | One dashboard every product reports into: an append-only event store on Cloudflare D1, Workers and Pages | Live · every product reports into one event store · [See the system →](https://github.com/kenmwara/unified-ops-dashboard) |
<!-- END section:systems -->

**Also running:** [T BOT Web Studio](https://studio.tbot.trade) (small-business sites, shipped on Cloudflare Pages) · **S-Ryder** (the live operating app for a Nairobi delivery business) · [tbot-client](https://github.com/kenmwara/tbot-client) (open-source subscriber client) · the full portfolio at [tbot.trade/portfolio](https://tbot.trade/portfolio)

<!-- BEGIN section:toolkit -->
<a name="toolkit"></a><a href="https://github.com/kenmwara/kenmwara#toolkit"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/section-toolkit.png?v=af67a51a" width="100%" alt="Toolkit"></a>

**AI security** &nbsp; <a href="https://github.com/kenmwara/kenmwara#ai"><img src="https://img.shields.io/badge/MCP-1f6f8b?style=flat-square&labelColor=14202e" alt="MCP"></a> <a href="https://github.com/kenmwara/kenmwara#ai"><img src="https://img.shields.io/badge/Claude_Code-1f6f8b?style=flat-square&labelColor=14202e" alt="Claude Code"></a> <a href="https://github.com/kenmwara/kenmwara#ai"><img src="https://img.shields.io/badge/OWASP_LLM_Top_10-1f6f8b?style=flat-square&labelColor=14202e" alt="OWASP LLM Top 10"></a> <a href="https://github.com/kenmwara/kenmwara#ai"><img src="https://img.shields.io/badge/MITRE_ATLAS-1f6f8b?style=flat-square&labelColor=14202e" alt="MITRE ATLAS"></a>

**Hunt & detect** &nbsp; <a href="https://github.com/kenmwara/kenmwara#hunt"><img src="https://img.shields.io/badge/Microsoft_Defender_for_Endpoint-A8323D?style=flat-square&labelColor=14202e" alt="Microsoft Defender for Endpoint"></a> <a href="https://github.com/kenmwara/kenmwara#hunt"><img src="https://img.shields.io/badge/Microsoft_Sentinel-A8323D?style=flat-square&labelColor=14202e" alt="Microsoft Sentinel"></a> <a href="https://github.com/kenmwara/kenmwara#hunt"><img src="https://img.shields.io/badge/KQL-A8323D?style=flat-square&labelColor=14202e" alt="KQL"></a> <a href="https://github.com/kenmwara/kenmwara#hunt"><img src="https://img.shields.io/badge/Sysmon-A8323D?style=flat-square&labelColor=14202e" alt="Sysmon"></a> <a href="https://github.com/kenmwara/kenmwara#hunt"><img src="https://img.shields.io/badge/Wireshark-A8323D?style=flat-square&labelColor=14202e" alt="Wireshark"></a> <a href="https://github.com/kenmwara/kenmwara#hunt"><img src="https://img.shields.io/badge/Nmap-A8323D?style=flat-square&labelColor=14202e" alt="Nmap"></a>

**Identity** &nbsp; <a href="https://github.com/kenmwara/kenmwara#identity"><img src="https://img.shields.io/badge/Active_Directory-2F4C80?style=flat-square&labelColor=14202e" alt="Active Directory"></a> <a href="https://github.com/kenmwara/kenmwara#identity"><img src="https://img.shields.io/badge/Group_Policy-2F4C80?style=flat-square&labelColor=14202e" alt="Group Policy"></a> <a href="https://github.com/kenmwara/kenmwara#identity"><img src="https://img.shields.io/badge/Windows_LAPS-2F4C80?style=flat-square&labelColor=14202e" alt="Windows LAPS"></a> <a href="https://github.com/kenmwara/kenmwara#identity"><img src="https://img.shields.io/badge/PowerShell-2F4C80?style=flat-square&labelColor=14202e" alt="PowerShell"></a>

**Harden** &nbsp; <a href="https://github.com/kenmwara/kenmwara#harden"><img src="https://img.shields.io/badge/Tenable-B4623C?style=flat-square&labelColor=14202e" alt="Tenable"></a> <a href="https://github.com/kenmwara/kenmwara#harden"><img src="https://img.shields.io/badge/DISA_STIGs-B4623C?style=flat-square&labelColor=14202e" alt="DISA STIGs"></a>

**Build & run** &nbsp; <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/Python-5D3D79?style=flat-square&labelColor=14202e" alt="Python"></a> <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/TypeScript-5D3D79?style=flat-square&labelColor=14202e" alt="TypeScript"></a> <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/Kotlin-5D3D79?style=flat-square&labelColor=14202e" alt="Kotlin"></a> <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/Swift-5D3D79?style=flat-square&labelColor=14202e" alt="Swift"></a> <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/SQL-5D3D79?style=flat-square&labelColor=14202e" alt="SQL"></a> <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/Cloudflare-5D3D79?style=flat-square&labelColor=14202e" alt="Cloudflare"></a> <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/DigitalOcean-5D3D79?style=flat-square&labelColor=14202e" alt="DigitalOcean"></a> <a href="https://github.com/kenmwara/kenmwara#systems"><img src="https://img.shields.io/badge/Claude_API-5D3D79?style=flat-square&labelColor=14202e" alt="Claude API"></a>
<!-- END section:toolkit -->

<!-- BEGIN section:credentials -->
<a name="credentials"></a><a href="https://github.com/kenmwara/kenmwara#credentials"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/section-credentials.png?v=118c6f21" width="100%" alt="Credentials"></a>

<a href="https://credentials.edx.org/credentials/89cc10e390654c709f8e9d902fffe419/"><img src="https://img.shields.io/badge/HarvardX-CS_for_Cybersecurity_%C2%B7_2026-A8323D?style=flat-square&labelColor=14202e" alt="HarvardX: CS for Cybersecurity · 2026"></a> <a href="https://cs50.harvard.edu/certificates/02ad8b9a-e117-4d13-98c0-1a7f2d028974"><img src="https://img.shields.io/badge/Harvard_CS50-Cybersecurity_%C2%B7_2026-A8323D?style=flat-square&labelColor=14202e" alt="Harvard CS50: Cybersecurity · 2026"></a> <a href="https://credentials.edx.org/credentials/c9bb24239a3044629308c0dde14aa3ca/"><img src="https://img.shields.io/badge/HarvardX-CS_for_AI_%C2%B7_2026-A8323D?style=flat-square&labelColor=14202e" alt="HarvardX: CS for AI · 2026"></a> <a href="https://cs50.harvard.edu/certificates/8c4ed10c-bec1-4bc1-bea1-a611b22489a0"><img src="https://img.shields.io/badge/Harvard_CS50-AI_with_Python_%C2%B7_2026-A8323D?style=flat-square&labelColor=14202e" alt="Harvard CS50: AI with Python · 2026"></a> <a href="https://www.credential.net/718b441f-b5a6-4c99-8582-d68bd00dba11"><img src="https://img.shields.io/badge/UBC-Ethical_Hacking_%C2%B7_2025-A8323D?style=flat-square&labelColor=14202e" alt="UBC: Ethical Hacking · 2025"></a> <a href="https://kenmwara.com/timetable/"><img src="https://img.shields.io/badge/WGU-B.S._Cybersecurity_%C2%B7_enrolled%2C_starts_Jan_2027-1f6f8b?style=flat-square&labelColor=14202e" alt="WGU: B.S. Cybersecurity · enrolled, starts Jan 2027"></a>
<!-- END section:credentials -->

<!-- BEGIN section:principles -->
<a name="principles"></a><a href="https://github.com/kenmwara/kenmwara#principles"><img src="https://raw.githubusercontent.com/kenmwara/kenmwara/main/assets/brand/section-principles.png?v=8d678e6c" width="100%" alt="How I work"></a>
<!-- END section:principles -->

- **Isolate every surface.** One system failing never takes another down.
- **Keep append-only logs.** History you can replay beats state you can't.
- **Label every number.** Measured, modeled or absent. Never made up.
- **Ship small, then watch.** A week of watching before the next thing.

<p align="center">
  <a href="https://linkedin.com/in/kenmwara"><img src="https://img.shields.io/badge/LinkedIn-kenmwara-1f6f8b?style=flat-square&labelColor=14202e" alt="LinkedIn: kenmwara"></a>
  <a href="https://tbot.trade/portfolio"><img src="https://img.shields.io/badge/Portfolio-tbot.trade-1f6f8b?style=flat-square&labelColor=14202e" alt="Portfolio: tbot.trade"></a>
  <a href="https://x.com/Ken_Mwara"><img src="https://img.shields.io/badge/X-Ken__Mwara-1f6f8b?style=flat-square&labelColor=14202e" alt="X: Ken_Mwara"></a>
  <a href="mailto:ken@tbot.trade"><img src="https://img.shields.io/badge/Email-ken%40tbot.trade-1f6f8b?style=flat-square&labelColor=14202e" alt="Email: ken@tbot.trade"></a>
</p>
<p align="center"><sub>Open to conversations on threat hunting, detection engineering and Active Directory.</sub></p>
