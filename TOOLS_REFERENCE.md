# 🔧 Master Tools Reference — Omar's AI Stack
> **Update this file whenever a new tool is added to the stack.**
> This is the canonical list of every tool, why it exists, and how it fits.

---

## 🤖 AI Models

| Model | Provider | Role | Cost | When To Use |
|---|---|---|---|---|
| Claude Pro | Anthropic | Deep reasoning, architecture | $20/mo flat | Design, specs, complex planning, code reviews |
| Gemini Pro | Google | Large context, documents | $0-20/mo | Long PDFs, Google ecosystem, multimodal |
| GPT-4o-mini | OpenAI API | Production deployment | ~$0.15/1M tokens | User-facing AI features, CI/CD integrations |
| llama3.2 | Ollama (local) | Routine automation | $0 | 70-80% of OpenClaw tasks, simple ops |
| qwen2.5-coder:7b | Ollama (local) | Local code help | $0 | Code assistance without API costs |
| NotebookLM | Google | Document synthesis | $0 | Building knowledge bases, deep doc synthesis |

### Model Routing Decision Tree
```
Is it simple / repetitive?           → Ollama llama3.2 (FREE)
Needs structured output / reasoning? → OpenAI gpt-4o-mini (~$0)
Requires deep reasoning / arch?      → Claude Pro
Huge document / Google ecosystem?    → Gemini Pro
```

---

## 🛠️ Development Tools

| Tool | Version | Role | Install | Status |
|---|---|---|---|---|
| Cursor | 2.1.71 | Main code editor | cursor.com | ✅ Installed |
| Claude Code | latest | Repo-level AI agent | `npm i -g @anthropic-ai/claude-code` | ✅ Installed |
| Gemini CLI | 0.32.1 | Terminal AI assistant | `npm i -g @google/gemini-cli` | ✅ Installed |
| Vercel CLI | - | Production hosting + deploy | `npm i -g vercel` | ❌ Pending |
| GitHub CLI | latest | Repo management | `brew install gh` | ✅ Installed |
| Node.js | v25.2.0 | JS runtime | brew / nvm | ✅ Installed |
| npm | 11.6.2 | Package manager | bundled with Node | ✅ Installed |
| Homebrew | 5.0.16 | macOS package manager | brew.sh | ✅ Installed |
| Git | 2.50.1 | Version control | Xcode tools | ✅ Installed |
| Docker | 29.1.3 | Container runtime | docker.com | ✅ Installed |
| poppler | latest | PDF text extraction | `brew install poppler` | ✅ Installed |

### Dev Tool Hierarchy (use in this order)
```
Daily edits / browse code    → Cursor
Feature touching 3+ files    → Claude Code (in Cursor terminal)
Terminal / logs / scripts    → Gemini CLI
Quick prototype              → Replit → then migrate to repo
Deploy                       → Vercel
```

---

## 🤖 Automation Tools

| Tool | Role | Location | Status |
|---|---|---|---|
| OpenClaw | Scheduled AI agents | `~/openclaw/` via Docker | ❌ Pending |
| Ollama | Local LLM server | localhost:11434 | ❌ Pending |
| Claude Cowork | Desktop agent for local files | Anthropic desktop app | ❌ Pending |

### OpenClaw Agent Roster
| Agent | Model | Schedule | Purpose | Status |
|---|---|---|---|---|
| goals-checkin | Claude API | Sundays 6pm | Weekly goals review | ❌ Not created |
| project-heartbeat | Ollama llama3.2 | Mondays 9am | Git log → status summary | ❌ Not created |
| db-maintenance | Ollama + Claude | Nightly 2am | Database health check | ❌ Not created |

---

## 📚 Productivity & Knowledge Tools

| Tool | Role | When To Use | Status |
|---|---|---|---|
| Notion | Second brain / Life OS | Projects, specs, goals, knowledge base | ❓ Unknown |
| Todoist | Task management | All next actions, recurring habits, daily reviews | ❓ Unknown |
| Notability | Capture & sketch | Handwritten notes, diagrams, iPad brainstorms | External |
| Perplexity | Research | Comparing tools, finding best practices | External |
| NotebookLM | Document synthesis | Large doc collections, knowledge bases | ❌ Pending |
| Replit | Rapid prototyping | Quick PoCs, shareable demos | External |

---

## 📁 Key File Locations

| File | Location | Purpose |
|---|---|---|
| Master Plan | `~/ai-stack-setup/PLAN.md` | Full 7-phase roadmap |
| Current State | `~/ai-stack-logs/CURRENT_STATE.md` | Session handoff doc |
| Tools Reference | `~/ai-stack-logs/TOOLS_REFERENCE.md` | This file |
| Session Logs | `~/ai-stack-logs/logs/` | Append-only history |
| Setup Guide (PDF) | `~/Documents/LLM/AI Stack Setup Guide.pdf` | Original spec doc |
| Setup Guide (MD) | `~/Documents/LLM/OMAR_AI_STACK_SETUP.md` | Claude Code instructions |
| Daily Routine | `~/ai-stack-setup/DAILY-ROUTINE.md` | Created in Phase 7 |
| OpenClaw Config | `~/openclaw/docker-compose.yml` | Created in Phase 4 |
| Cowork Specs | `~/Cowork/specs/` | Goals spec + project context |

---

## 🆕 How To Add A New Tool

When a new tool is introduced to the stack:

1. **Add a row** to the appropriate table above
2. **Update `CURRENT_STATE.md`** — add to installed/pending list
3. **Add to `PLAN.md`** in `ai-stack-setup` if it requires a setup phase
4. **Log the decision** in the session log (`logs/YYYY-MM-DD-NNN.md`) with:
   - Why this tool was added
   - What it replaces or complements
   - How it fits the cost model
5. **Commit both repos**

---

*Last updated: 2026-03-07 | Session 001*
