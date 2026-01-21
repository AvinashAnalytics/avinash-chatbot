
<div align="center">

# <img src="https://github.com/AvinashAnalytics/AvinashAnalytics.github.io/blob/main/assets/digital_twin_new.jpg" alt="Robot" width="100" height="100" /> Avinash Digital Twin Ecosystem

### *"If I have to do it twice, I script it."*

[![Source Code](https://img.shields.io/badge/%F0%9F%A4%97%20Source_Code-Hugging_Face-yellow?style=for-the-badge)](https://huggingface.co/spaces/AvinashAnalytics/avinash-chatbot/tree/main)
[![Live Demo](https://img.shields.io/badge/🚀_Live-Demo-06b6d4?style=for-the-badge)](https://avinashanalytics-avinash-chatbot.hf.space)
[![Telegram Bot](https://img.shields.io/badge/🤖_Chat-Telegram-26A5E4?style=for-the-badge)](https://t.me/AvinashAnalytics_bot)
[![Groq Powered](https://img.shields.io/badge/⚡_Groq-Llama3_70B-orange?style=for-the-badge)](https://groq.com/)

<br/>

<img src="https://img.shields.io/badge/Version-4.0-purple?style=flat-square"/>
<img src="https://img.shields.io/badge/Status-🟢_Online-brightgreen?style=flat-square"/>
<img src="https://img.shields.io/badge/TTS-Orpheus_Engine-ff6b6b?style=flat-square"/>
<img src="https://img.shields.io/badge/Auth-JWT_+_2FA-blue?style=flat-square"/>
<img src="https://img.shields.io/badge/Codebase-730_KB-yellow?style=flat-square"/>

---

**🧠 A self-aware AI agent that represents my professional identity 24/7**

*RAG-Powered • Voice-Enabled • Admin-Controlled • Always Learning*

<br/>

[🎮 Try Demo](https://avinashanalytics-avinash-chatbot.hf.space) · [📦 Browse Code](https://huggingface.co/spaces/AvinashAnalytics/avinash-chatbot/tree/main) · [🎛️ Admin Panel](https://avinashanalytics-avinash-chatbot.hf.space/mini_app/user) · [📖 Security Docs](https://huggingface.co/spaces/AvinashAnalytics/avinash-chatbot/blob/main/SECURITY.md)

</div>

---

## 📍 Source Code Location

> **🤗 Complete source code hosted on Hugging Face Spaces:**
> 
> ### 👉 [huggingface.co/spaces/AvinashAnalytics/avinash-chatbot](https://huggingface.co/spaces/AvinashAnalytics/avinash-chatbot)
>
> Click the **"Files"** tab to browse all code, or clone using instructions below.

---

## ⚠️ Disclaimer

> **This is NOT a job assignment. This is NOT a tutorial.**
> 
> This is pure *"Vibe Coding"* — hundreds of hours building an AI ecosystem driven by obsession with LLMs, voice synthesis, and automation. Every commit at 2 AM, fueled by curiosity and mass amounts of ☕

---

## 🏗️ System Architecture

```mermaid
flowchart TB
    subgraph Users["🌐 User Layer"]
        WEB["Web Interface"]
        TG_USER["Telegram Users"]
        MINI["Mini App"]
    end

    subgraph Core["🐳 HF Spaces Core"]
        APP["app.py<br/>FastAPI Orchestrator<br/><small>167 KB</small>"]
        TG_BOT["telegram_bot.py<br/>Bot Engine<br/><small>98.6 KB</small>"]
        ADMIN_API["admin_panel_api.py<br/>Dashboard API<br/><small>60.2 KB</small>"]
    end

    subgraph Intelligence["🧠 AI Layer"]
        RAG["rag_engine.py<br/>ChromaDB RAG"]
        INTENT["intent.py<br/>17+ Intents"]
        WORKFLOW["workflow.py<br/>LangGraph"]
        TTS["tts_fallback.py<br/>Orpheus TTS"]
    end

    subgraph Security["🔐 Security Layer"]
        JWT["jwt_auth.py<br/>JWT + 2FA"]
        SEC["security.py<br/>Audit & Revocation"]
    end

    subgraph Storage["💾 Data Layer"]
        CHROMA[("ChromaDB<br/>Vector Memory")]
        SQLITE[("SQLite WAL<br/>Chat History")]
        MYDATA["mydata.txt<br/>Knowledge Base"]
    end

    Users <--> Core
    Core <--> Intelligence
    Core <--> Security
    Intelligence <--> Storage
    
    style Users fill:#0ea5e9,color:#fff
    style Core fill:#8b5cf6,color:#fff
    style Intelligence fill:#f59e0b,color:#fff
    style Security fill:#ef4444,color:#fff
    style Storage fill:#10b981,color:#fff
```

---

## ⚡ Core Features

<table>
<tr>
<td width="50%" valign="top">

### 🧠 Hybrid RAG Memory
**Dual-tier contextual memory:**

| Component | Technology |
|:---|:---|
| Semantic Search | ChromaDB + MiniLM-L6-v2 |
| Chat History | SQLite (WAL Mode) |
| Knowledge Base | `mydata.txt` (18.9 KB) |

</td>
<td width="50%" valign="top">

### 🗣️ Orpheus Voice Engine
**Real-time TTS with fallback chain:**

```
Primary:   Orpheus TTS (v4.0)
Fallback:  Groq TTS
Fallback:  Edge-TTS
```
*See: `tts_fallback.py` & `TTS_FALLBACK_README.md`*

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔐 Enterprise Security
**JWT + 2FA authentication system:**

- 🔑 JWT token authentication
- 📱 2FA with backup codes
- 🚫 Token revocation
- 📋 Full audit logging

*See: `SECURITY.md` for details*

</td>
<td width="50%" valign="top">

### 🤖 Bot Builder
**Visual Telegram bot customization:**

- 📝 Start message editor
- 🔘 Button management
- ⚙️ Dynamic configuration
- 🎨 No-code interface

*See: `button_builder.py`*

</td>
</tr>
</table>

---

## 📁 Complete File Structure

```
avinash-chatbot/                    # 730 KB Total
│
├── 🚀 CORE APPLICATION
│   ├── app.py                      # 167 KB - FastAPI main orchestrator
│   ├── telegram_bot.py             # 98.6 KB - Telegram bot engine
│   ├── admin_panel_api.py          # 60.2 KB - Admin dashboard API
│   └── workflow.py                 # 10.1 KB - LangGraph workflows
│
├── 🧠 AI & INTELLIGENCE
│   ├── rag_engine.py               # 7.77 KB - ChromaDB RAG system
│   ├── intent.py                   # 23.2 KB - Intent classification (17+)
│   ├── memory_engine.py            # 6.5 KB - Memory management
│   ├── model_factory.py            # 3.13 KB - Model initialization
│   └── mydata.txt                  # 18.9 KB - Knowledge base
│
├── 🗣️ VOICE ENGINE
│   ├── tts_fallback.py             # 13.1 KB - Orpheus TTS + fallbacks
│   └── TTS_FALLBACK_README.md      # 7.24 KB - TTS documentation
│
├── 🔐 SECURITY
│   ├── security.py                 # 16.2 KB - Auth & audit system
│   ├── jwt_auth.py                 # 17.9 KB - JWT + 2FA
│   └── SECURITY.md                 # 5.83 KB - Security documentation
│
├── 🎛️ ADMIN TOOLS
│   ├── admin_engine.py             # 13.9 KB - Admin functions
│   ├── admin_replies.py            # 3.91 KB - Manual reply queue
│   ├── button_builder.py           # 11.1 KB - Bot button builder
│   └── logger.py                   # 30.2 KB - Logging system
│
├── 🐳 DEPLOYMENT
│   ├── Dockerfile                  # 2.26 KB - HF Spaces container
│   ├── requirements.txt            # 382 B - Python dependencies
│   ├── .env.example                # 2.82 KB - Environment template
│   └── DEPLOY_EVERYTHING.ps1       # 1.62 KB - Deploy script
│
├── 📁 DIRECTORIES
│   ├── static/                     # Frontend assets (HTML, CSS, JS)
│   ├── project-showcase/           # Showcase page
│   ├── scripts_archive/            # Utility scripts
│   └── tests/                      # Test files
│
└── 📄 OTHER
    ├── README.md                   # This file
    ├── .gitignore
    └── .dockerignore
```

---

## 🛠️ Tech Stack

<div align="center">

| Layer | Technology | File |
|:---:|:---|:---|
| **🧠 LLM** | Llama 3 70B via Groq | `model_factory.py` |
| **💾 Vector DB** | ChromaDB + MiniLM-L6-v2 | `rag_engine.py` |
| **🗄️ Database** | SQLite (WAL Mode) | `logger.py` |
| **⚙️ Backend** | FastAPI + Uvicorn | `app.py` |
| **🔐 Auth** | JWT + TOTP 2FA | `jwt_auth.py`, `security.py` |
| **🗣️ Voice** | Orpheus + Edge-TTS | `tts_fallback.py` |
| **📱 Bot** | python-telegram-bot | `telegram_bot.py` |
| **🐳 Deploy** | Docker on HF Spaces | `Dockerfile` |

</div>

---

## 🚀 Quick Start

### Option 1: Clone with Git-Xet (Recommended)

```bash
# Install git-xet
brew install git-xet      # macOS
git xet install

# Clone repository
git clone https://huggingface.co/spaces/AvinashAnalytics/avinash-chatbot
cd avinash-chatbot
```

### Option 2: HuggingFace CLI

```powershell
# Install HF CLI (Windows)
powershell -ExecutionPolicy ByPass -c "irm https://hf.co/cli/install.ps1 | iex"

# Download Space
hf download AvinashAnalytics/avinash-chatbot --repo-type=space
```

### Option 3: Clone without large files

```bash
GIT_LFS_SKIP_SMUDGE=1 git clone https://huggingface.co/spaces/AvinashAnalytics/avinash-chatbot
```

---

## ⚙️ Environment Setup

Copy `.env.example` to `.env` and configure:

```bash
# ═══════════════════════════════════════════════════════════════
# TELEGRAM CONFIGURATION
# ═══════════════════════════════════════════════════════════════
TELEGRAM_BOT_TOKEN=your_bot_token_from_botfather
ADMIN_TELEGRAM_CHAT_ID=your_telegram_user_id

# ═══════════════════════════════════════════════════════════════
# SECURITY (Required for Admin Panel)
# ═══════════════════════════════════════════════════════════════
ADMIN_API_KEY=generate_with_secrets.token_urlsafe(32)
WEBHOOK_SECRET=generate_with_secrets.token_hex(32)

# ═══════════════════════════════════════════════════════════════
# DEPLOYMENT
# ═══════════════════════════════════════════════════════════════
PORT=7860
```

**Generate secure keys:**
```python
import secrets
print("ADMIN_API_KEY:", secrets.token_urlsafe(32))
print("WEBHOOK_SECRET:", secrets.token_hex(32))
```

---

## 🐳 Run with Docker

```bash
# Build
docker build -t avinash-twin .

# Run
docker run -p 7860:7860 \
  -e TELEGRAM_BOT_TOKEN="your_token" \
  -e ADMIN_TELEGRAM_CHAT_ID="your_id" \
  -e ADMIN_API_KEY="your_key" \
  avinash-twin
```

---

## 📊 System Metrics

<div align="center">

```
╔════════════════════════════════════════════════════════════════════╗
║                    🟢 SYSTEM STATUS: OPERATIONAL                   ║
╠════════════════════════════════════════════════════════════════════╣
║  Component              │  Status      │  Version / Details        ║
╠════════════════════════════════════════════════════════════════════╣
║  🧠 LLM Engine          │  ✅ Online   │  Llama 3 70B @ Groq       ║
║  💾 Vector Memory       │  ✅ Active   │  ChromaDB + MiniLM        ║
║  🗣️ Voice Engine        │  ✅ Ready    │  Orpheus TTS (v4.0)       ║
║  🔐 Auth System         │  ✅ Secure   │  JWT + 2FA + Revocation   ║
║  📱 Telegram Bot        │  ✅ Running  │  Admin Bridge Active      ║
║  🎛️ Admin Panel         │  ✅ Live     │  Full Dashboard           ║
║  🤖 Bot Builder         │  ✅ Active   │  Visual Config UI         ║
╚════════════════════════════════════════════════════════════════════╝
```

</div>

---

## 📖 Documentation

| Document | Description |
|:---|:---|
| [SECURITY.md](https://huggingface.co/spaces/AvinashAnalytics/avinash-chatbot/blob/main/SECURITY.md) | Authentication, 2FA, audit logs |
| [TTS_FALLBACK_README.md](https://huggingface.co/spaces/AvinashAnalytics/avinash-chatbot/blob/main/TTS_FALLBACK_README.md) | Voice engine configuration |
| [.env.example](https://huggingface.co/spaces/AvinashAnalytics/avinash-chatbot/blob/main/.env.example) | Environment variables template |

---

## 🔗 Connect

<div align="center">

[![Portfolio](https://img.shields.io/badge/🌐_Portfolio-avinashanalytics.github.io-00d4aa?style=for-the-badge)](https://avinashanalytics.github.io/)
[![LinkedIn](https://img.shields.io/badge/💼_LinkedIn-Avinash_Rai-0077b5?style=for-the-badge)](https://linkedin.com/in/AvinashAnalytics)
[![Telegram](https://img.shields.io/badge/📱_Telegram-@AvinashAnalytics-26A5E4?style=for-the-badge)](https://t.me/AvinashAnalytics_bot)
[![HuggingFace](https://img.shields.io/badge/🤗_HuggingFace-AvinashAnalytics-yellow?style=for-the-badge)](https://huggingface.co/AvinashAnalytics)

---

**Built with ❤️ and mass amounts of ☕ by [Avinash Rai](https://avinashanalytics.github.io)**

<sub>© 2024 Avinash Rai • All Digital Rights Reserved</sub>

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer"/>

</div>
```

