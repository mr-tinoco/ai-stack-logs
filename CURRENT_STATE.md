# 🟢 Current State — Omar's AI Stack
> **Last updated:** 2026-03-19 | **Session:** 003 (complete)
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

**Active Phase:** Phase 4 — Automation (OpenClaw) — agents not yet built
**Last completed action:** All 4 Ollama models installed. OpenClaw (n8n) running via Docker. All 3 API keys rotated and loaded into ~/openclaw/.env (Session 003).

### Phase Progress:
| Phase | Name | Status |
|---|---|---|
| 1 | Foundations (Notion + Todoist) | ✅ COMPLETE |
| 2 | Dev Environment | ✅ COMPLETE |
| 3 | Local AI (Ollama) | ✅ COMPLETE |
| 4 | Automation (OpenClaw) | 🟡 IN PROGRESS — infra up, agents not built |
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
| Gemini CLI | 0.32.1 | ✅ |
| Docker | 29.1.3 | ✅ Running |
| Git | 2.50.1 | ✅ |
| Homebrew | 5.0.16 | ✅ |
| GitHub CLI (gh) | ✅ | Authenticated as **mr-tinoco** |
| Ollama | ✅ | Running — 4 models installed |
| llama3.2 | 2.0 GB | ✅ fast automation |
| qwen2.5-coder:7b | 4.7 GB | ✅ code tasks |
| qwen2.5:14b | 9.0 GB | ✅ daily driver |
| deepseek-r1:14b | 9.0 GB | ✅ reasoning |
| OpenClaw (n8n) | ✅ | Running at http://localhost:5678 via Docker |
| API Keys | ✅ | Anthropic + OpenAI + Google — rotated & loaded in ~/openclaw/.env |

---

## ❌ What Still Needs Doing

| Item | Phase | Notes |
|---|---|---|
| Build Agent 1: goals-checkin | 4 | Claude, Sundays 6pm |
| Build Agent 2: project-heartbeat | 4 | Ollama, Mondays 9am |
| Build Agent 3: db-maintenance | 4 | Ollama, nightly 2am |
| Set spend caps | 4 | Anthropic $20/mo, OpenAI $10/mo |
| Claude Cowork | 5 | Anthropic desktop app |

---

## 🧠 Key Decisions Made So Far

1. **Repo strategy:** Two repos — `ai-stack-setup` (plan + config) and `ai-stack-logs` (memory + logs)
2. **Model routing:** Ollama handles 70-80% of OpenClaw tasks (free), Claude/OpenAI only for complex work
3. **Cost target:** Three tiers — Lean <$30 / Growth <$100 / Power <$200 (currently on Tier 1)
4. **Tool hierarchy:** Cursor → Claude Code → Gemini CLI (in that order for code work)
5. **Knowledge system:** Notion (why/context) + Todoist (what/when) + markdown files (portable)
6. **Claude Projects → deprecated as primary brain:** Context migrated to markdown + Notion. Claude Projects kept as read-only archive.
7. **Session memory system:** Guru prompt now has `<session_boot>` block — reads CURRENT_STATE.md at start of every session. No more cold starts.
8. **Normie AI context fully loaded:** All key PDFs read. Goals Spec being generated from existing docs (no manual export needed).
9. **Notion:** Omar has "Supreme second brain north star" template under Areas — use this as base for Life OS structure.

---

## 🔮 Next Session — Phase 4 (OpenClaw Agents)

**Pick up right here:**
1. Open http://localhost:5678 (make sure Docker is running first)
2. Build Agent 1: `goals-checkin` — weekly Sunday 6pm check-in via Claude
3. Build Agent 2: `project-heartbeat` — Monday 9am git log summary via Ollama
4. Build Agent 3: `db-maintenance` — nightly 2am cleanup via Ollama
5. Set spend caps: Anthropic console $20/mo, OpenAI $10/mo

### Open Questions
- What notification channel for agents? (Telegram / Discord / email — pick one)

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

- [ ] What notification channel for OpenClaw agents? (Telegram / Discord / email)

---

*Update this file at the end of every session. It is the single source of truth for session continuity.*
