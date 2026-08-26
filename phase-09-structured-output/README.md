# 📦 Phase 09 — Structured AI Output

**Status:** 🔴 Not Started

## 🎯 Goal

Make AI responses predictable, validated and type-safe.

> 💡 The payoff phase — Phases 1–6 exist to make this one work.

## 🧭 Mental Model

```text
User → Agent → LLM → Structured Output → Pydantic Model → Validation → Application
```

## 📂 What lives in this folder

| Path | Contents |
|---|---|
| `notes/` | One markdown file per topic, using the notes template |
| `examples/` | Minimal working code — typed from memory, not copy-pasted |
| `practice/` | Deliberately broken code + the fix, and mini experiments |

**Suggested files in `examples/`:**

```text
01_text_vs_structured.py
02_simple_output_model.py
03_nested_output.py
04_list_output.py
05_output_retries.py
```

## ✅ Topics to Cover

### 9.1 Output Models

- [ ] Text output
- [ ] Pydantic output
- [ ] Simple output model
- [ ] Nested output model
- [ ] Lists of models
- [ ] Complex structured output
- [ ] Output validation
- [ ] Invalid output handling
- [ ] Output retries

### 9.2 Practice Projects

- [ ] Resume parser
- [ ] Movie recommendation agent
- [ ] Product information extractor
- [ ] Invoice extractor
- [ ] Generic JSON extraction agent

## 🏁 Exit Criteria

> An agent that returns a validated nested model, and recovers when the LLM returns something malformed.

Only mark this phase 🟢 in [`DASHBOARD.md`](../DASHBOARD.md) once that is true.

## 🐛 Mistakes Log

| Date | What broke | Why | Fix |
|---|---|---|---|
| | | | |

---

[⬅️ Phase 08](../phase-08-agents-and-instructions/) · [📊 Dashboard](../DASHBOARD.md) · [Phase 10 ➡️](../phase-10-dependencies-and-runcontext/)
