<p align="center">
  <img src="assets/profile.jpg" width="170" alt="Abdelrhman Silem" />
</p>

<h1 align="center">Abdelrhman Silem</h1>
<p align="center"><strong>Security researcher &amp; bug bounty hunter</strong><br />Web · API · Android reverse engineering · AI-assisted tooling</p>

<p align="center">
  <a href="https://abdelrhmansalim.vercel.app"><img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-virusboda-2ea44f?style=flat-square" /></a>
  <a href="https://hackerone.com/virusboda"><img alt="HackerOne" src="https://img.shields.io/badge/HackerOne-virusboda-1f2a23?style=flat-square" /></a>
  <a href="https://bugcrowd.com/h/virusboda"><img alt="Bugcrowd" src="https://img.shields.io/badge/Bugcrowd-virusboda-f36c22?style=flat-square" /></a>
</p>

<p align="center">
  <a href="https://abdelrhmansalim.vercel.app">Portfolio</a> ·
  <a href="https://hackerone.com/virusboda">HackerOne</a> ·
  <a href="https://bugcrowd.com/h/virusboda">Bugcrowd</a> ·
  <a href="https://www.linkedin.com/in/abdelrhman-silem-61050a384/">LinkedIn</a> ·
  <a href="https://x.com/SilemAbdelrhman">X</a> ·
  <a href="https://medium.com/@abdelrhmansleem998">Medium</a>
</p>

## About

Independent bug bounty hunter and security researcher (handle: **virusboda** on HackerOne and Bugcrowd), currently a Computer Science student at Suez Canal University, Faculty of Computers and Information. Background in competitive programming (ICPC) and web application penetration testing. I test web apps and APIs, reverse engineer shipped Android and native binaries, and build AI-assisted tooling for the boring half of the work.

**Live portfolio:** https://abdelrhmansalim.vercel.app

## Bug bounty targets

| Program | Platform | Work |
|---|---|---|
| Agoda | HackerOne | CORS origin reflection with credentials on sensitive endpoints (card deletion, name change); two-tier JWT architecture review |
| Vodafone Egypt | HackerOne | OAuth authorization code leaked to a third-party domain via the `x-dtreferer` header |
| Arc | HackerOne | Consensus signer without anti-equivocation state, unauthenticated CL admin RPC, pending-state blocklist gaps — proven with local harnesses (6/6, 12/12) |
| Syfe | HackerOne | WAF bypass via exposed origin IP with Laravel debug mode live in production; referral IDOR leaking user PII |
| Just Eat Takeaway | Bugcrowd | XSS sanitizer bypass in the SSR fallback path of the PIE cookie-banner component |
| McGraw-Hill | HackerOne VDP | Unauthenticated AEM JCR content disclosure via a `.xml` selector on a staging host |
| Lexzur | Private | Cross-tenant BOLA leaking JWTs, CSRF + IDOR on user edit, anonymous Confluence REST exposure, unauthenticated Swagger on the Lexa AI API |
| Khatwetk | Private | CORS wildcard with credentials, publicly readable S3 bucket, DOM open redirect, JWT in localStorage, payment endpoint findings |
| FCI | Private | Unauthenticated API exposing instructor PII |

Other programs and platforms: Aiven, Auth0 by Okta, Mattermost, Netflix, Epic Games, Vercel, Box, Coupang, Expensify, Nebius, Zapier, Whatnot.

## Reverse engineering

Android-first, native where the answer lives there.

- **APK analysis** — jadx and apktool on a production game client: 10,385 classes, 6,721 DEX files and 10,859 resources mapped, then swept for credentials and internal endpoints.
- **Native binaries** — Ghidra headless analysis and decompilation on a 493 MB Unreal `libUnreal.so`, symbol and property sweeps for engine configuration material.
- **Runtime instrumentation** — Frida on a physical device to dump live configuration and observe API traffic when static analysis dead-ends.
- **Signing and provenance** — APK Signing Block parsing for v2/v3 certificates so a build is proven vendor-signed before it is trusted; certificate-pinning checks against intercepted traffic.
- **Secret triage** — 121 base64 literals decoded, leaked API keys validated with read-only oracles; a key that unlocks nothing gets dropped instead of reported.
- **Toolchain** — adb · apktool · uber-apk-signer · jadx · Ghidra · Frida · Python.

## AI & automation

- **AI-assisted hunting pipeline** — recon → triage → validation driven by agents, with hard gates: every candidate still needs a control-vs-attack diff and a replay before it is called a finding.
- **VirusAi.py** — Telegram security bot powered by Gemini.
- **AI XSS scanner** — mitmproxy interception feeding a Groq-hosted model that classifies reflected contexts.
- **Custom MCP tooling** — jadx, Ghidra and Android-device MCP servers wired into the agent so the model drives real tooling instead of guessing.
- **LLM application security** — prompt injection, indirect injection through documents, and agentic tool-use abuse (current research direction).

## Certifications

- **Google Cybersecurity Professional Certificate** — Google, via Coursera
- **McKinsey Forward Program** — McKinsey.org
- **CS50x — Introduction to Computer Science** — Harvard University

## Skills

- **Languages & scripting:** C++, Python, Java, Bash, JavaScript, HTML/CSS
- **Security:** web application penetration testing, API testing, OSINT, reconnaissance and attack surface mapping, reporting
- **Reverse engineering:** jadx, apktool, Ghidra, Frida, adb, APK signing/provenance, secret extraction
- **Systems & networking:** Linux, Windows Server administration basics, networking fundamentals
- **Web/backend:** Node.js, Express, web fundamentals
- **Other:** Git & GitHub, databases, system analysis

## Vulnerability classes

XSS, SQLi, IDOR/BOLA, XXE, SSRF, CSRF, LFI, file upload, broken access control, information disclosure, authentication flaws, API testing, business logic flaws.

## Projects

- **Rofixa** — SaaS platform for construction finishing cost estimation and a contractor marketplace, targeting Egypt with planned expansion across the Arab world. Nine-role RBAC matrix and a completed security threat model.
- **VirusAi.py** — Telegram security bot powered by Gemini AI.
- **XSS scanner** — Python tool built on mitmproxy with Groq AI.
- **ASM/bug bounty automation pipeline** — reconnaissance and attack surface monitoring pipeline.

## Currently learning

OSCP and CRTP paths, Active Directory offensive security (HTB Academy, GOAD lab, BloodHound, Impacket, Mimikatz), C++ systems programming for security tooling.

## Contact

- Portfolio: [abdelrhmansalim.vercel.app](https://abdelrhmansalim.vercel.app)
- GitHub: [abdelrhmansleem998-sketch](https://github.com/abdelrhmansleem998-sketch)
- LinkedIn: [abdelrhman-silem](https://www.linkedin.com/in/abdelrhman-silem-61050a384/)
- X: [@SilemAbdelrhman](https://x.com/SilemAbdelrhman)
- Medium: [@abdelrhmansleem998](https://medium.com/@abdelrhmansleem998)
