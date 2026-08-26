# 🛡️ Phase 03 — Pydantic Validation

**Status:** 🔴 Not Started

## 🎯 Goal

Control how Pydantic validates, transforms and rejects data.

> 💡 Validators are where business rules live — and where AI output gets rejected before it reaches your app.

## 📂 What lives in this folder

| Path | Contents |
|---|---|
| `notes/` | One markdown file per topic, using the notes template |
| `examples/` | Minimal working code — typed from memory, not copy-pasted |
| `practice/` | Deliberately broken code + the fix, and mini experiments |

**Suggested files in `examples/`:**

```text
01_basic_validation.py
02_field_validator_before.py
03_field_validator_after.py
04_model_validator.py
05_cross_field_validation.py
06_custom_errors.py
```

## ✅ Topics to Cover

### 3.1 Basic Validation

- [ ] Type validation
- [ ] Required field validation
- [ ] Default value validation
- [ ] Constraint validation
- [ ] Nested validation
- [ ] Reading validation errors

### 3.2 Field Validators

- [ ] field_validator
- [ ] mode='before'
- [ ] mode='after'
- [ ] Validating multiple fields
- [ ] Validation ordering
- [ ] Custom error messages

### 3.3 Model Validators

- [ ] model_validator
- [ ] mode='before'
- [ ] mode='after'
- [ ] Cross-field validation
- [ ] Complex validation logic

### 3.4 Validation Practice

- [ ] User registration validator
- [ ] Password validator
- [ ] Product validator
- [ ] Order validator
- [ ] Payment validator

## 🏁 Exit Criteria

> I can write a cross-field validator (e.g. `password == confirm_password`) without looking it up.

Only mark this phase 🟢 in [`DASHBOARD.md`](../DASHBOARD.md) once that is true.

## 🐛 Mistakes Log

| Date | What broke | Why | Fix |
|---|---|---|---|
| | | | |

---

[⬅️ Phase 02](../phase-02-models-and-types/) · [📊 Dashboard](../DASHBOARD.md) · [Phase 04 ➡️](../phase-04-serialization/)
