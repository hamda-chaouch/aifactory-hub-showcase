# 🏭 AIFactory Hub

![Status](https://img.shields.io/badge/Status-Phase%201%20In%20Progress-blue)
![License](https://img.shields.io/badge/License-Proprietary-red)
![Qt](https://img.shields.io/badge/Qt-6.8.1-green)
![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20macOS-lightgrey)

**🌐 Live Showcase:** [hamda-chaouch.github.io/aifactory-hub-showcase](https://hamda-chaouch.github.io/aifactory-hub-showcase/)

**Development Engineering AI Suite** — A unified Qt 6 + QML desktop platform
for AI-powered content creation, data analysis, engineering, and coding automation.

> ⚠️ **Source code is proprietary.** This repository contains documentation
> and screenshots only. For licensing inquiries, see [contact/](contact/).

---

## 🎯 Vision

Most AI tools today are fragmented: one app for video, one for images,
one for coding, one for documents. AIFactory Hub unifies them into a single,
hybrid (local + cloud) desktop platform.

**One Platform. Infinite Possibilities.**

---

## 📦 Modules

| Module | Mission |
| :--- | :--- |
| 🎨 **AI Media Studio** | Auto Content Factory · Manual Content Factory<br>Images · Videos · 3D |
| 📊 **Data & Knowledge Studio** | Documents · PDF · RAG<br>Statistics · Analysis · Research |
| ⚙️ **Engineering Studio** | PCB · CAD · Robotics<br>Code · Architecture · Datasheets |
| 🤖 **Hamda Agent** | AI Coding & Automation Agent<br>Plan · Code · Build · Test · Document · Deploy |

---

## 🏗️ High-Level Architecture
QML FRONTEND
│
▼
UI SHELL
│
▼
MODULES
/
▼ ▼
ENGINES AI CONTRACTS
│ │
▼ ▼
Core PROVIDERS
│
▼
Local + Cloud AI
(Ollama · Gemini · ComfyUI)


**Key features:**
- **Hybrid AI** — local models (Ollama) + cloud (Gemini) with automatic routing
- **Modular** — 4 independent workspaces in one shell
- **Private by default** — your data stays local when possible
- **Extensible** — designed for plugins and community modules

Full architecture: [`docs/ARCHITECTURE.md`](docs/ARCHITECTURE.md).

---

## 🛠️ Technology Stack

| Layer | Technology |
| :--- | :--- |
| **UI** | Qt 6 + QML |
| **Backend** | C++17 |
| **Local AI** | Ollama (Qwen, Gemma, DeepSeek) |
| **Cloud AI** | Google Gemini |
| **Image/Video Gen** | ComfyUI, SDXL, Wan |
| **Transcription** | whisper.cpp |
| **Media Processing** | FFmpeg |
| **Platforms** | Windows (primary), Linux, macOS |

---

## 📅 Development Status

| Phase | Deliverable | Status |
| :--- | :--- | :--- |
| **Phase 1** | Shell + Core Foundation | 🚧 In Progress |
| **Phase 2** | AI Media Studio — Auto Content Factory | ⏳ Pending |
| **Phase 3** | WhisperEngine → Transcriber | ⏳ Pending |
| **Phase 4** | Gateway + Gemini → Highlight Detection | ⏳ Pending |
| **Phase 5** | FFmpeg pipeline (Cut · SRT · Burn) | ⏳ Pending |
| **Phase 6** | Publishing (Telegram + YouTube) | ⏳ Pending |
| **Phase 7–9** | Manual Image / Video / 3D Tools | ⏳ Pending |
| **Phase 10** | Data & Knowledge + Engineering Studios | ⏳ Pending |
| **Phase 11** | Hamda Agent | ⏳ Pending |

Full roadmap: [`docs/ROADMAP.md`](docs/ROADMAP.md).

---

## 📸 Screenshots

*Screenshots will be added here as the UI is built.*

| Home | AI Media Studio |
| :---: | :---: |
| *(coming soon)* | *(coming soon)* |

---

## 💼 Business Model

AIFactory Hub operates under a **revenue-share contributor model**.

- **Primary production module:** Content Factory
- **Commercial licensing available** for enterprise use
- **Contributors** earn revenue share on the code they help build

See [`CONTRIBUTORS.md`](CONTRIBUTORS.md) and [`contact/`](contact/) for details.

---

## 📬 Contact

| Purpose | Contact |
| :--- | :--- |
| **Licensing inquiries** | See [`contact/`](contact/) |
| **Contributor applications** | See [`CONTRIBUTORS.md`](CONTRIBUTORS.md) |
| **Press / media** | See [`contact/`](contact/) |

---

## 📄 License

**Proprietary.** All Rights Reserved.
See [`LICENSE`](LICENSE) for full terms.

---

*Built with Qt 6, C++17, and a hybrid local-first AI philosophy.*