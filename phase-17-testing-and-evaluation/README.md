# 🧪 Phase 17 — Testing & Evaluation

**Status:** 🔴 Not Started

## 🎯 Goal

Stop manually eyeballing every response.

> 💡 Tests should run without hitting a real LLM. Mock the model; test your logic.

## 📂 What lives in this folder

| Path | Contents |
|---|---|
| `notes/` | One markdown file per topic, using the notes template |
| `examples/` | Minimal working code — typed from memory, not copy-pasted |
| `practice/` | Deliberately broken code + the fix, and mini experiments |

**Suggested files in `examples/`:**

```text
test_models.py
test_validators.py
test_agents.py
test_tools.py
conftest.py
evals/dataset.json
```

## ✅ Topics to Cover

### 17.1 Python Testing

- [ ] pytest
- [ ] Unit tests
- [ ] Integration tests
- [ ] Fixtures
- [ ] Mocking
- [ ] Async testing

### 17.2 Pydantic Testing

- [ ] Model validation tests
- [ ] Validator tests
- [ ] Serialization tests
- [ ] Schema tests

### 17.3 PydanticAI Testing

- [ ] Agent tests
- [ ] Tool tests
- [ ] Dependency tests
- [ ] Model mocking
- [ ] Output testing
- [ ] Error testing

### 17.4 AI Evaluation

- [ ] What AI evaluation is
- [ ] Test datasets
- [ ] Expected outputs
- [ ] Structured evaluation
- [ ] LLM-as-judge
- [ ] Accuracy
- [ ] Reliability
- [ ] Tool-use evaluation
- [ ] Regression testing
- [ ] Evaluation pipelines

## 🏁 Exit Criteria

> A green test suite that runs offline, without a real LLM call.

Only mark this phase 🟢 in [`DASHBOARD.md`](../DASHBOARD.md) once that is true.

## 🐛 Mistakes Log

| Date | What broke | Why | Fix |
|---|---|---|---|
| | | | |

---

[⬅️ Phase 16](../phase-16-multi-agent/) · [📊 Dashboard](../DASHBOARD.md) · [Phase 18 ➡️](../phase-18-observability/)
