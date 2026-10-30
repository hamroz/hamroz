<div align="center">

<img src="assets/terminal.svg" width="100%" alt="Terminal: Hamroz Gavharov, software engineer, applied AI × cybersecurity">

<a href="https://www.linkedin.com/in/hamroz-gavharov/"><img src="https://img.shields.io/badge/LinkedIn-hamroz--gavharov-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
<a href="mailto:hamroz.gavharov@gmail.com"><img src="https://img.shields.io/badge/Email-hamroz.gavharov%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
<img src="https://img.shields.io/badge/Berlin-open%20to%20roles-34d399?style=flat-square" alt="Berlin, open to roles">
<a href="https://www.credly.com/badges/c0df4b24-98a9-4e90-a693-40f28532676b/public_url"><img src="https://img.shields.io/badge/Cisco-CCNA-1BA0D7?style=flat-square&logo=cisco&logoColor=white" alt="CCNA"></a>

</div>

I build software with AI agents every day, and I care about what happens when those agents touch real systems.
MSc in Applied Cybersecurity (Erasmus Mundus CyberMACS, Berlin + Istanbul). My thesis made an LLM turn
analyst questions into **safe** Elasticsearch queries. Before that: sole full-stack engineer for a US franchise group, where I
shipped a platform to 30+ production sites, the release pipeline behind it, and the self-hosted agent stack I worked with.

## ⚡ The agent stack I actually run

```yaml
# ~/.config/hamroz/agents.yaml
coding:       [claude-code, codex, opencode → openrouter, cursor-agent]
claude_code:  [custom skills, pre-tool hooks, MCP servers]
self_hosted:  [paperclip, hermes-agent, ollama, open-webui]  # hardened Docker + Caddy
building:     [multi-agent orchestration, RAG, n8n AI nodes, LLM observability]
red_team:     [promptfoo, garak, PyRIT, Inspect]
guardrails:   remote actions → allowlisted, audited SSH gateway. never raw shell.
rule:         "agents do the typing; I own the design, the tests, the blast radius"
```

## 🧪 Things I've built

| Project | What it is | Built with |
| --- | --- | --- |
| **[PayFix](https://github.com/hamroz/payfix)** · [live](https://payfix-mu.vercel.app) | Colosseum hackathon (team of 3). Turns wrong USDC payments on Solana into one shared settlement link: claim-once signatures, double-entry ledger in exact token units. Built with AI coding agents under milestone acceptance gates. | Next.js 16 · TypeScript · Solana |
| **[ES-NL2DSL](https://github.com/hamroz/es-nl2dsl)** | MSc thesis. Natural language → Elasticsearch DSL for SOC threat hunting. Execution F1 **0.91** over 12 SOC scenarios; blocks **97.2%** of adversarial prompts at 3.1% false positives, across OpenAI, Anthropic, Gemini and local Ollama. | Python · LLMs · Elasticsearch |
| **[EasyControl](https://github.com/hamroz/easy-control)** | Control your Mac with hand gestures. Apple Vision hand landmarks feed my own Core ML pose classifier (**94.3%** on people it has never seen). Fully on-device, no frames stored. | Swift · Vision · Core ML |
| **[Mac Tools](https://github.com/hamroz/mac-tools)** | Menu-bar toolkit, including a live gauge for how much of my **Claude** and **Codex** limits is left. Local-first. | Swift · SwiftUI |
| **[Easy Learn](https://github.com/hamroz/easy-learn)** | Type a topic, get an AI-designed course: editable outline, per-topic visual identity, long-form lessons with interactive widgets. | Next.js · Postgres · LLM agents |
| **[moodle_stripe_payment](https://github.com/hamroz/moodle_stripe_payment)** | Stripe gateway for Moodle. Its big brother, a private cohort-subscription plugin, has sold access to 200+ buyers. | PHP · Stripe |

## 🛡️ Security work

- **AI security:** LLM red-teaming and evals; an LLM-assisted phishing-simulation platform (GoPhish + GPT, Claude, Llama 3.1) at SecureWay, a PCI QSA firm, where I also supported PCI DSS v4 audits.
- **Blue team:** Wazuh + Elastic SOC lab, detection rules mapped to MITRE ATT&CK, triage write-ups.
- **Red team:** internal Active Directory pentest (LLMNR poisoning, SMB relay, Kerberoasting, pass-the-hash) with a NIST SP 800-115 report. CTFs, OSCP/OSWP in progress.

## 🧱 Engineering I'm proud of

- **Fleet release pipeline:** self-hosted update channel that rejects anything failing a SHA-256 check, staged rollouts (staging → 3 canaries → batches of 10, halt on first failure) across 30+ sites.
- **Ops gateway:** SSH/CLI gateway with a command allowlist, automatic DB snapshots before any write, and an audit log. My agents use it too.
- **Health-gated staging CI/CD** across 7 services for a pricing platform: GitHub Actions, Docker Compose, preflight checks, deploy lock, graceful nginx reloads.
- **Campus face-recognition checkpoint** (BSc thesis): Django + React, deployed at the University of Central Asia, best CS thesis of the year.

## 🧰 Toolbox

<p align="center">
  <img src="https://skillicons.dev/icons?i=ts,nextjs,react,nodejs,python,fastapi,django,swift,go,rust,php,postgres,redis,mongodb&perline=14" alt="Languages and frameworks"><br>
  <img src="https://skillicons.dev/icons?i=docker,kubernetes,terraform,aws,cloudflare,githubactions,linux,bash,elasticsearch,grafana,prometheus,kafka,pytorch&perline=14" alt="Infrastructure and data">
</p>

<sub>Most of my client work lives in private repos. Happy to walk through any of it.</sub>
