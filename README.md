# 🎯 Lifelong Catch & Correct

**Offline-first SOC training platform with verifiable proof-of-work artifacts**

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE-CORE)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey)](#installation)
[![Status](https://img.shields.io/badge/Status-Production%20Ready-green)](#)

---

## 🚀 What is This?

**Lifelong Catch & Correct** is a desktop application for learning cybersecurity operations through hands-on labs. Unlike cloud-based training platforms, everything runs 100% locally—no network required, no telemetry, no monthly fees for core features.

### Core Principles
✅ **Offline-first** - No network required after install  
✅ **Privacy-respecting** - All data stays in your local Vault  
✅ **Verifiable proof-of-work** - Generate portfolio artifacts for job applications  
✅ **Deterministic execution** - Labs behave identically on every run  
✅ **Open-core model** - Core platform is Apache 2.0; premium labs available  

---

## 📦 Features

### 🔬 Hands-On Labs
- 10+ SOC Tier 1 scenarios (DNS beaconing, phishing, lateral movement, etc.)
- Sandboxed execution with evidence capture
- Timeline creation, decision logs, artifact generation
- SHA256 verification for data integrity

### 📄 Portfolio Artifacts
- **Incident Case Packets** - Complete investigation summaries
- **Escalation Packets** - Professional handoff documents
- **Runbook Updates** - Procedural improvements
- **Interview Stories** - STAR-formatted narratives for interviews
- All exports include QR codes for tamper detection

### 🎤 Mock Interview Practice
- Offline voice transcription (whisper.cpp)
- Adaptive questioning with branching logic
- Persona-based interviewers (calm, skeptical, interrupting)
- Automated scoring on 8 key signals
- Debrief exports for self-review

### 🔐 Security & Compliance
- No email/Gmail/Google APIs
- No background network calls
- FERPA, GDPR, CCPA alignment
- Audit logs for all operations
- Backup/restore with encryption support

---

## 📥 Installation

### Quick Start
1. Download the installer for your platform:
   - **Windows:** `lifelong-catch-correct_v1.0.0.msi`
   - **macOS:** `lifelong-catch-correct_v1.0.0.dmg`
   - **Linux:** `lifelong-catch-correct_v1.0.0.AppImage` or `.deb`

2. Run the installer and select a Vault location (folder where all data is stored)

3. Launch the app - curriculum modules load automatically

4. Start with **SOC1-Triage-001** (DNS Beaconing) for a 30-minute intro

### Building from Source
```bash
# Clone repo
git clone https://github.com/quantam101/lifelong-catch-correct.git
cd lifelong-catch-correct/core

# Install dependencies
npm ci

# Development mode
npm run tauri dev

# Production build
npm run tauri build
```

See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed build instructions.

---

## 🎓 Getting Started

### First Lab Walkthrough (30 minutes)
1. **Launch app** → Select "Guided Mode"
2. **Choose SOC1-Triage-001** (DNS Beaconing Detection)
3. **Follow prompts** to:
   - Analyze DNS query logs
   - Create a timeline with UTC timestamps
   - Document decision-making process
   - Generate hypotheses
4. **Verify completion** → Gates enforce quality standards
5. **Export artifacts** → Get PDF portfolio pack with SHA256 manifest

### Interview Practice (45 minutes)
1. **Navigate to Interview tab**
2. **Select "SOC Tier 1 Analyst" role**
3. **Choose persona** (start with "Calm" for first attempt)
4. **Record answers** via microphone (transcribed offline)
5. **Review scoring** on 8 key signals
6. **Export debrief** → Markdown summary + session JSON

---

## 📂 Project Structure

```
lifelong-catch-correct/
├── core/                    # Open source (Apache 2.0)
│   ├── src/                # React frontend
│   ├── src-tauri/          # Rust backend
│   ├── vault_seed/         # 10 starter labs + templates
│   └── data/               # Interview personas + flows
├── proprietary/            # Commercial (closed source)
│   ├── curriculum/         # Full lab library
│   ├── datasets/           # Real-world scenarios
│   └── instructor/         # Cohort management
├── docs/                   # Technical documentation
├── scripts/                # Build/verification pipelines
└── release/                # SBOM, checksums, attestations
```

---

## 🤝 Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for:
- Code of Conduct
- Development setup
- PR guidelines
- Contributor License Agreement (CLA)

### Areas to Contribute
- 🐛 **Bug fixes** - See [open issues](https://github.com/quantam101/lifelong-catch-correct/issues)
- 📚 **Lab content** - Submit new scenarios via [Lab Contribution template](.github/ISSUE_TEMPLATE/lab_contribution.md)
- 🌍 **Translations** - Help make the platform multilingual
- 📖 **Documentation** - Improve guides, tutorials, examples

---

## 📊 Business Model (Open-Core)

| Tier | Price | What You Get |
|------|-------|-------------|
| **Individual (Free)** | $0 | Core platform + 2 sample labs |
| **Learner** | $29/mo | All 10+ labs + certification eligible |
| **Instructor** | $99/mo | Cohort management + analytics |
| **Enterprise** | Custom | Unlimited cohorts + white-label |
| **Partner** | 70/30 split | Create and sell custom content |

---

## 📜 License

This project uses a **dual-license model**:

- **Core platform** (`core/` directory): [Apache License 2.0](LICENSE-CORE)
- **Proprietary content** (`proprietary/` directory): [Commercial License](LICENSE-PROPRIETARY)

See [NOTICE.md](NOTICE.md) for full license details and third-party attributions.

---

## 🔒 Security

For vulnerability reports, see [SECURITY.md](SECURITY.md).  
**Do not** open public issues for security concerns.

---

## 📞 Support

- **Documentation:** [docs/](docs/)
- **Discussions:** [GitHub Discussions](https://github.com/quantam101/lifelong-catch-correct/discussions)
- **Issues:** [GitHub Issues](https://github.com/quantam101/lifelong-catch-correct/issues)
- **Twitter:** [@Ask_Rube](https://twitter.com/Ask_Rube)

---

## 🌟 Roadmap

### v1.1 (Q1 2026)
- [ ] Multi-language support (Spanish, French, Japanese)
- [ ] Team collaboration features
- [ ] Advanced analytics dashboard
- [ ] Custom lab authoring UI

### v1.2 (Q2 2026)
- [ ] Mobile companion app (read-only)
- [ ] Video walkthrough generator
- [ ] Integration with LMS platforms

---

## 🙏 Acknowledgments

Built with:
- [Tauri](https://tauri.app/) - Cross-platform desktop framework
- [whisper.cpp](https://github.com/ggerganov/whisper.cpp) - Offline speech recognition
- [Rust](https://www.rust-lang.org/) & [React](https://react.dev/) - Core technologies

Inspired by the need for privacy-respecting, verifiable training in cybersecurity education.

---

**Ready to build your SOC portfolio?** [Download v1.0.0](#) or [Build from source](#building-from-source)
