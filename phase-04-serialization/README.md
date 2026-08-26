# 🔄 Phase 04 — Pydantic Serialization

**Status:** 🔴 Not Started

## 🎯 Goal

Move data confidently between Python objects, dictionaries and JSON.

> 💡 Every API response, every LLM payload, every DB write crosses this boundary.

## 🧭 Mental Model

```text
dict → model_validate() → Model → model_dump() → dict → JSON
```

## 📂 What lives in this folder

| Path | Contents |
|---|---|
| `notes/` | One markdown file per topic, using the notes template |
| `examples/` | Minimal working code — typed from memory, not copy-pasted |
| `practice/` | Deliberately broken code + the fix, and mini experiments |

**Suggested files in `examples/`:**

```text
01_model_dump.py
02_model_dump_json.py
03_include_exclude.py
04_aliases.py
05_model_validate.py
06_round_trip.py
```

## ✅ Topics to Cover

### 4.1 Serialization

- [ ] model_dump()
- [ ] model_dump_json()
- [ ] include
- [ ] exclude
- [ ] Nested serialization
- [ ] Serialization aliases
- [ ] Custom serializers

### 4.2 Deserialization

- [ ] model_validate()
- [ ] model_validate_json()
- [ ] Validate dicts
- [ ] Validate JSON strings
- [ ] Validate model instances

## 🏁 Exit Criteria

> I can round-trip a nested model to JSON and back with no data loss, and exclude a secret field on the way out.

Only mark this phase 🟢 in [`DASHBOARD.md`](../DASHBOARD.md) once that is true.

## 🐛 Mistakes Log

| Date | What broke | Why | Fix |
|---|---|---|---|
| | | | |

---

[⬅️ Phase 03](../phase-03-validation/) · [📊 Dashboard](../DASHBOARD.md) · [Phase 05 ➡️](../phase-05-advanced-pydantic/)
