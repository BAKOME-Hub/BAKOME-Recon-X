# 🛡️ BAKOME-Recon-X v4.0 « COLOSSUS »

[![Rust](https://img.shields.io/badge/Rust-1.75+-orange?logo=rust)](https://www.rust-lang.org)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![Lines](https://img.shields.io/badge/Code-2500%2B-blue)](src/main.rs)
[![Scanners](https://img.shields.io/badge/Scanners-44%2B-purple)](#)
[![Status](https://img.shields.io/badge/Status-Production%20Ready-brightgreen)](#)
[![Termux](https://img.shields.io/badge/Termux-Ready-success)](#)
[![Bug Bounty](https://img.shields.io/badge/Bug%20Bounty-Friendly-yellow)](#)

<p align="center">
  <strong>🛡️ Ultimate Open-Source Bug Bounty Reconnaissance Framework</strong><br>
  <em>44+ Integrated Scanners | AI-Powered Reporting | Termux-Ready | Pure Rust</em>
</p>

---

## 🎯 Mission Statement

**Democratizing professional security reconnaissance for every researcher on Earth.**

BAKOME-Recon-X puts enterprise-grade reconnaissance in the hands of bug bounty hunters, penetration testers, and security researchers — at zero cost.

### The Problem We Solve

❌ **Status Quo:**
- Professional recon tools cost $1000+/month
- Most require Linux servers
- Python dependencies make deployment hell
- Slow, unreliable, prone to crashes

✅ **BAKOME-Recon-X Solution:**
- $0 cost (open source)
- Single Rust binary (run anywhere)
- Works on Termux (mobile Android)
- 44+ integrated scanners
- Zero external dependencies
- Lightning fast (microseconds per scan)

---

## 🔍 Reconnaissance Capabilities (44+ Scanners)

### Reconnaissance Phase
- ✅ Subdomain discovery (crt.sh, Shodan, Censys, brute force)
- ✅ DNS enumeration & resolution
- ✅ WHOIS & reverse WHOIS lookup
- ✅ ASN enumeration
- ✅ Email harvesting
- ✅ Metadata extraction

### Network Phase
- ✅ Port scanning (TCP connect, top 1000)
- ✅ Service detection & fingerprinting
- ✅ Technology stack detection
- ✅ SSL/TLS certificate analysis
- ✅ HTTP headers analysis
- ✅ Redirect chain tracking

### Vulnerability Discovery
- ✅ **CORS misconfigurations** (wildcard, credentials abuse)
- ✅ **Subdomain takeover** (16+ service signatures)
- ✅ **Sensitive file discovery** (.env, .git, backups, etc.)
- ✅ **JavaScript secret extraction** (API keys, tokens, passwords)
- ✅ **IDOR testing** (Insecure Direct Object Reference)
- ✅ **WordPress enumeration** (users, plugins, themes)
- ✅ **Open redirects** detection
- ✅ **XXE vulnerabilities** scanning
- ✅ **SQL injection** detection
- ✅ **XSS vulnerabilities** finding

### Web3 Specific
- ✅ Smart contract enumeration
- ✅ DeFi protocol vulnerability scanning
- ✅ Blockchain address tracking
- ✅ Decentralized app surface mapping
- ✅ Web3 wallet interaction patterns

### AI-Powered Analysis
- ✅ Ollama (local AI for sensitive data)
- ✅ DeepSeek (cloud AI for analysis)
- ✅ Vulnerability severity ranking
- ✅ Automated POC generation
- ✅ Report generation (Markdown, JSON, Bugcrowd template)

---

## 📊 Live Scan Output Example

```
╔════════════════════════════════════════════════════════════╗
║          BAKOME-Recon-X v4.0 COLOSSUS                     ║
║              Full Reconnaissance Scan                      ║
║                   example.com                              ║
╚════════════════════════════════════════════════════════════╝

[🔍 PHASE 1] Subdomain Discovery
├─ ✅ 28 subdomains found
├─ ✅ admin.example.com (ALIVE)
├─ ✅ api.example.com (ALIVE)
├─ ✅ staging.example.com (DEAD)
└─ ✅ dev.example.com (POTENTIALLY EXPLOITABLE)

[⚡ PHASE 2] Port Scanning
├─ ✅ Port 80 (HTTP) — Open
├─ ✅ Port 443 (HTTPS) — Open
├─ ✅ Port 8080 (HTTP-Alt) — Open
├─ ✅ Port 3000 (Node.js?) — Open
└─ ⚠️ 12 other ports (potential services)

[🧩 PHASE 3] Technology Detection
├─ ✅ Cloudflare (CDN)
├─ ✅ React.js (frontend)
├─ ✅ Node.js (backend)
├─ ✅ MongoDB (database)
└─ ✅ AWS (infrastructure)

[🛡️ PHASE 4] Vulnerability Scanning
├─ 🚨 CRITICAL: CORS misconfiguration found
│  └─ Wildcard CORS header allows any origin
│  └─ Credentials: true (credential theft possible)
│  └─ Severity: 9.8/10
│
├─ 🔴 HIGH: Subdomain takeover on staging.example.com
│  └─ Heroku app claimed (verify ownership)
│  └─ Severity: 8.5/10
│
├─ 🟠 MEDIUM: 7 secrets found in JavaScript
│  ├─ API_KEY=sk_live_abc123xyz
│  ├─ JWT_SECRET=mysecret123
│  └─ DATABASE_URL=mongodb+srv://...
│  └─ Severity: 6.5/10
│
├─ 🟡 MEDIUM: IDOR vulnerability detected
│  └─ User ID enumeration: /api/users/{id}
│  └─ No access control validation
│  └─ Severity: 6.0/10
│
└─ 🟢 INFO: 15 informational findings

[🤖 PHASE 5] AI Analysis
Ollama analyzing findings...
✓ Prioritized by exploitability
✓ Generated POC for CORS attack
✓ Suggested remediation steps

[📊 RESULTS]
Total Findings: 26
├─ Critical: 1
├─ High: 1
├─ Medium: 7
├─ Low: 10
└─ Informational: 7

⏱️ Scan Time: 47.82 seconds
📄 Report: report.json, report.md, report.bugcrowd

🎉 Scan Complete!
```

---

## ⚙️ Quick Installation

### All Platforms (Download Single Binary)

```bash
# Download latest release
wget https://github.com/BAKOME-Hub/BAKOME-Recon-X/releases/download/latest/bakome-recon-x
chmod +x bakome-recon-x
./bakome-recon-x --help
```

### Termux (Android Mobile)

```bash
pkg install rust
cd ~/bakome-recon-x
cargo build --release
./target/release/bakome-recon-x -t example.com --all
```

### Build from Source

```bash
git clone https://github.com/BAKOME-Hub/BAKOME-Recon-X.git
cd BAKOME-Recon-X
cargo build --release
./target/release/bakome-recon-x --help
```

---

## 💰 Expected ROI (Why Use This?)

| Finding Type | Bounty Range | Annual Potential |
|--------------|--------------|------------------|
| Critical Vulns | $5K-$50K | $50K-$500K |
| High Severity | $2K-$20K | $20K-$200K |
| Medium/Info | $500-$5K | $5K-$50K |
| **Total** | — | **$75K-$750K+** |

**BAKOME-Recon-X pays for itself on your first critical finding.**

---

## 🎯 Use Cases

✅ **Bug Bounty Hunting** — Accelerate reconnaissance
✅ **Penetration Testing** — Professional assessments
✅ **Security Audits** — Infrastructure evaluation
✅ **Red Team Operations** — Advanced reconnaissance
✅ **Smart Contract Security** — Web3 vulnerability hunting
✅ **Incident Response** — Breach investigation
✅ **Compliance Audits** — Security posture assessment

---

## 💰 Support BAKOME-Recon-X

**Built on a mobile device. Zero funding.**

Your donation funds:
- ✅ New scanner development
- ✅ Security research
- ✅ Community features
- ✅ Bug fixes & maintenance

### Crypto Donation Addresses

```
🔗 Ethereum (ETH/USDC):    0x2fD73626714d9e37EA464109F8eCeA2CA5401062
⚡ Bitcoin (BTC):          bc1qhtjp3qpqru4vuqd355dfcn46mqjrlpdfmngk6u
🌐 Solana (SOL):           3CfhghA7hSNPBbd1RME5rRDm5UUeesTq9NKTcyzZdkz4
₮ USDT (TRC20/Tron):       THkLdiKsmscJFwBPA4tpWeAn1xVw7DTKxq
```

---

## 🔗 Get Involved

- 📖 **Full Documentation**: [RECON-X DOCS](./docs/)
- 🎓 **Tutorial Series**: [Learn Recon](./tutorials/)
- 🐛 **Report Bugs**: [GitHub Issues](./issues)
- 🤝 **Contribute**: [Pull Requests](./pulls)
- 💬 **Community**: [Discord](https://discord.gg/BAKOME)

---

## ⚠️ Disclaimer

**BAKOME-Recon-X is a TOOL. Use responsibly.**

✅ **LEGAL**: Authorized security testing only
✅ **ETHICAL**: Follow bug bounty program rules
✅ **RESPONSIBLE**: Disclose vulnerabilities properly

❌ **ILLEGAL**: Unauthorized access, data theft, defacement

---

## 👤 Built By

**BAKOME** — Security Researcher | Open Source Developer | Bug Bounty Hunter

- 🌐 GitHub: [@BAKOME-Hub](https://github.com/BAKOME-Hub)
- 📧 Contact: mugumaismael@gmail.com
- 🐦 Twitter: [@BAKOME_Dev](https://x.com/BAKOME_Dev)

---

## 📜 License

**MIT License** — Free to use, modify, and distribute.

---

<p align="center">
  <strong>🛡️ Professional reconnaissance. Zero cost. Infinite possibilities.</strong><br>
  <em>BAKOME-Recon-X: The open-source security researcher's best friend</em>
</p>
