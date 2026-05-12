# Contributing to MR NOTHING

MR NOTHING is an open-source project built on the belief that the best technology is built by people who care about people.

## What We're Building

An Android-native AI agent that:
- Understands natural language (text + voice)
- Plans and executes multi-step tasks
- Remembers context across sessions
- Runs natively on your device

## How to Contribute

1. Fork the repo and create a branch: `git checkout -b feat/your-feature`
2. Write code with clear comments and type hints (Kotlin or Python)
3. Add tests
4. Open a PR with a clear description of what you built and why

## Contribution Areas

| Area | Skills Needed | Priority |
|------|--------------|---------|
| Android agent runtime | Kotlin, Coroutines | 🔴 High |
| Voice STT/TTS | Python, Whisper | 🔴 High |
| Memory layer | Python, Qdrant | 🟡 Medium |
| Task planner | Kotlin / Python | 🟡 Medium |
| Dashboard UI | TypeScript, Next.js | 🟢 Normal |
| SDK | Kotlin / Python | 🟢 Normal |

## Commit Convention

```
feat(android): add voice wake word detection
feat(backend): implement contextual memory search
fix(planner): resolve intent classification edge case
docs: update Android setup guide
test(memory): add vector search unit tests
```

## Code of Conduct

This project was built in the spirit of loyalty, respect, and shared purpose. Be kind. Be honest. Lift others up.
