# 🤝 Phase 16 — Multi-Agent Systems

**Status:** 🔴 Not Started

## 🎯 Goal

Make specialized agents collaborate.

> 💡 Structured output (Phase 9) is what makes agent-to-agent communication reliable.

## 🧭 Mental Model

```text
User → Manager → [Research Agent | Coding Agent | Review Agent]
```

## 📂 What lives in this folder

| Path | Contents |
|---|---|
| `notes/` | One markdown file per topic, using the notes template |
| `examples/` | Minimal working code — typed from memory, not copy-pasted |
| `practice/` | Deliberately broken code + the fix, and mini experiments |

**Suggested files in `examples/`:**

```text
01_two_agents.py
02_delegation.py
03_manager_worker.py
04_router_pattern.py
05_reviewer_pattern.py
06_parallel_agents.py
```

## ✅ Topics to Cover

### 16.1 Multi-Agent Concepts

- [ ] Multiple agents
- [ ] Specialized agents
- [ ] Agent delegation
- [ ] Agent handoffs
- [ ] Agent orchestration
- [ ] Agent communication
- [ ] Shared dependencies
- [ ] Structured communication
- [ ] Result passing
- [ ] Manager agents
- [ ] Worker agents

### 16.2 Multi-Agent Patterns

- [ ] Sequential agents
- [ ] Parallel agents
- [ ] Manager/worker
- [ ] Router pattern
- [ ] Reviewer pattern
- [ ] Research → analysis → report
- [ ] Human-in-the-loop

## 🏁 Exit Criteria

> A manager agent that routes to at least two workers and merges their structured results.

Only mark this phase 🟢 in [`DASHBOARD.md`](../DASHBOARD.md) once that is true.

## 🐛 Mistakes Log

| Date | What broke | Why | Fix |
|---|---|---|---|
| | | | |

---

[⬅️ Phase 15](../phase-15-retries-and-errors/) · [📊 Dashboard](../DASHBOARD.md) · [Phase 17 ➡️](../phase-17-testing-and-evaluation/)
