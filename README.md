# MR NOTHING

> For Hustlers. Dreamers. Builders.

[![License: MIT](https://img.shields.io/badge/License-MIT-gold.svg)](LICENSE)
[![Android](https://img.shields.io/badge/Android-Kotlin%20%2F%20Jetpack%20Compose-green.svg)](https://developer.android.com)
[![FastAPI](https://img.shields.io/badge/Backend-FastAPI%20%2F%20Python-blue.svg)](https://fastapi.tiangolo.com)
[![Status](https://img.shields.io/badge/Status-Building-gold.svg)]()
[![Stewardship](https://img.shields.io/badge/Stewardship-FCRI-purple.svg)](https://fcri.science)

**MR NOTHING** is an open-source Android-native agentic computing platform — built as a tribute to brotherhood, loyalty, and the belief that the greatest investment is in people.

This platform transforms your Android device from a passive digital tool into an intelligent execution partner.

---

## For Monichan and Rappi

This project is named for two brothers — known together as MR. The people who stand beside you when life collapses. Who pull you upward in your hardest moments. Who prove that the greatest empires are built through trust, relationships, and humans who refuse to let each other fall.

---

## Architecture

```
┌──────────────────────────────────────────────────┐
│                  ANDROID DEVICE                  │
│                                                  │
│  ┌────────────┐    ┌──────────────────────────┐  │
│  │   Voice    │    │      Jetpack Compose UI  │  │
│  │  Interface │    │  (Launcher / Dashboard)  │  │
│  └─────┬──────┘    └──────────┬───────────────┘  │
│        └─────────────┬────────┘                  │
│                      │                            │
│              ┌───────▼────────┐                  │
│              │  Agent Runtime │                  │
│              │  (Kotlin Core) │                  │
│              └───────┬────────┘                  │
│                      │                            │
│         ┌────────────▼─────────────┐             │
│         │    Task Planner          │             │
│         │  (Intent → Steps)        │             │
│         └────────────┬─────────────┘             │
└──────────────────────┼───────────────────────────┘
                       │  (HTTPS)
                       ▼
          ┌────────────────────────┐
          │  FastAPI Backend       │
          │  ├── Memory (Qdrant)   │
          │  ├── Voice (Whisper)   │
          │  ├── Worker agents     │
          │  └── Workflow engine   │
          └────────────────────────┘
```

---

## Stack

| Layer | Technology |
|-------|-----------|
| Android UI | Kotlin · Jetpack Compose |
| Agent Runtime | Kotlin coroutines |
| Backend API | FastAPI · Python 3.11+ |
| Memory | Qdrant (vector) + PostgreSQL |
| Voice | OpenAI Whisper (STT) + TTS |
| Realtime | Redis |
| Dashboard | Next.js · TypeScript |

---

## Repository Layout

```
MrNothing/
├── android/          Android app (Kotlin / Jetpack Compose)
│   └── app/src/main/kotlin/com/mrnothing/
│       ├── agent/    Core agent runtime
│       ├── core/     Task planning and intent handling
│       └── memory/   Memory store interface
├── backend/          FastAPI backend (Python)
├── dashboard/        Web dashboard (Next.js)
├── sdk/              MR NOTHING integration SDK
└── docs/             Architecture and integration docs
```

---

## Roadmap

| Phase | Focus | Status |
|-------|-------|--------|
| Phase 1 | Android MVP + Core agent loop | 🔨 Building |
| Phase 2 | Contextual memory + Task planner | 📋 Planned |
| Phase 3 | Voice intelligence | 📋 Planned |
| Phase 4 | Launcher integration + SDK | 📋 Planned |
| Phase 5 | Ecosystem + community marketplace | 📋 Planned |

---

## Quick Start (Backend)

```bash
git clone https://github.com/Davidcarmelalex/MrNothing
cd MrNothing/backend
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
cp .env.example .env
uvicorn main:app --reload
```

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Open source under [MIT License](LICENSE).  
Stewardship: [Fusion Civilization Research Institute (FCRI)](https://fcri.science).
