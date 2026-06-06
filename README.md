# 🐜 Ants-Review

Ants-Review 是一個以資安審查為核心的雙引擎 Code Review 平台。

理念來自：

> 一隻螞蟻看不到整個戰場，
> 但一群螞蟻可以找到所有漏洞。

---

## 核心設計

Ants-Review 不試圖取代資安顧問。

而是將不同 AI Reviewer 的能力整合：

### Open Code Review

角色：

- PR Reviewer
- Diff Reviewer
- Code Quality Reviewer

負責：

- 程式品質
- 可維護性
- Bug Pattern
- Pull Request 建議

---

### Metis

角色：

- Security Reviewer

負責：

- SQL Injection
- XSS
- CSRF
- Mass Assignment
- WordPress Security
- CWE Mapping

---

### CyberAnts Layer

角色：

- Human Guided Security Review

負責：

- RBAC
- IDOR
- Multi-Tenant
- Business Logic
- ISO 27001 思維
- False Positive 過濾

---

## 架構

```text
Next.js Frontend
        │
        ▼
FastAPI Backend
        │
        ▼
Review Orchestrator
 ├─ Open Code Review
 ├─ Metis
 ├─ CyberAnts Rules
 ├─ Cost Guard
 └─ Export Engine
```

---

## MVP

第一版聚焦：

- Local Repository Review
- Folder Review
- Security Review
- Cost Control
- JSON Export
- Markdown Export

---

## Future

- GitHub App
- GitLab Integration
- SARIF Export
- MCP Integration
- Multi-Agent Review
- Security Knowledge Base

---

## Why Ants?

螞蟻個體很小。

但群體非常強大。

資安審查也是如此。

單一工具永遠有盲點。

多個 Reviewer 協作，
才能更接近真實世界的安全風險。

---

## License

MIT
