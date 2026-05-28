📝 README.md

```bash
cd ~/bakome-recon-x && cat > README.md << 'EOF'
# 🛡️ BAKOME-Recon-X v4.0 « COLOSSUS »

[![Rust](https://img.shields.io/badge/Rust-1.75+-orange?logo=rust)](https://www.rust-lang.org)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![Version](https://img.shields.io/badge/Version-4.0.0-blue)](Cargo.toml)
[![Lines](https://img.shields.io/badge/Lines-2500+-brightgreen)](src/main.rs)
[![Sponsors](https://img.shields.io/badge/Sponsor-♥-pink?logo=github-sponsors)](https://github.com/sponsors/BAKOME-Hub)

<p align="center">
  <img src="https://image.pollinations.ai/prompt/A_cinematic_8K_epic_render_of_BAKOME-Recon-X_bug_bounty_framework,_holographic_terminal_with_code,_vulnerability_scanners,_neon_colors,_dark_cyberpunk_theme?width=1200&height=630&seed=100" width="100%">
</p>

<p align="center"><i>🛡️ 44+ integrated scanners · crt.sh · Shodan · Censys · AI-powered reporting · Pure Rust</i></p>

---

## 🎥 BAKOME-Recon-X in Action

| Demo | Video |
|------|-------|
| 🔍 **Full Recon Scan** | [▶️ Watch](https://video.pollinations.ai/prompt/A_realistic_video_of_a_developer_running_BAKOME_Recon_X_in_a_terminal,_scanning_a_website,_subdomains_appearing,_vulnerabilities_detected,_cyberpunk_theme?duration=5&seed=200) |
| 🛡️ **Vulnerability Detection** | [▶️ Watch](https://video.pollinations.ai/prompt/A_realistic_video_of_BAKOME_Recon_X_detecting_CORS_misconfiguration_and_subdomain_takeover,_alerts_appearing,_terminal_output?duration=5&seed=201) |
| 🤖 **AI-Powered Report** | [▶️ Watch](https://video.pollinations.ai/prompt/A_realistic_video_of_BAKOME_Recon_X_generating_an_AI_powered_security_report,_Ollama_processing,_Markdown_file_saved?duration=5&seed=202) |

---

## 🧠 What is BAKOME-Recon-X?

**BAKOME-Recon-X** is the ultimate open-source bug bounty reconnaissance and pentest framework built in pure Rust. It automates **subdomain discovery** (crt.sh, Shodan, Censys, brute force), **port scanning**, **technology detection**, **vulnerability assessment** (CORS, subdomain takeover, WordPress enumeration, secret extraction, IDOR), and **AI-powered report generation** (Ollama + DeepSeek).

---

## 🏗️ Features

| Module | Description |
|--------|-------------|
| 🔍 **Subdomain Discovery** | crt.sh, Shodan, Censys, brute force |
| ⚡ **Port Scanning** | TCP connect, top 1000 ports, async |
| 🧩 **Technology Detection** | Wappalyzer-like fingerprints (WordPress, Cloudflare, React, etc.) |
| 🛡️ **CORS Misconfiguration** | Wildcard, credentials, arbitrary origin |
| 📁 **Sensitive Files** | .env, .git/config, backups, etc. |
| 🏴 **Subdomain Takeover** | 16+ service signatures (GitHub Pages, Heroku, AWS S3, etc.) |
| 📝 **WordPress Enumeration** | REST API user enumeration |
| 🔑 **Secret Extraction** | API keys, tokens, passwords in JavaScript |
| 🧪 **IDOR Testing** | Insecure Direct Object Reference |
| 🤖 **AI Reporting** | Ollama (local) + DeepSeek (cloud) |
| 📊 **Report Generation** | Markdown, JSON, Bugcrowd template |

---

## ⚙️ Quick Start

```bash
git clone https://github.com/BAKOME-Hub/BAKOME-Recon-X.git
cd BAKOME-Recon-X
cargo build --release
cargo run -- scan example.com -o report
```

---

📊 Live Demo Output

```
╔══════════════════════════════════════════════════╗
║   BAKOME-Recon-X v4.0 COLOSSUS                 ║
╚══════════════════════════════════════════════════╝
🔍 Scanning example.com

═══ Subdomain Discovery ═══
✅ 15 subdomains found.

═══ Port Scanning ═══
✅ Port 80 open
✅ Port 443 open

═══ Technology Detection ═══
✅ Detected: Cloudflare

═══ Vulnerability Scanning ═══
⚠️ 2 CORS issues found
🚨 1 potential subdomain takeover
🚨 3 secret leaks found

═══ AI Analysis ═══
Prioritize CORS and secret leaks...

🎉 Scan completed in 49.87s.
```

---

💖 Support Open Source

```
₿ BTC  : bc1qhtjp3qpqru4vuqd355dfcn46mqjrlpdfmngk6u0
Ξ ETH  : 0x2fD73626714d9e37EA464109F8eCeA2CA5401062
◎ SOL  : 3CfhghA7hSNPBbd1RME5rRDm5UUeesTq9NKTcyzZdkz4
₮ USDT : THkLdiKsmscJFwBPA4tpWeAn1xVw7DTKxq (TRC20)
```

🔗 GitHub Sponsors · Drips

---

👤 Author

BAKOME — @BAKOME-Hub

📜 License

MIT — Free to use, modify, and distribute.

---

Built for bug bounty hunters. Powered by open source. 🚀
EOF
