# 🔐 Phase 20 — Security & Production

**Status:** 🔴 Not Started

## 🎯 Goal

Deploy AI agents safely.

> 💡 Prompt injection is the one in this list with no clean solution — read widely on it.

## 📂 What lives in this folder

| Path | Contents |
|---|---|
| `notes/` | One markdown file per topic, using the notes template |
| `examples/` | Minimal working code — typed from memory, not copy-pasted |
| `practice/` | Deliberately broken code + the fix, and mini experiments |

**Suggested files in `examples/`:**

```text
Dockerfile
docker-compose.yml
.github/workflows/ci.yml
01_secret_management.py
02_prompt_injection_demo.py
03_rate_limiting.py
```

## ✅ Topics to Cover

### 20.1 Security

- [ ] API key management
- [ ] Environment variables
- [ ] Secret management
- [ ] Input validation
- [ ] Output validation
- [ ] Prompt injection
- [ ] Tool security
- [ ] Permission control
- [ ] Authentication
- [ ] Authorization
- [ ] Rate limiting
- [ ] Sensitive data handling
- [ ] Secure logging

### 20.2 Production Architecture

- [ ] Application architecture
- [ ] Configuration management
- [ ] Environment management
- [ ] Error handling
- [ ] Logging
- [ ] Monitoring
- [ ] Health checks
- [ ] Scaling
- [ ] Caching
- [ ] Queues
- [ ] Background jobs

### 20.3 Docker

- [ ] Docker basics
- [ ] Dockerfile
- [ ] Docker Compose
- [ ] Environment variables
- [ ] Production containers
- [ ] Database containers

### 20.4 CI/CD

- [ ] GitHub Actions
- [ ] Automated tests
- [ ] Linting
- [ ] Formatting
- [ ] Build pipeline
- [ ] Deployment pipeline

### 20.5 Deployment

- [ ] Production server
- [ ] Cloud deployment
- [ ] Database deployment
- [ ] Environment configuration
- [ ] Monitoring
- [ ] Health checks
- [ ] Rollbacks

### 20.6 Performance & Cost

- [ ] Token optimization
- [ ] Prompt optimization
- [ ] Model selection
- [ ] Context optimization
- [ ] Caching
- [ ] Request batching
- [ ] Concurrency
- [ ] Latency optimization
- [ ] Tool optimization
- [ ] Cost tracking
- [ ] Model fallback

## 🏁 Exit Criteria

> The app runs in Docker, deploys via CI, and no secret is anywhere near the repo.

Only mark this phase 🟢 in [`DASHBOARD.md`](../DASHBOARD.md) once that is true.

## 🐛 Mistakes Log

| Date | What broke | Why | Fix |
|---|---|---|---|
| | | | |

---

[⬅️ Phase 19](../phase-19-fastapi-and-database/) · [📊 Dashboard](../DASHBOARD.md) · [Phase 21 — Projects ➡️](../phase-21-projects/)
