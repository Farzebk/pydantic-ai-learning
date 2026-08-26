# 🔁 Phase 15 — Retries & Error Handling

**Status:** 🔴 Not Started

## 🎯 Goal

Build agents that don't collapse under real conditions.

> 💡 LLM calls fail. Networks fail. Output is malformed. Plan for all three.

## 📂 What lives in this folder

| Path | Contents |
|---|---|
| `notes/` | One markdown file per topic, using the notes template |
| `examples/` | Minimal working code — typed from memory, not copy-pasted |
| `practice/` | Deliberately broken code + the fix, and mini experiments |

**Suggested files in `examples/`:**

```text
01_error_types.py
02_output_retries.py
03_tool_retries.py
04_backoff.py
05_graceful_degradation.py
```

## ✅ Topics to Cover

### 15.1 Agent Errors

- [ ] Model errors
- [ ] API errors
- [ ] Timeout errors
- [ ] Validation errors
- [ ] Tool errors
- [ ] Output errors

### 15.2 Retries

- [ ] Retry concepts
- [ ] Retrying validation
- [ ] Retrying tools
- [ ] Retrying model calls
- [ ] Retry limits
- [ ] Backoff strategies

### 15.3 Reliability

- [ ] Timeouts
- [ ] Fallbacks
- [ ] Graceful degradation
- [ ] Error reporting
- [ ] Recovery strategies

## 🏁 Exit Criteria

> An agent that retries a failed validation and reports cleanly when retries run out.

Only mark this phase 🟢 in [`DASHBOARD.md`](../DASHBOARD.md) once that is true.

## 🐛 Mistakes Log

| Date | What broke | Why | Fix |
|---|---|---|---|
| | | | |

---

[⬅️ Phase 14](../phase-14-model-providers/) · [📊 Dashboard](../DASHBOARD.md) · [Phase 16 ➡️](../phase-16-multi-agent/)
