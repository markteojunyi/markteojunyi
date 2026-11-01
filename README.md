## Hi, I'm Mark 👋

**AVP, Transformation & Innovation at [Mandai Wildlife Group](https://www.mandai.com)** · Lean Six Sigma Black Belt

I lead Lean, Design Thinking, innovation and AI upskilling across the organisation. I also build. I believe transformation leaders should understand the technology well enough to ship it themselves, so this is where I turn ideas into working tools: AI agents, automations and apps with testing and security built in from day one.

### ⭐ Featured: Agentic Travel Planner
[**NUS-ISS-SWE5008-STACKABLE-2026-07-Team1/agentic-travel-planner**](https://github.com/NUS-ISS-SWE5008-STACKABLE-2026-07-Team1/agentic-travel-planner) · *NUS-ISS Graduate Certificate in Architecting AI Systems, team of 5, Jul–Oct 2026*

A five-agent AI travel planner running in production on Google Kubernetes Engine. I was the team's largest contributor by commits. What I owned:

- **Flight Agent, end to end.** Design rule: *code decides which flights are real and how they rank; the AI only plans the search and explains the result.* A grounding check rejects any flight the model names that isn't in inventory, so it can never invent a bookable-looking flight. Three execution modes: one model call, a bounded tool-calling loop, or automatic escalation from one to the other.
- **Shared AI guardrail layer.** Input screening for prompt injection, bias and toxicity, plus output screening, tested against an adversarial test set and mapped to IMDA's Model AI Governance Framework for Agentic AI.
- **Agent-to-agent protocol.** Made the agents conformant with Google's A2A protocol, verified with its official conformance test kit (TCK).
- **Production deployment and DevSecOps pipeline.** Containerised the system on GKE Autopilot and built the CI/CD workflows: every merge is scanned and tested, then deployed automatically with rollback if health checks fail. Includes keyless cloud login, least-privilege access, and autoscaling (1→3 pods) proven under load.

| Area | What I used |
|---|---|
| **AI and agents** | OpenAI GPT-5 / GPT-5-mini · LangGraph · LangChain · Pydantic · Google A2A protocol (a2a-sdk) |
| **Backend and data** | Python · Flask · Starlette / Uvicorn · Gunicorn · PostgreSQL on Supabase (connection pooling) |
| **Cloud and platform** | Docker · GKE Autopilot · Kubernetes (Kustomize, autoscaling on custom metrics, NetworkPolicy, PodDisruptionBudgets) · Artifact Registry · Identity-Aware Proxy · Workload Identity Federation · Cloud Monitoring + Managed Prometheus · Render (backup host) |
| **Security in CI/CD** | GitHub Actions · **Secret scanning:** gitleaks · **SAST** (scans the code): Bandit, Semgrep with 9 custom LLM/agent rules, SonarCloud · **SCA** (scans the libraries): pip-audit · **Container scanning:** Trivy · **DAST** (attacks the running app): OWASP ZAP, authenticated scan · **Infrastructure checks:** kubeconform, kubesec, hadolint · Branch protection with 5 required checks |
| **Testing and AI evaluation** | pytest (incl. a Postgres suite) · Playwright end-to-end tests · adversarial guardrail test set · golden scenarios · bias audit · LLM-as-a-judge evaluation · load and autoscaling tests |

*Team CI at release: 1,247 automated tests, SonarCloud quality gate passed (A/A/A), 80% coverage.*

### 🛠️ Other Projects

| Project | The problem it solves | Built with |
|---|---|---|
| [**family-scheduler-bot**](https://github.com/markteojunyi/family-scheduler-bot) | School schedule changes arriving as app notifications with no export, then living in someone's memory. A Telegram bot that turns a message or a screenshot into the right calendar entry, and asks a human before every write. Ran 24/7 for my household; 793 tests. | Python, OpenAI, Telegram Bot API, Google Calendar API, SQLite, GCP |
| [**hdb-resale-rag-assistant**](https://github.com/markteojunyi/hdb-resale-rag-assistant) | HDB buying rules scattered across dozens of web pages. A RAG chatbot grounded in HDB's own guidance, plus a resale price explorer. | Python, LangChain, OpenAI, ChromaDB, Streamlit |
| [**fever-tracker**](https://github.com/markteojunyi/fever-tracker) | Parents juggling a sick child's temperature readings and medicine doses on scraps of paper. A full web app with login, tests and automated security scanning in CI. | Next.js, TypeScript, MongoDB, Vitest, OWASP ZAP |
| [**PeerConnect**](https://github.com/nus-mtech-se-projects/PeerConnect) | Students' peer support being informal and scattered. An Azure-hosted peer tutoring platform (team of 7, NUS-ISS). My part: the peer feedback feature's backend, refactoring a "god class" audit service into a Facade with pluggable sinks, and fixing dependency vulnerabilities flagged by Snyk. | Spring Boot, React, Azure, Azure SQL, Sentry, Azure Monitor, Snyk |
| [**ai-news-newsletter-agent**](https://github.com/markteojunyi/ai-news-newsletter-agent) | AI news written for engineers, not leaders. Picks the top 5 stories daily and frames each as *"what this means for you"*. | Python, Claude API, RSS, SQLite, GitHub Actions |
| [**youtube-digest**](https://github.com/markteojunyi/youtube-digest) | Losing 30 minutes a day skimming YouTube. Summarises new videos from chosen channels into a 60-second executive email each morning. | Python, Claude API, YouTube API, GitHub Actions |
| [**gof-pattern-auditor**](https://github.com/markteojunyi/gof-pattern-auditor) | Reviewing code design is slow and subjective. A three-step prompt chain that detects, validates and refactors design patterns. | JavaScript, Claude API, prompt chaining |

### 💡 How I work

- **Start with the problem, not the tool.** Most of my personal projects began as a real annoyance at home or at work. The Lean habit: go and see, then fix the process.
- **Build small, ship, learn.** MVP first, then iterate. Design Thinking in practice.
- **Responsible by default.** Secrets stay out of code, scans run on every push, and AI output gets checked and grounded in sources.

### 🧰 Toolkit

`Python` `TypeScript` `Next.js` `Java / Spring Boot` `PostgreSQL` · `Claude / OpenAI APIs` `LangGraph` `LangChain` `RAG` `Multi-agent / A2A` `AI guardrails` `LLM evaluation` · `GitHub Actions` `Docker` `Kubernetes (GKE)` `Google Cloud` `Azure` · `SAST / DAST / SCA` `Playwright` · `Power Platform` `Copilot Studio`

### 📫 Connect

[LinkedIn](https://www.linkedin.com/in/markteojunyi/) · markteojunyi@gmail.com
