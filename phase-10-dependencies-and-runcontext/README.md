# 🔌 Phase 10 — Dependencies & RunContext

**Status:** 🔴 Not Started

## 🎯 Goal

Supply application data to an agent at runtime.

> 💡 Without this, agents are stateless toys. With it, they know who the user is.

## 🧭 Mental Model

```text
Application → Dependencies → RunContext → Agent → Instructions / Tools
```

## 📂 What lives in this folder

| Path | Contents |
|---|---|
| `notes/` | One markdown file per topic, using the notes template |
| `examples/` | Minimal working code — typed from memory, not copy-pasted |
| `practice/` | Deliberately broken code + the fix, and mini experiments |

**Suggested files in `examples/`:**

```text
01_simple_dependency.py
02_dataclass_deps.py
03_deps_in_instructions.py
04_deps_in_tools.py
05_db_dependency.py
```

## ✅ Topics to Cover

### 10.1 Dependencies

- [ ] What dependencies are
- [ ] Dependency injection
- [ ] Agent dependencies
- [ ] Runtime dependencies
- [ ] Dynamic dependencies
- [ ] Database dependencies
- [ ] API dependencies
- [ ] User dependencies
- [ ] Configuration dependencies

### 10.2 RunContext

- [ ] Understanding RunContext
- [ ] Accessing dependencies
- [ ] Context in instructions
- [ ] Context in tools
- [ ] Runtime state
- [ ] Context lifecycle

## 🏁 Exit Criteria

> An agent whose instructions change based on injected user data.

Only mark this phase 🟢 in [`DASHBOARD.md`](../DASHBOARD.md) once that is true.

## 🐛 Mistakes Log

| Date | What broke | Why | Fix |
|---|---|---|---|
| | | | |

---

[⬅️ Phase 09](../phase-09-structured-output/) · [📊 Dashboard](../DASHBOARD.md) · [Phase 11 ➡️](../phase-11-tools/)
