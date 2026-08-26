# 📐 Phase 06 — JSON Schema & Structured Data

**Status:** 🔴 Not Started

## 🎯 Goal

Understand the bridge between Pydantic and structured AI output.

> 💡 **This is the hinge of the entire repo.** Everything before it is Pydantic; everything after it is AI. This phase is what connects them.

## 🧭 Mental Model

```text
Pydantic Model → JSON Schema → Expected Structure → AI Output → Pydantic Validation
```

## 📂 What lives in this folder

| Path | Contents |
|---|---|
| `notes/` | One markdown file per topic, using the notes template |
| `examples/` | Minimal working code — typed from memory, not copy-pasted |
| `practice/` | Deliberately broken code + the fix, and mini experiments |

**Suggested files in `examples/`:**

```text
01_model_json_schema.py
02_constraints_in_schema.py
03_descriptions_matter.py
04_nested_schema.py
05_schema_to_llm_prompt.py
```

## ✅ Topics to Cover

### 6.1 JSON Schema

- [ ] What JSON Schema is
- [ ] Why it exists
- [ ] model_json_schema()
- [ ] Schema properties
- [ ] Required fields in schema
- [ ] Nested schemas
- [ ] Constraints in schema
- [ ] Descriptions in schema
- [ ] Schema generation rules

### 6.2 The AI Connection

- [ ] Why LLM output is unpredictable
- [ ] Why structured output matters
- [ ] How schemas describe expected output
- [ ] How Pydantic validates AI responses
- [ ] Why this matters in PydanticAI

## 🏁 Exit Criteria

> I can look at a model and predict its generated schema, including exactly how `description=` shows up.

Only mark this phase 🟢 in [`DASHBOARD.md`](../DASHBOARD.md) once that is true.

## 🐛 Mistakes Log

| Date | What broke | Why | Fix |
|---|---|---|---|
| | | | |

---

[⬅️ Phase 05](../phase-05-advanced-pydantic/) · [📊 Dashboard](../DASHBOARD.md) · [Phase 07 ➡️](../phase-07-pydanticai-fundamentals/)
