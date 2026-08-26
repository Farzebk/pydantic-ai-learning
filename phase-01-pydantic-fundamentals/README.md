# 🧱 Phase 01 — Pydantic Fundamentals

**Status:** 🟡 In Progress ← current

## 🎯 Goal

Understand what Pydantic is, why it exists, and how it turns raw data into validated Python objects.

> 💡 Everything else in this repo is a variation on `BaseModel`. Get this one properly solid.

## 🧭 Mental Model

```text
Pydantic → Data Validation → Structured Python Data → JSON Schema → Structured AI Output → PydanticAI
```

## 📂 What lives in this folder

| Path | Contents |
|---|---|
| `notes/` | One markdown file per topic, using the notes template |
| `examples/` | Minimal working code — typed from memory, not copy-pasted |
| `practice/` | Deliberately broken code + the fix, and mini experiments |

**Suggested files in `examples/`:**

```text
01_basemodel_basics.py
02_required_vs_optional.py
03_defaults.py
04_nested_models.py
05_lists_and_dicts_of_models.py
06_recursive_models.py
07_model_inheritance.py
```

## ✅ Topics to Cover

### 1.1 Pydantic vs PydanticAI ✅

- [x] What Pydantic is
- [x] What PydanticAI is
- [x] How they relate
- [x] Why Pydantic matters for AI
- [x] Structured data
- [x] Data validation

### 1.2 BaseModel ✅

- [x] Import BaseModel
- [x] Create a basic model
- [x] Define fields
- [x] Instantiate
- [x] Access fields
- [x] Modify fields
- [x] How validation fires
- [x] Reading ValidationError
- [x] BaseModel vs a normal class

### 1.3 Model Fundamentals 🔄

- [ ] Required fields
- [ ] Optional fields
- [ ] Default values
- [ ] Nested models
- [ ] Lists of models
- [ ] Dicts of models
- [ ] Recursive models
- [ ] Model inheritance
- [ ] Model inspection

## 🏁 Exit Criteria

> I can write a nested model from memory, trigger a `ValidationError` on purpose, and read the error output correctly.

Only mark this phase 🟢 in [`DASHBOARD.md`](../DASHBOARD.md) once that is true.

## 🐛 Mistakes Log

| Date | What broke | Why | Fix |
|---|---|---|---|
| | | | |

---

[⬅️ Phase 00](../phase-00-python-foundations/) · [📊 Dashboard](../DASHBOARD.md) · [Phase 02 ➡️](../phase-02-models-and-types/)
