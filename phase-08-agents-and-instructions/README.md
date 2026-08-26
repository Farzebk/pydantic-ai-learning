# 🧑‍💻 Phase 08 — Agents & Instructions

**Status:** 🔴 Not Started

## 🎯 Goal

Build and control PydanticAI agents.

> 💡 First real agent. Keep the API key in `.env` from day one — never in a committed file.

## 🧭 Mental Model

```text
User → Agent → Model → LLM → Response
```

## 📂 What lives in this folder

| Path | Contents |
|---|---|
| `notes/` | One markdown file per topic, using the notes template |
| `examples/` | Minimal working code — typed from memory, not copy-pasted |
| `practice/` | Deliberately broken code + the fix, and mini experiments |

**Suggested files in `examples/`:**

```text
01_first_agent.py
02_static_instructions.py
03_dynamic_instructions.py
04_result_object.py
.env.example
```

## ✅ Topics to Cover

### 8.1 First Agent

- [ ] Install PydanticAI
- [ ] Configure environment
- [ ] Configure API key
- [ ] Select a model
- [ ] Create an Agent
- [ ] Add instructions
- [ ] Run the agent
- [ ] Read the response
- [ ] Understand the result object

### 8.2 Agent Instructions

- [ ] Static instructions
- [ ] System prompts
- [ ] Agent instructions
- [ ] Dynamic instructions
- [ ] Instruction functions
- [ ] Runtime context in instructions
- [ ] Reusable instructions
- [ ] Instruction design

### 8.3 Agent Lifecycle

- [ ] Agent creation
- [ ] Run
- [ ] Model request
- [ ] Tool execution
- [ ] Output validation
- [ ] Final result
- [ ] Error handling

## 🏁 Exit Criteria

> A working agent running from my own script, with instructions I wrote myself.

Only mark this phase 🟢 in [`DASHBOARD.md`](../DASHBOARD.md) once that is true.

## 🐛 Mistakes Log

| Date | What broke | Why | Fix |
|---|---|---|---|
| | | | |

---

[⬅️ Phase 07](../phase-07-pydanticai-fundamentals/) · [📊 Dashboard](../DASHBOARD.md) · [Phase 09 ➡️](../phase-09-structured-output/)
