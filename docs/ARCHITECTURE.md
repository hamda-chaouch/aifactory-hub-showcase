# AIFactory Hub — High-Level Architecture

This document describes the architectural vision at a high level.
Detailed implementation is proprietary.

---

## Layers

| Layer | Purpose | Visibility |
| :--- | :--- | :--- |
| **QML Frontend** | User interface | Public (this doc) |
| **UI Shell** | Module registry, theming, bridge | Public (concept) |
| **Modules** | 4 workspaces | Public (concept) |
| **Engines** | Local processing (Whisper, FFmpeg) | Public (names) |
| **AI Contracts** | Provider-independent interfaces | Concept public, code private |
| **Gateway** | Facade for external systems | Concept public |
| **Integrations** | Ollama, Gemini, ComfyUI, YouTube, Telegram | Public (names) |
| **Core** | Config, logging, storage, events | Concept public |

---

## Communication Model

| Need | Mechanism |
| :--- | :--- |
| External operation | Gateway (composition) + injected contract (runtime) |
| Local technical operation | Engine |
| Internal cross-module request | Service contract |
| "Something happened" | EventBus |

---

## Design Principles

1. **Dependency direction** — Higher-level components depend on lower-level contracts.
2. **AI contracts are compile-time only** — Not runtime layers.
3. **Hybrid AI** — Local-first with cloud fallback.
4. **DI over singletons** — Constructor injection preferred.
5. **EventBus for events, contracts for requests** — No module imports another module.
6. **Secrets in OS keychain** — Never in config files.
7. **Data discipline** — `raw/` immutable · `assets/` reusable · `cache/` reconstructible.
8. **UI thread responsive** — Long operations run off the main thread.

---

## Hybrid AI Routing
Simple tasks → Local (Ollama · Qwen · fast, private)
Complex tasks → Cloud (Gemini · powerful, requires internet)
Fallback → Auto (if local fails, route to cloud)

Full details are proprietary.

---

*For licensing inquiries: see [`../contact/`](../contact/).*