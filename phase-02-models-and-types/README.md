# 🏷️ Phase 02 — Pydantic Models & Types

**Status:** 🔴 Not Started

## 🎯 Goal

Model complex, strongly typed real-world data comfortably.

> 💡 This is where you stop writing `if not isinstance(...)` by hand.

## 📂 What lives in this folder

| Path | Contents |
|---|---|
| `notes/` | One markdown file per topic, using the notes template |
| `examples/` | Minimal working code — typed from memory, not copy-pasted |
| `practice/` | Deliberately broken code + the fix, and mini experiments |

**Suggested files in `examples/`:**

```text
01_field_basics.py
02_field_constraints.py
03_basic_and_collection_types.py
04_union_and_optional.py
05_special_types.py
06_pydantic_types.py
07_nested_models.py
```

## ✅ Topics to Cover

### 2.1 Field()

- [ ] default
- [ ] default_factory
- [ ] title
- [ ] description
- [ ] alias
- [ ] examples
- [ ] gt / ge / lt / le
- [ ] multiple_of
- [ ] min_length / max_length
- [ ] pattern

### 2.2 Basic Types

- [ ] str
- [ ] int
- [ ] float
- [ ] bool
- [ ] None

### 2.3 Collection Types

- [ ] list
- [ ] dict
- [ ] tuple
- [ ] set
- [ ] frozenset

### 2.4 Union & Optional

- [ ] Optional
- [ ] Union
- [ ] Modern | syntax
- [ ] str | None
- [ ] str | int

### 2.5 Special Types

- [ ] Literal
- [ ] Enum
- [ ] UUID
- [ ] datetime
- [ ] date
- [ ] time
- [ ] timedelta
- [ ] Decimal

### 2.6 Pydantic Types

- [ ] EmailStr
- [ ] URL types
- [ ] Network types
- [ ] Secret types
- [ ] File-related types

### 2.7 Nested Models

- [ ] Basic nesting
- [ ] Multiple nested models
- [ ] Lists of models
- [ ] Dicts of models
- [ ] Optional nested models
- [ ] Deeply nested structures
- [ ] Recursive models
- [ ] Nested validation behavior

## 🏁 Exit Criteria

> I can model an *order with line items and a customer* in one sitting, using field constraints instead of manual checks.

Only mark this phase 🟢 in [`DASHBOARD.md`](../DASHBOARD.md) once that is true.

## 🐛 Mistakes Log

| Date | What broke | Why | Fix |
|---|---|---|---|
| | | | |

---

[⬅️ Phase 01](../phase-01-pydantic-fundamentals/) · [📊 Dashboard](../DASHBOARD.md) · [Phase 03 ➡️](../phase-03-validation/)
