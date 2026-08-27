# 📊 Learning Dashboard — Pydantic & PydanticAI

> Single source of truth for **where I am**, **what's next**, and **what "done" means** for every phase of this repository.
>
> **Last updated:** August 26, 2026

---

## 🎯 At a Glance

| | |
|---|---|
| **Current phase** | `PHASE 5` — Advanced Pydantic 🟡 |
| **Also active** | `PHASE 0` — Python Foundations 🟡 |
| **Current topic** | `Advanced Pydantic` |
| **Just completed** | `model_dump()`, `model_dump_json()`, nested serialization |
| **Next up** | Types → Nested Models → Validation |
| **Milestone tier** | 🥉 Beginner (in progress) |
| **Overall progress** | `██░░░░░░░░░░░░░░░░░░` ~7% (2 / 22 phases started) |

**Current learning path:**

```text
BaseModel ✅  →  Field 🔄  →  Types  →  Nested Models  →  Validation
   →  Serialization  →  Advanced Pydantic  →  JSON Schema  →  PydanticAI 🤖
```

---

## 📑 Contents

- [Status Legend](#-status-legend)
- [Phase Dashboard](#-phase-dashboard)
- [Phase Breakdown](#-phase-breakdown)
- [Milestones](#-milestones)
- [Project Portfolio](#-project-portfolio)
- [Learning Method](#-learning-method)
- [Repository Structure](#-repository-structure)
- [Progress Log](#-progress-log)
- [Resources](#-resources)

---

## 🚦 Status Legend

| Symbol | Meaning |
|:---:|---|
| 🔴 | Not started |
| 🟡 | Currently learning |
| 🟢 | Completed — concept understood and written from memory |
| 🔵 | Practiced — built at least one mini example without help |
| 🟣 | Project completed — used in a real, working piece of code |

A phase is only 🟢 when I can **explain it in my own words** and **write the code without looking**.

---

## 🗺️ Phase Dashboard

### Part I — Foundations (Pydantic)

| # | Phase | Status | Progress | Core Skill Unlocked |
|:---:|---|:---:|---|---|
| 0 | Python Foundations | 🟢 | `███░░░░░░░` | Read and write modern, typed Python |
| 1 | Pydantic Fundamentals | 🟢 | `████░░░░░░` | Define and instantiate models |
| 2 | Pydantic Models & Types | 🟢 | `░░░░░░░░░░` | Model any real-world data shape |
| 3 | Pydantic Validation | 🟢 | `░░░░░░░░░░` | Reject bad data before it spreads |
| 4 | Pydantic Serialization | 🟢 | `░░░░░░░░░░` | Move between Python ⇄ dict ⇄ JSON |
| 5 | Advanced Pydantic | 🔴 | `░░░░░░░░░░` | Config, generics, custom types |
| 6 | JSON Schema & Structured Data | 🔴 | `░░░░░░░░░░` | Describe data to an LLM |

### Part II — Building Agents (PydanticAI)

| # | Phase | Status | Progress | Core Skill Unlocked |
|:---:|---|:---:|---|---|
| 7 | PydanticAI Fundamentals | 🔴 | `░░░░░░░░░░` | Vocabulary and mental model |
| 8 | Agents & Instructions | 🔴 | `░░░░░░░░░░` | Run my first agent |
| 9 | Structured AI Output | 🔴 | `░░░░░░░░░░` | Type-safe, validated LLM responses |
| 10 | Dependencies & RunContext | 🔴 | `░░░░░░░░░░` | Feed app data into an agent |
| 11 | Tools & Tool Calling | 🔴 | `░░░░░░░░░░` | Let agents take real actions |
| 12 | Messages & History | 🔴 | `░░░░░░░░░░` | Multi-turn conversations |
| 13 | Streaming | 🔴 | `░░░░░░░░░░` | Real-time responses |
| 14 | Model Providers | 🔴 | `░░░░░░░░░░` | Swap LLMs without rewriting |

### Part III — Reliability & Scale

| # | Phase | Status | Progress | Core Skill Unlocked |
|:---:|---|:---:|---|---|
| 15 | Retries & Error Handling | 🔴 | `░░░░░░░░░░` | Agents that survive failure |
| 16 | Multi-Agent Systems | 🔴 | `░░░░░░░░░░` | Orchestration and delegation |
| 17 | Testing & Evaluation | 🔴 | `░░░░░░░░░░` | Prove it works, repeatedly |
| 18 | Observability | 🔴 | `░░░░░░░░░░` | See inside a running agent |

### Part IV — Production

| # | Phase | Status | Progress | Core Skill Unlocked |
|:---:|---|:---:|---|---|
| 19 | FastAPI & Database Integration | 🔴 | `░░░░░░░░░░` | Agents as real backends |
| 20 | Security & Production | 🔴 | `░░░░░░░░░░` | Safe, deployable systems |
| 21 | Real-World Projects | 🔴 | `░░░░░░░░░░` | End-to-end portfolio work |

---

## 🧭 Phase Breakdown

Each phase below lists its **goal**, the **key points** to cover, and the **exit criteria** that move it from 🟡 to 🟢.

---

### 🐍 Phase 0 — Python Foundations 🟢

**Goal:** Build a Python base strong enough to understand Pydantic and modern AI application development.

**Key points**
- Variables, data types, type conversion, `type()`
- Operators — arithmetic, comparison, logical, identity, membership
- Strings — indexing, slicing, methods, f-strings
- Collections — lists, tuples, sets, dictionaries, comprehensions
- Control flow — `if` / `elif` / `else`, `for`, `while`, `break`, `continue`
- Functions — arguments, defaults, `*args`, `**kwargs`, lambdas, scope
- Exceptions — `try` / `except` / `else` / `finally`, `raise`, custom exceptions
- OOP — classes, `__init__`, inheritance, polymorphism, abstract classes
- **Type hints** — `list[str]`, `dict[str, int]`, `Optional`, `Union`, `Literal`, `Annotated`, generics
- Modern Python — decorators, context managers, generators, dataclasses, packaging, `.env`, `async` / `await`

> ⭐ **Highest-leverage sub-topics for Pydantic:** type hints, decorators, dataclasses, `async`.

**Exit criteria:** I can write a typed Python class with inheritance and a decorator from memory, and explain what a type hint does and does *not* enforce at runtime.

---

### 🧱 Phase 1 — Pydantic Fundamentals 🟢 

**Goal:** Understand what Pydantic is, why it exists, and how it turns raw data into validated Python objects.

**Key points**
- Pydantic vs PydanticAI, and how they relate ✅
- `BaseModel` — fields, instantiation, attribute access ✅
- Validation and `ValidationError` ✅
- `BaseModel` vs a plain Python class ✅
- Required vs optional fields, default values 🔄
- Nested models, lists of models, dicts of models 🔄
- Recursive models, model inheritance, model inspection

**Mental model**

```text
Pydantic → Data Validation → Structured Python Data → JSON Schema
        → Structured AI Output → PydanticAI
```

**Exit criteria:** I can write a nested model from memory, trigger a `ValidationError` on purpose, and read the error output correctly.

---

### 🏷️ Phase 2 — Pydantic Models & Types 🟢

**Goal:** Model complex, strongly typed data comfortably.

**Key points**
- `Field()` — `default`, `default_factory`, `title`, `description`, `alias`, `examples`
- Numeric constraints — `gt`, `ge`, `lt`, `le`, `multiple_of`
- String constraints — `min_length`, `max_length`, `pattern`
- Basic and collection types — `str`, `int`, `float`, `bool`, `list`, `dict`, `tuple`, `set`
- Union and optional — `Optional`, `Union`, modern `str | None`
- Special types — `Literal`, `Enum`, `UUID`, `datetime`, `Decimal`
- Pydantic types — `EmailStr`, URL, network, secret types
- Nested models — optional, deeply nested, recursive

**Exit criteria:** I can model an "order with line items and a customer" in one sitting, using constraints instead of manual checks.

---

### 🛡️ Phase 3 — Pydantic Validation 🟢

**Goal:** Control how Pydantic validates, transforms, and rejects data.

**Key points**
- Type, required-field, default, and constraint validation
- `field_validator` — before vs after mode, ordering, multiple fields
- `model_validator` — before vs after, cross-field logic
- Raising clean, useful custom errors
- **Practice builds:** user registration, password rules, product, order, payment validators

**Exit criteria:** I can write a cross-field validator (e.g. `password == confirm_password`) without looking it up.

---

### 🔄 Phase 4 — Pydantic Serialization 🟢

**Goal:** Move data confidently between Python objects, dictionaries, and JSON.

**Key points**
- `model_dump()`, `model_dump_json()`
- `include` / `exclude`, nested serialization, serialization aliases
- `model_validate()`, `model_validate_json()`
- Custom serializers

**Flow**

```text
dict → model_validate() → Model → model_dump() → dict → JSON
```

**Exit criteria:** I can round-trip a nested model to JSON and back with no data loss, and exclude a secret field on the way out.

---

### 🧬 Phase 5 — Advanced Pydantic 🟡 ← *current*

**Goal:** Go beyond basic models.

**Key points**
- `ConfigDict` — extra fields (ignore / forbid / allow), strict mode, `validate_assignment`, aliases
- Custom types — `Annotated`, `BeforeValidator`, `AfterValidator`, reusable validation
- Generics — `TypeVar`, generic models (e.g. `Response[User]`, `Response[Order]`)
- `computed_field` and derived values
- Model copying, rebuilding, inspection, metadata

**Exit criteria:** I've built one reusable `Annotated` type and one generic `Response[T]` wrapper used in two places.

---

### 📐 Phase 6 — JSON Schema & Structured Data 🔴

**Goal:** Understand the bridge between Pydantic and structured AI output. **This is the hinge of the whole repo.**

**Key points**
- What JSON Schema is and why it exists
- `model_json_schema()` — properties, required fields, nested schemas, constraints, descriptions
- Why LLM output is unpredictable and why structure fixes it
- How a schema tells a model what shape to return
- How Pydantic validates what comes back

**Flow**

```text
Pydantic Model → JSON Schema → Expected Structure
              → AI Output → Pydantic Validation
```

**Exit criteria:** I can look at a model and predict its generated schema, including how `description=` shows up.

---

### 🤖 Phase 7 — PydanticAI Fundamentals 🔴

**Goal:** Learn the architecture and vocabulary before writing agent code.

**Key points**
- LLM basics — prompts, system instructions, user/assistant messages, tokens, context window, temperature
- Structured output, tool calling, function calling
- Agent vs chatbot — what's actually different
- PydanticAI concepts — `Agent`, model, instructions, dependencies, tools, `RunContext`, output, messages, history, streaming

**Exit criteria:** I can draw the agent architecture on paper and name each component's job.

---

### 🧑‍💻 Phase 8 — Agents & Instructions 🔴

**Goal:** Build and control agents.

**Key points**
- Install, configure environment and API key, select a model
- Create an `Agent`, add instructions, run it, read the result object
- Static vs dynamic instructions; instruction functions with runtime context
- Agent lifecycle — creation → run → model request → tool execution → output validation → result

```text
User → Agent → Model → LLM → Response
```

**Exit criteria:** A working agent running from my own script, with instructions I wrote.

---

### 📦 Phase 9 — Structured AI Output 🔴

**Goal:** Make AI responses predictable, validated, and type-safe.

**Key points**
- Text output vs Pydantic output
- Simple → nested → list-of-models → complex output models
- Output validation, invalid-output handling, output retries

**Practice projects:** resume parser · movie recommender · product info extractor · invoice extractor · generic JSON extraction agent

**Exit criteria:** An agent that returns a validated nested model and recovers when the LLM returns something malformed.

---

### 🔌 Phase 10 — Dependencies & RunContext 🔴

**Goal:** Supply application data to an agent at runtime.

**Key points**
- Dependency injection — what and why
- Database, API, user, and configuration dependencies
- `RunContext` — accessing deps inside instructions and tools, runtime state, lifecycle

```text
Application → Dependencies → RunContext → Agent → Instructions / Tools
```

**Exit criteria:** An agent whose instructions change based on injected user data.

---

### 🔧 Phase 11 — Tools & Tool Calling 🔴

**Goal:** Give agents the ability to act.

**Key points**
- Define a tool — description, arguments, return values
- Multiple tools and how the model selects between them
- Tools with `RunContext` and dependencies
- Tool errors — retryable vs non-retryable, graceful failure

**Practice tools:** calculator · weather · search · database · user lookup · API request · file search · email · calendar

**Exit criteria:** An agent that picks correctly between three tools, and recovers when one raises.

---

### 💬 Phase 12 — Messages & Conversation History 🔴

**Goal:** Maintain context across turns.

**Key points**
- Message types — user, assistant, tool, model
- Message structure and history
- Single-turn vs multi-turn, reusing and persisting history, context management

**Exit criteria:** A conversation where turn 3 correctly references something said in turn 1.

---

### 🌊 Phase 13 — Streaming 🔴

**Goal:** Deliver real-time responses.

**Key points**
- Why streaming matters, text and async streaming
- Partial responses, streaming events
- Structured output streaming, streaming with tools, UI integration

**Exit criteria:** Tokens visibly appearing in my terminal or UI as the model generates them.

---

### 🌐 Phase 14 — Model Providers 🔴

**Goal:** Stay provider-independent.

**Key points**
- Model abstraction and provider configuration
- OpenAI · Anthropic · Google / Gemini · local and open-source models
- Model switching, provider-specific capabilities, fallback strategies

**Exit criteria:** The same agent runs against two different providers with a one-line change.

---

### 🔁 Phase 15 — Retries & Error Handling 🔴

**Goal:** Build agents that don't collapse under real conditions.

**Key points**
- Error types — model, API, timeout, validation, tool, output
- Retry concepts — retrying validation, tools, and model calls; limits; backoff
- Reliability — timeouts, fallbacks, graceful degradation, error reporting, recovery

**Exit criteria:** An agent that retries a failed validation and reports cleanly when retries run out.

---

### 🤝 Phase 16 — Multi-Agent Systems 🔴

**Goal:** Make specialized agents collaborate.

```text
                    ┌── Research Agent
User → Manager ─────┼── Coding Agent
                    └── Review Agent
```

**Key points**
- Delegation, handoffs, orchestration, agent-to-agent communication
- Shared dependencies, structured result passing, manager/worker roles
- Patterns — sequential, parallel, manager/worker, router, reviewer, research → analysis → report, human-in-the-loop

**Exit criteria:** A manager agent that routes to at least two workers and merges their structured results.

---

### 🧪 Phase 17 — Testing & Evaluation 🔴

**Goal:** Stop manually eyeballing every response.

**Key points**
- `pytest` — unit, integration, fixtures, mocking, async testing
- Pydantic tests — models, validators, serialization, schema
- PydanticAI tests — agents, tools, dependencies, model mocking, output and error testing
- AI evaluation — test datasets, expected outputs, LLM-as-judge, accuracy, tool-use evaluation, regression testing

**Exit criteria:** A green test suite that runs without hitting a real LLM.

---

### 🔍 Phase 18 — Observability 🔴

**Goal:** See what the agent is actually doing.

**Key points**
- Logging — Python logging, agent/tool/error logs, structured logging
- Tracing — agent traces, model calls, tool calls, execution flow
- Metrics — token usage, latency, error rate, tool time, cost tracking
- Logfire — tracing, debugging, production monitoring

**Exit criteria:** I can open a trace and explain every step of a single agent run.

---

### ⚡ Phase 19 — FastAPI & Database Integration 🔴

**Goal:** Turn agents into real backend applications.

**Key points**
- Async Python — `async` / `await`, `asyncio`, concurrent tasks, async DB calls
- FastAPI — routes, request/response models, dependency injection, async and streaming endpoints, error handling, auth, docs
- PostgreSQL — tables, queries, relationships, indexes, transactions, pooling, ORM
- Database + agents — DB dependencies and tools, natural language → SQL, SQL validation, security

```text
Client → FastAPI → Pydantic → PydanticAI → LLM → Structured Response → Client
```

**Exit criteria:** A `POST /agent` endpoint returning a validated model, backed by real database reads.

---

### 🔐 Phase 20 — Security & Production 🔴

**Goal:** Deploy safely.

**Key points**
- **Security** — API key and secret management, input/output validation, prompt injection, tool security, permissions, auth, rate limiting, secure logging
- **Architecture** — configuration and environment management, monitoring, health checks, scaling, caching, queues, background jobs
- **Docker** — Dockerfile, Compose, production and database containers
- **CI/CD** — GitHub Actions, automated tests, linting, formatting, build and deploy pipelines
- **Deployment** — cloud deployment, environment config, monitoring, rollbacks
- **Performance & cost** — token and prompt optimization, model selection, caching, batching, concurrency, cost tracking, fallbacks

**Exit criteria:** The app runs in Docker, deploys via CI, and no secret is anywhere near the repo.

---

### 🏗️ Phase 21 — Real-World Projects 🔴

See [Project Portfolio](#-project-portfolio) below.

---

## 📈 Milestones

### 🥉 Beginner
- [ ] Python fundamentals
- [x] `BaseModel`
- [ ] `Field`
- [ ] Types
- [ ] Nested models
- [ ] Validation
- [ ] Serialization

### 🥈 Intermediate
- [ ] Advanced Pydantic
- [ ] JSON Schema
- [ ] First PydanticAI agent
- [ ] Instructions
- [ ] Structured output
- [ ] Dependencies
- [ ] Tools
- [ ] Conversation history
- [ ] Streaming

### 🥇 Advanced
- [ ] Model providers
- [ ] Error handling & retries
- [ ] Multi-agent systems
- [ ] Testing & evaluation
- [ ] Observability
- [ ] FastAPI
- [ ] Database integration

### 🏆 Production Ready
- [ ] Security
- [ ] Async architecture
- [ ] Docker
- [ ] CI/CD
- [ ] Deployment
- [ ] Monitoring
- [ ] Cost optimization
- [ ] A production AI application

---

## 🏗️ Project Portfolio

| # | Project | Status | Depends On | Core Idea |
|:---:|---|:---:|---|---|
| 01 | Structured Data Extractor | 🔴 | Phases 1–9 | Raw text → validated structured JSON |
| 02 | AI Research Agent | 🔴 | Phases 9–18 | Search tool + structured research report with sources |
| 03 | Database Agent | 🔴 | Phases 10–19 | Natural language → validated SQL → structured result |
| 04 | Personal AI Assistant | 🔴 | Phases 8–20 | Tools, memory, multi-agent, streaming, deployed API |
| 05 | Multi-Agent Research Platform | 🔴 | Phases 16–20 | Manager → search / analysis / fact-check / report |

<details>
<summary><b>Project 05 architecture</b></summary>

```text
                         ┌── Research Agent
                         ├── Search Agent
User → Manager Agent ────┼── Analysis Agent
                         ├── Fact Checker
                         └── Report Writer
```

</details>

---

## 🧪 Learning Method

Every new concept goes through the same loop:

```text
1. Learn → 2. Understand → 3. Write from memory → 4. Modify the example
→ 5. Break it on purpose → 6. Debug it → 7. Build a mini project
→ 8. Document it → 9. Commit it → 10. Move forward
```

### 📝 Notes template

For every topic, document:

| Section | What goes in it |
|---|---|
| **What is it?** | The concept in plain words |
| **Why does it exist?** | The problem it solves |
| **How does it work?** | The underlying behavior |
| **Syntax** | The minimal form |
| **Example** | A tiny working example |
| **Deep understanding** | What I understood *after* experimenting |
| **Common mistakes** | Errors I actually hit |
| **Real-world use case** | Where this shows up in production |
| **PydanticAI connection** | How it feeds into agents |

**Practice checklist per topic:** write it without looking · modify it · break it · debug it · build a mini example · explain it aloud.

---

## 📂 Repository Structure

```text
.
├── README.md              ← what this repo is
├── DASHBOARD.md           ← this file: progress + phase map
├── phase-00-python/
├── phase-01-pydantic-fundamentals/
│   ├── notes.md
│   ├── examples/
│   └── practice/
├── phase-02-models-and-types/
├── ...
├── phase-21-projects/
│   ├── 01-structured-data-extractor/
│   ├── 02-research-agent/
│   ├── 03-database-agent/
│   ├── 04-personal-assistant/
│   └── 05-multi-agent-platform/
└── resources.md
```

Each phase folder keeps the same three parts: `notes.md` (the template above), `examples/` (code I typed from memory), `practice/` (things I broke on purpose).

---

## 📅 Progress Log

### August 26, 2026
- **Stage:** Pydantic Fundamentals
- **Learned:** Pydantic vs PydanticAI · `BaseModel`
- **Learning now:** `Field`
- **Python practice:** variables · `int` · `float` · `type()` · arithmetic operations

<!-- Add a new dated entry at the TOP of this section after each session.
     Keep it to four lines: Stage / Learned / Learning now / Practice. -->

---

## 🔄 How to Update This Dashboard

1. Change the phase **status emoji** and progress bar in the [Phase Dashboard](#-phase-dashboard).
2. Tick the matching box in [Milestones](#-milestones).
3. Add a dated entry at the top of the [Progress Log](#-progress-log).
4. Update **At a Glance** (current phase, current topic, next up).
5. Bump the **Last updated** date at the top.

Progress bars are ten blocks: `█` = done, `░` = remaining. One block ≈ 10%.

---

## 📚 Resources

**Pydantic** — official documentation · API reference · examples
**PydanticAI** — official documentation · examples · API reference
**Python** — language docs · `typing` docs · `asyncio` docs
**Related** — FastAPI · PostgreSQL · pytest · Docker · GitHub Actions · Logfire

---

## ⭐ Philosophy

This repo is a **learning record + knowledge base + code practice + AI engineering portfolio** — not a tutorial collection.

Every commit should represent something real: a concept learned, an example implemented, a mistake fixed, an experiment run, a mini-project built, a phase completed.

```text
Learn → Practice → Break → Fix → Build → Document → Commit → Repeat
```

**Final goal:** independently design, build, test, deploy, and maintain production-quality AI agent systems with Python, Pydantic, PydanticAI, structured outputs, tools, multi-agent architectures, FastAPI, PostgreSQL, testing, evaluation, observability, Docker, and CI/CD.
