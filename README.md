## Hi, I'm Mark 👋

**AVP, Transformation & Innovation at [Mandai Wildlife Group](https://www.mandai.com)** · Lean Six Sigma Black Belt

I lead Lean, Design Thinking, innovation and AI upskilling across the organisation. I also build. I believe transformation leaders should understand the technology well enough to ship it themselves, so this is where I turn ideas into working tools: AI agents, automations and apps with testing and security built in from day one.

### ⭐ Featured: Agentic Travel Planner
[**NUS-ISS-SWE5008-STACKABLE-2026-07-Team1/agentic-travel-planner**](https://github.com/NUS-ISS-SWE5008-STACKABLE-2026-07-Team1/agentic-travel-planner) · *NUS-ISS Graduate Certificate in Architecting AI Systems, team of 5, Jul–Oct 2026*

A five-agent AI travel planner (LangGraph + OpenAI) running in production on Google Kubernetes Engine. I was the team's largest contributor by commits. What I owned:

- **Flight Agent, end to end.** Design rule: *code decides which flights are real and how they rank; the AI only plans the search and explains the result.* A grounding check rejects any flight the model names that isn't in inventory, so it can never invent a bookable-looking flight.
- **Shared AI guardrail layer.** Input screening for prompt injection, bias and toxicity, plus output screening, tested against an adversarial test set; mapped to IMDA's Model AI Governance Framework for Agentic AI.
- **Agent-to-agent protocol.** Made the agents conformant with Google's A2A protocol, verified with its official conformance test kit.
- **Production deployment.** Containerised the system on GKE Autopilot, with a CI/CD pipeline that deploys on every merge and rolls back automatically, keyless cloud login, least-privilege access, and autoscaling (1→3 pods) proven under load.

*Team CI at release: 1,247 automated tests, SonarCloud quality gate passed (A/A/A), 80% coverage.*

### 🛠️ What I've built

| Project | The problem it solves | Built with |
|---|---|---|
| [**fever-tracker**](https://github.com/markteojunyi/fever-tracker) | Parents juggling a sick child's temperature readings and medicine doses on scraps of paper. A full web app with login, tests and automated security scanning in CI. | Next.js, TypeScript, MongoDB, Vitest, OWASP ZAP |
| [**youtube-digest**](https://github.com/markteojunyi/youtube-digest) | Losing 30 minutes a day skimming YouTube. Summarises new videos from chosen channels into a 60-second executive email each morning. | Python, Claude API, YouTube API, GitHub Actions |
| [**ai-news-newsletter-agent**](https://github.com/markteojunyi/ai-news-newsletter-agent) | AI news written for engineers, not leaders. Picks the top 5 stories daily and frames each as *"what this means for you"*. | Python, Claude API, RSS, SQLite, GitHub Actions |
| [**hdb-resale-rag-assistant**](https://github.com/markteojunyi/hdb-resale-rag-assistant) | HDB buying rules scattered across dozens of web pages. A RAG chatbot grounded in HDB's own guidance, plus a resale price explorer. | Python, LangChain, OpenAI, ChromaDB, Streamlit |
| [**springboot-devsecops-pipeline**](https://github.com/markteojunyi/springboot-devsecops-pipeline) | Security checked too late in delivery. A CI/CD pipeline that tests, scans libraries (Snyk), attacks the live app (ZAP) and alerts via Telegram. | GitHub Actions, Java, Snyk, OWASP ZAP |
| [**gof-pattern-auditor**](https://github.com/markteojunyi/gof-pattern-auditor) | Reviewing code design is slow and subjective. A three-step prompt chain that detects, validates and refactors design patterns. | JavaScript, Claude API, prompt chaining |

### 👥 Other team projects

- [**PeerConnect**](https://github.com/nus-mtech-se-projects/PeerConnect): Azure-hosted peer tutoring platform (Spring Boot + React), team of 7, NUS-ISS SWE5006. I built the peer feedback feature's backend, refactored a "god class" audit service into a Facade with pluggable sinks (SQL, Azure Monitor, Sentry), and fixed dependency vulnerabilities flagged by Snyk.

### 💡 How I work

- **Start with the problem, not the tool.** Every project above began as a real annoyance. The Lean habit: go and see, then fix the process.
- **Build small, ship, learn.** MVP first, then iterate. Design Thinking in practice.
- **Responsible by default.** Secrets stay out of code, scans run on every push, and AI output gets checked and grounded in sources.

### 🧰 Toolkit

`Python` `TypeScript` `Next.js` `Java / Spring Boot` · `Claude / OpenAI APIs` `LangGraph` `LangChain` `RAG` `Multi-agent / A2A` `AI guardrails` · `GitHub Actions` `Docker` `Kubernetes (GKE)` `Azure` · `Power Platform` `Copilot Studio`

### 📫 Connect

[LinkedIn](https://www.linkedin.com/in/markteojunyi/) · markteojunyi@gmail.com
