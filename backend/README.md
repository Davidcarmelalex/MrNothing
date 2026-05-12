# MrNothing Backend

FastAPI backend powering the MrNothing agent platform.

## Stack
- FastAPI + Python 3.11+
- Qdrant (vector memory)
- PostgreSQL
- Redis
- Whisper (voice STT)

## Quick Start
```bash
pip install -r ../requirements.txt
cp ../.env.example .env
uvicorn main:app --reload
```
