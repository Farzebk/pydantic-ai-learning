# Pydantic & PydanticAI — Version Comparison

> A practical reference for understanding the differences between Pydantic v1/v2 and older/newer PydanticAI APIs.

---

## 🎯 Purpose

This section is part of my **PydanticAI Learning Repository**.

The goal is to understand:

- Pydantic v1 vs v2
- PydanticAI API evolution
- Breaking changes
- Deprecated APIs
- Migration patterns
- How to recognize outdated tutorials
- How to convert older examples to current APIs

This is especially useful when following older YouTube tutorials, blog posts, GitHub repositories, or documentation.

---

# 📚 Table of Contents

- [1. Pydantic vs PydanticAI](#1-pydantic-vs-pydanticai)
- [2. Pydantic v1 vs v2](#2-pydantic-v1-vs-v2)
- [3. PydanticAI Version Evolution](#3-pydanticai-version-evolution)
- [4. Important API Changes](#4-important-api-changes)
- [5. Migration Cheat Sheet](#5-migration-cheat-sheet)
- [6. How to Identify Old Tutorials](#6-how-to-identify-old-tutorials)
- [7. Learning Strategy](#7-learning-strategy)
- [8. Practice Tasks](#8-practice-tasks)
- [9. Version Checklist](#9-version-checklist)

---

# 1. Pydantic vs PydanticAI

These are two different projects.

## Pydantic

Pydantic is a Python library for:

- Data validation
- Data parsing
- Serialization
- Type-safe data models
- Schema generation

Example:

```python
from pydantic import BaseModel


class User(BaseModel):
    name: str
    age: int
```

---

## PydanticAI

PydanticAI is an agent framework built around Python type safety and Pydantic models.

It provides concepts such as:

- Agents
- Models
- Tools
- Dependencies
- Structured outputs
- Streaming
- Message history
- Multi-agent workflows
- Testing

Example:

```python
from pydantic_ai import Agent

agent = Agent(
    "openai:gpt-4o",
    output_type=str,
)
```

---

# 2. Pydantic v1 vs v2

Pydantic v2 introduced significant changes to the API and internals.

## 2.1 Validators

### Pydantic v1

```python
from pydantic import BaseModel, validator


class User(BaseModel):
    name: str

    @validator("name")
    def validate_name(cls, value):
        return value.strip()
```

### Pydantic v2

```python
from pydantic import BaseModel, field_validator


class User(BaseModel):
    name: str

    @field_validator("name")
    @classmethod
    def validate_name(cls, value):
        return value.strip()
```

### Main change

```text
@validator
     ↓
@field_validator
```

---

# 2.2 Model Serialization

### Pydantic v1

```python
user.dict()
```

### Pydantic v2

```python
user.model_dump()
```

---

## JSON Serialization

### Pydantic v1

```python
user.json()
```

### Pydantic v2

```python
user.model_dump_json()
```

---

# 2.3 Model Parsing

### Pydantic v1

```python
User.parse_obj(data)
```

### Pydantic v2

```python
User.model_validate(data)
```

---

## JSON Parsing

### Pydantic v1

```python
User.parse_raw(json_data)
```

### Pydantic v2

```python
User.model_validate_json(json_data)
```

---

# 2.4 Configuration

### Pydantic v1

```python
from pydantic import BaseModel


class User(BaseModel):

    class Config:
        validate_assignment = True
```

### Pydantic v2

```python
from pydantic import BaseModel, ConfigDict


class User(BaseModel):

    model_config = ConfigDict(
        validate_assignment=True
    )
```

---

# 2.5 Root Models

Pydantic v2 introduced a more explicit approach to root models.

```python
from pydantic import RootModel


class UserIds(RootModel[list[int]]):
    pass
```

---

# 2.6 Field Changes

Modern Pydantic code commonly uses:

```python
from pydantic import BaseModel, Field


class User(BaseModel):
    name: str = Field(
        min_length=2,
        max_length=50
    )
```

This allows validation rules to remain close to the field definition.

---

# 3. PydanticAI Version Evolution

PydanticAI has also evolved considerably.

Older tutorials may use APIs that differ from current releases.

The most important rule is:

> **Always check the PydanticAI version before copying code from an older tutorial.**

---

## Older PydanticAI examples

You may encounter:

```python
Agent(
    ...,
    result_type=...
)
```

and:

```python
result.data
```

Newer APIs may use:

```python
Agent(
    ...,
    output_type=...
)
```

and:

```python
result.output
```

The exact API should always be verified against the version installed in the project.

---

# 4. Important API Changes

## 4.1 `result_type` → `output_type`

Older examples may contain:

```python
agent = Agent(
    "openai:gpt-4o",
    result_type=User,
)
```

Current-style examples use:

```python
agent = Agent(
    "openai:gpt-4o",
    output_type=User,
)
```

---

## 4.2 `result.data` → `result.output`

Older examples:

```python
result = agent.run_sync("...")
print(result.data)
```

Current-style examples:

```python
result = agent.run_sync("...")
print(result.output)
```

---

## 4.3 Tools

PydanticAI uses decorators to expose Python functions as agent tools.

Example:

```python
from pydantic_ai import Agent


agent = Agent("openai:gpt-4o")


@agent.tool_plain
def get_weather(city: str) -> str:
    return f"Weather for {city}"
```

When working with dependencies, tools can receive execution context.

```python
from pydantic_ai import Agent, RunContext


agent = Agent("openai:gpt-4o")


@agent.tool
def get_user(
    ctx: RunContext,
    user_id: int,
) -> str:
    return f"User: {user_id}"
```

> Tool APIs have evolved across releases, so verify the installed version when practicing.

---

# 5. Migration Cheat Sheet

| Older API / Concept | Modern Equivalent / Direction |
|---|---|
| `result_type` | `output_type` |
| `result.data` | `result.output` |
| `@validator` | `@field_validator` |
| `.dict()` | `.model_dump()` |
| `.json()` | `.model_dump_json()` |
| `.parse_obj()` | `.model_validate()` |
| `.parse_raw()` | `.model_validate_json()` |
| `class Config` | `ConfigDict` / `model_config` |

> This table is a learning cheat sheet, not a substitute for checking the release-specific migration guide.

---

# 6. How to Identify Old Tutorials

When following a tutorial, look for these patterns.

## Pydantic

If you see:

```python
@validator
```

or:

```python
class Config:
```

or:

```python
model.dict()
```

the tutorial may be using Pydantic v1.

---

## PydanticAI

If you see:

```python
result_type=
```

or:

```python
result.data
```

the tutorial may target an older PydanticAI API.

---

## Check the installed version

Use:

```bash
pip show pydantic
```

and:

```bash
pip show pydantic-ai
```

Or:

```bash
pip freeze | findstr pydantic
```

On Linux/macOS:

```bash
pip freeze | grep pydantic
```

---

# 7. Learning Strategy

Do **not** try to memorize every historical API.

Instead:

```text
                    PydanticAI
                        │
                        ▼
                Learn current API
                        │
                        ▼
              Understand core concepts
                        │
          ┌─────────────┴─────────────┐
          ▼                           ▼
   Read older tutorials        Read current docs
          │                           │
          ▼                           ▼
    Identify old API           Learn recommended API
          │
          ▼
    Translate old → new
```

The goal is to understand **why the API works**, not just memorize syntax.

---

# 8. Practice Tasks

## Task 1 — Pydantic v1 → v2

Take this:

```python
class User(BaseModel):

    @validator("name")
    def validate_name(cls, value):
        return value.strip()
```

Convert it to Pydantic v2.

---

## Task 2 — Serialization

Convert:

```python
user.dict()
```

to the Pydantic v2 equivalent.

---

## Task 3 — Parsing

Convert:

```python
User.parse_obj(data)
```

to the Pydantic v2 equivalent.

---

## Task 4 — PydanticAI Output

Find an old PydanticAI example using:

```python
result_type
```

and rewrite it using the current API.

---

## Task 5 — Result Handling

Convert:

```python
result.data
```

to the current result access pattern.

---

## Task 6 — Tool Migration

Find an older PydanticAI tool example and:

1. Identify the version.
2. Identify deprecated APIs.
3. Rewrite it using the current API.
4. Explain the changes.

---

# 9. Version Checklist

Before starting any PydanticAI project:

- [ ] Check Python version
- [ ] Check Pydantic version
- [ ] Check PydanticAI version
- [ ] Check tutorial/documentation version
- [ ] Read relevant migration notes
- [ ] Avoid blindly copying old code
- [ ] Verify deprecated APIs
- [ ] Run examples locally

---

# 🧠 Key Takeaways

### Pydantic

```text
Pydantic v1
     ↓
Pydantic v2
     ↓
Major API + architecture improvements
```

Important examples:

```text
@validator
    ↓
@field_validator

.dict()
    ↓
.model_dump()

.json()
    ↓
.model_dump_json()

.parse_obj()
    ↓
.model_validate()
```

### PydanticAI

```text
Older PydanticAI APIs
        ↓
Newer PydanticAI APIs
```

Important examples you may encounter:

```text
result_type
    ↓
output_type

result.data
    ↓
result.output
```

The exact PydanticAI API depends on the installed release, so version-checking is an important part of working with the framework.

---

# 🚀 Personal Learning Rule

When I encounter code from an older tutorial:

```text
1. Identify the version
        ↓
2. Run/check the old example
        ↓
3. Find the current API
        ↓
4. Rewrite the example
        ↓
5. Understand WHY it changed
        ↓
6. Add the migration example to this folder
```

This turns outdated tutorials into useful learning material instead of confusion.

---

## Related Sections

- `01-pydantic-v2/` — Pydantic fundamentals
- `02-pydantic-ai-basics/` — PydanticAI fundamentals
- `03-tools/` — Agent tools
- `04-dependencies/` — Dependency injection
- `05-structured-output/` — Structured responses
- `06-streaming/` — Streaming
- `07-message-history/` — Conversations and messages
- `08-multi-agent/` — Multi-agent systems
- `09-testing/` — Testing agents
- `10-production/` — Production patterns

---

## Status

🚧 **Learning in progress**

This document will be updated as I learn new Pydantic and PydanticAI APIs and encounter migration issues.
