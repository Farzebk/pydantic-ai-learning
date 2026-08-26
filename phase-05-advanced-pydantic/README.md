# 🧬 Phase 05 — Advanced Pydantic

**Status:** 🔴 Not Started

## 🎯 Goal

Go beyond basic models into configuration, custom types and generics.

> 💡 This is what separates 'I used Pydantic' from 'I designed the data layer'.

## 📂 What lives in this folder

| Path | Contents |
|---|---|
| `notes/` | One markdown file per topic, using the notes template |
| `examples/` | Minimal working code — typed from memory, not copy-pasted |
| `practice/` | Deliberately broken code + the fix, and mini experiments |

**Suggested files in `examples/`:**

```text
01_config_dict.py
02_extra_fields.py
03_strict_mode.py
04_annotated_custom_types.py
05_generic_models.py
06_computed_fields.py
```

## ✅ Topics to Cover

### 5.1 Configuration

- [ ] ConfigDict
- [ ] Extra fields: ignore / forbid / allow
- [ ] Strict mode
- [ ] validate_assignment
- [ ] validate_default
- [ ] Alias configuration
- [ ] Serialization configuration

### 5.2 Custom Types

- [ ] Custom validation functions
- [ ] Reusable validation
- [ ] Annotated
- [ ] AfterValidator
- [ ] BeforeValidator
- [ ] Fully custom types

### 5.3 Generics

- [ ] TypeVar
- [ ] Generic models
- [ ] Generic API responses — Response[User], Response[Order]
- [ ] Generic validation

### 5.4 Computed Fields

- [ ] computed_field
- [ ] Derived values
- [ ] Serializing computed fields

### 5.5 Advanced Model Features

- [ ] Model copying
- [ ] Model rebuilding
- [ ] Model inspection
- [ ] Model metadata
- [ ] Custom schema behavior

## 🏁 Exit Criteria

> I've built one reusable `Annotated` type and one generic `Response[T]` wrapper used in two different places.

Only mark this phase 🟢 in [`DASHBOARD.md`](../DASHBOARD.md) once that is true.

## 🐛 Mistakes Log

| Date | What broke | Why | Fix |
|---|---|---|---|
| | | | |

---

[⬅️ Phase 04](../phase-04-serialization/) · [📊 Dashboard](../DASHBOARD.md) · [Phase 06 ➡️](../phase-06-json-schema/)
