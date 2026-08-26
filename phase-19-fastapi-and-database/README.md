# ⚡ Phase 19 — FastAPI & Database Integration

**Status:** 🔴 Not Started

## 🎯 Goal

Turn PydanticAI agents into real backend applications.

> 💡 FastAPI is built on Pydantic — by this point the request/response models will feel familiar.

## 🧭 Mental Model

```text
Client → FastAPI → Pydantic → PydanticAI → LLM → Structured Response → Client
```

## 📂 What lives in this folder

| Path | Contents |
|---|---|
| `notes/` | One markdown file per topic, using the notes template |
| `examples/` | Minimal working code — typed from memory, not copy-pasted |
| `practice/` | Deliberately broken code + the fix, and mini experiments |

**Suggested files in `examples/`:**

```text
app/main.py
app/routes/
app/models/
app/agents/
app/db/
01_async_basics.py
02_first_endpoint.py
03_agent_endpoint.py
04_streaming_endpoint.py
```

## ✅ Topics to Cover

### 19.1 Async Python

- [ ] async
- [ ] await
- [ ] asyncio
- [ ] Async functions
- [ ] Async API calls
- [ ] Async tools
- [ ] Concurrent tasks
- [ ] Async database calls
- [ ] Async FastAPI
- [ ] Streaming with async

### 19.2 FastAPI

- [ ] FastAPI basics
- [ ] Routes
- [ ] Request models
- [ ] Response models
- [ ] Dependency injection
- [ ] Async endpoints
- [ ] Agent endpoints
- [ ] Streaming endpoints
- [ ] Error handling
- [ ] Authentication
- [ ] API documentation

### 19.3 PostgreSQL

- [ ] SQL basics
- [ ] PostgreSQL
- [ ] Tables
- [ ] Queries
- [ ] Relationships
- [ ] Indexes
- [ ] Transactions
- [ ] Connection pooling
- [ ] Async database
- [ ] ORM

### 19.4 Database + PydanticAI

- [ ] Database dependencies
- [ ] Database tools
- [ ] Query agent
- [ ] Structured database results
- [ ] Natural language → SQL
- [ ] SQL validation
- [ ] Query execution
- [ ] Database security

## 🏁 Exit Criteria

> A `POST /agent` endpoint returning a validated model, backed by real database reads.

Only mark this phase 🟢 in [`DASHBOARD.md`](../DASHBOARD.md) once that is true.

## 🐛 Mistakes Log

| Date | What broke | Why | Fix |
|---|---|---|---|
| | | | |

---

[⬅️ Phase 18](../phase-18-observability/) · [📊 Dashboard](../DASHBOARD.md) · [Phase 20 ➡️](../phase-20-security-and-production/)
