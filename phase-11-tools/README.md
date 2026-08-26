# 🔧 Phase 11 — Tools & Tool Calling

**Status:** 🔴 Not Started

## 🎯 Goal

Give agents the ability to perform real-world actions.

> 💡 Tool descriptions are prompts. Write them like documentation for a colleague.

## 🧭 Mental Model

```text
Agent → Tool → Python Function → Result → Agent
```

## 📂 What lives in this folder

| Path | Contents |
|---|---|
| `notes/` | One markdown file per topic, using the notes template |
| `examples/` | Minimal working code — typed from memory, not copy-pasted |
| `practice/` | Deliberately broken code + the fix, and mini experiments |

**Suggested files in `examples/`:**

```text
01_first_tool.py
02_multiple_tools.py
03_tools_with_context.py
04_tool_errors.py
05_retryable_tools.py
```

## ✅ Topics to Cover

### 11.1 Basic Tools

- [ ] Define a tool
- [ ] Tool description
- [ ] Tool arguments
- [ ] Tool return values
- [ ] Multiple tools
- [ ] How the model selects a tool

### 11.2 Tool Context

- [ ] Tool context
- [ ] RunContext inside tools
- [ ] Dependencies inside tools
- [ ] Runtime data
- [ ] Tool metadata

### 11.3 Tool Errors

- [ ] Tool exceptions
- [ ] Validation errors
- [ ] Retryable errors
- [ ] Non-retryable errors
- [ ] Graceful failures

### 11.4 Practice Tools

- [ ] Calculator
- [ ] Weather
- [ ] Search
- [ ] Database
- [ ] User lookup
- [ ] API request
- [ ] File search
- [ ] Email
- [ ] Calendar

## 🏁 Exit Criteria

> An agent that picks correctly between three tools, and recovers cleanly when one raises.

Only mark this phase 🟢 in [`DASHBOARD.md`](../DASHBOARD.md) once that is true.

## 🐛 Mistakes Log

| Date | What broke | Why | Fix |
|---|---|---|---|
| | | | |

---

[⬅️ Phase 10](../phase-10-dependencies-and-runcontext/) · [📊 Dashboard](../DASHBOARD.md) · [Phase 12 ➡️](../phase-12-messages-and-history/)
