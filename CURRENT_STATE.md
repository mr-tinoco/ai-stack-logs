# 🟢 Current State — Omar's AI Stack
> **Last updated:** 2026-03-07 | **Session:** 001
> **Read this at the start of every Claude Code session.**

---

## 🎯 What We're Building

A seamless AI dev stack that:
- Routes tasks to the cheapest capable model (Ollama → OpenAI mini → Claude/Gemini)
- Keeps all knowledge portable (Notion + markdown)
- Runs automated agents overnight via OpenClaw
- Costs under $30/month

**Master plan lives here:** `~/ai-stack-setup/PLAN.md`
**GitHub:** https://github.com/mr-tinoco/ai-stack-setup

---

## 📍 Where We Are Right Now

**Active Phase:** Phase 1 — Foundations (NOT STARTED YET)
**Last completed action:** Created repos + PLAN.md (Session 001)

### Phase Progress:
| Phase | Name | Status |
|---|---|---|
| 1 | Foundations (Notion + Todoist) | 🔴 Not started |
| 2 | Dev Environment | 🟡 80% done — need Vercel CLI + CLAUDE.md |
| 3 | Local AI (Ollama) | 🔴 Not started |
| 4 | Automation (OpenClaw) | 🔴 Not started |
| 5 | Claude Cowork | 🔴 Not started |
| 6 | NotebookLM | 🔴 Not started |
| 7 | Daily Workflow Lock-in | 🔴 Not started |

---

## ✅ What's Already Installed

| Tool | Version | Notes |
|---|---|---|
| Cursor | 2.1.71 | Installed, connected to GitHub |
| Claude Code | ✅ | Installed + authenticated |
| Node.js | v25.2.0 | ✅ |
| npm | 11.6.2 | ✅ |
| Gemini CLI | 0.32.1 | Installed — auth status unknown, test next session |
| Docker | 29.1.3 | ✅ Running |
| Git | 2.50.1 | ✅ |
| Homebrew | 5.0.16 | ✅ |
| GitHub CLI (gh) | ✅ | Authenticated as **mr-tinoco** |
| poppler | ✅ | Installed this session (for PDF reading) |

---

## ❌ What Still Needs Installing

| Tool | Phase | How |
|---|---|---|
| Vercel CLI | 2 | `npm install -g vercel && vercel login` |
| Ollama | 3 | Download from https://ollama.com/download/mac |
| llama3.2 model | 3 | `ollama pull llama3.2` |
| qwen2.5-coder:7b | 3 | `ollama pull qwen2.5-coder:7b` |
| OpenClaw | 4 | Docker compose setup in `~/openclaw/` |
| Claude Cowork | 5 | Anthropic desktop app |

---

## 🧠 Key Decisions Made So Far

1. **Repo strategy:** Two repos — `ai-stack-setup` (plan + config) and `ai-stack-logs` (memory + logs)
2. **Model routing:** Ollama handles 70-80% of OpenClaw tasks (free), Claude/OpenAI only for complex work
3. **Cost target:** $20-30/month variable + Claude Pro subscription
4. **Tool hierarchy:** Cursor → Claude Code → Gemini CLI (in that order for code work)
5. **Knowledge system:** Notion (why/context) + Todoist (what/when) + markdown files (portable)

---

## 🔮 Next Session Should Do

1. **Start Phase 1** — Ask Omar about Notion (does he have an account? existing structure?)
2. Walk through 1.1 → Export Claude data
3. Walk through 1.2 → Summarize key Claude projects into Goals Spec
4. Walk through 1.3 → Build Notion Life OS structure
5. Walk through 1.4 → Set up Todoist projects
6. Then immediately close out Phase 2 (Vercel CLI + CLAUDE.md)

---

## 💬 Context About Omar

- GitHub: **mr-tinoco**
- Machine: macOS (Apple Silicon — M-series)
- RAM: 16GB (inferred from guide recommendations)
- Main editor: Cursor
- Uses Claude Pro subscription
- Goal: Build automated AI system for dev work + personal life management
- Reference docs:
  - `/Users/omar/Documents/LLM/AI Stack Setup Guide.pdf`
  - `/Users/omar/Documents/LLM/OMAR_AI_STACK_SETUP.md`

---

## 🚨 Blockers / Open Questions

- [ ] Does Omar have a Notion account? What's the current structure?
- [ ] Does Omar have a Todoist account?
- [ ] Does Omar have an Anthropic API key (for OpenClaw agents)?
- [ ] Does Omar have an OpenAI API key?
- [ ] Does Omar have a Telegram/Discord for agent notifications?
- [ ] What is Omar's main project? (needed for CLAUDE.md in Phase 2.3)

---

*Update this file at the end of every session. It is the single source of truth for session continuity.*
