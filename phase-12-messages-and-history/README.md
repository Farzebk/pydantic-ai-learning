# 💬 Phase 12 — Messages & Conversation History

**Status:** 🔴 Not Started

## 🎯 Goal

Build agents that understand and maintain conversation context.

> 💡 History is just a list you pass in. The hard part is deciding what to keep.

## 🧭 Mental Model

```text
User → Message → Agent → Response → History → Next Message → Agent + History
```

## 📂 What lives in this folder

| Path | Contents |
|---|---|
| `notes/` | One markdown file per topic, using the notes template |
| `examples/` | Minimal working code — typed from memory, not copy-pasted |
| `practice/` | Deliberately broken code + the fix, and mini experiments |

**Suggested files in `examples/`:**

```text
01_message_types.py
02_multi_turn.py
03_passing_history.py
04_persisting_history.py
05_trimming_context.py
```

## ✅ Topics to Cover

### 12.1 Messages

- [ ] User messages
- [ ] Assistant messages
- [ ] Tool messages
- [ ] Model messages
- [ ] Message structure
- [ ] Message history

### 12.2 Conversation

- [ ] Single-turn agent
- [ ] Multi-turn agent
- [ ] Reusing history
- [ ] Passing previous messages
- [ ] Persistent history
- [ ] Context management
- [ ] History storage

## 🏁 Exit Criteria

> A conversation where turn 3 correctly references something said in turn 1.

Only mark this phase 🟢 in [`DASHBOARD.md`](../DASHBOARD.md) once that is true.

## 🐛 Mistakes Log

| Date | What broke | Why | Fix |
|---|---|---|---|
| | | | |

---

[⬅️ Phase 11](../phase-11-tools/) · [📊 Dashboard](../DASHBOARD.md) · [Phase 13 ➡️](../phase-13-streaming/)
