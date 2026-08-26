# 🌊 Phase 13 — Streaming

**Status:** 🔴 Not Started

## 🎯 Goal

Deliver real-time AI responses.

> 💡 Streaming is where async stops being optional. Revisit Phase 0.10 if needed.

## 🧭 Mental Model

```text
Agent → LLM → Stream → Application → User
```

## 📂 What lives in this folder

| Path | Contents |
|---|---|
| `notes/` | One markdown file per topic, using the notes template |
| `examples/` | Minimal working code — typed from memory, not copy-pasted |
| `practice/` | Deliberately broken code + the fix, and mini experiments |

**Suggested files in `examples/`:**

```text
01_stream_text.py
02_async_stream.py
03_stream_structured.py
04_stream_with_tools.py
```

## ✅ Topics to Cover

### 13.1 Streaming

- [ ] Why streaming?
- [ ] Text streaming
- [ ] Async streaming
- [ ] Partial responses
- [ ] Streaming events
- [ ] Structured output streaming
- [ ] Streaming with tools
- [ ] Streaming UI integration

## 🏁 Exit Criteria

> Tokens visibly appearing in my terminal or UI as the model generates them.

Only mark this phase 🟢 in [`DASHBOARD.md`](../DASHBOARD.md) once that is true.

## 🐛 Mistakes Log

| Date | What broke | Why | Fix |
|---|---|---|---|
| | | | |

---

[⬅️ Phase 12](../phase-12-messages-and-history/) · [📊 Dashboard](../DASHBOARD.md) · [Phase 14 ➡️](../phase-14-model-providers/)
