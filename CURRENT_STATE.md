# 🟢 Current State — Omar's AI Stack
> **Last updated:** 2026-03-29 | **Session:** 005 (complete)
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
**Normie AI repos:** https://github.com/mr-tinoco/Normieai

---

## 📍 Where We Are Right Now

**Active Phase:** Phase 5 — Claude Cowork (HQ project ready to create)
**Last completed action (Session 005):** QA Agent ecosystem fully deployed. Main agent prompt + 3 companion skills built (qa-run, ux-audit, market-scan). INDEX.md, tech-os.md, CURRENT_STATE.md, Notion all updated. Logs written. All pushed to GitHub.

### Phase Progress:
| Phase | Name | Status |
|---|---|---|
| 1 | Foundations (Notion + Todoist) | ✅ COMPLETE |
| 2 | Dev Environment | ✅ COMPLETE |
| 3 | Local AI (Ollama) | ✅ COMPLETE |
| 4 | Automation (OpenClaw) | 🟡 IN PROGRESS — infra up, n8n workflows not yet built |
| 5 | Claude Cowork | 🟡 IN PROGRESS — HQ system prompt ready, project not yet created in claude.ai |
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
| API Keys | ✅ | Anthropic + OpenAI + Google — in ~/openclaw/.env |
| Vercel CLI | ✅ | Authenticated as mr-tinoco |

---

## 🤖 Agent Ecosystem — 12 Active + 1 Paused

### Layer 1 — `~/.claude/prompts/` (Claude Code slash commands)
| Slash Command | Agent | Status |
|---|---|---|
| `/ceo-agent` | CEO Agent (gstack framework) | ✅ Deployed |
| `/gstack-advisor` | gstack Advisor (ecosystem auditor) | ✅ Deployed |
| `/crisis-manager` | Crisis Manager | ✅ Deployed |
| `/weekly-planner` | Weekly Planner | ✅ Deployed |
| `/ynab-agent` | YNAB Financial Specialist | ✅ Deployed |
| `/kpi-dashboard` | KPI Dashboard | ✅ Deployed |
| `/brand-strategist` | Brand Strategist | ✅ Deployed |
| `/content-creator` | Content Creator | ✅ Deployed |
| `/infrastructure-agent` | Infrastructure Agent | ✅ Deployed |
| `/marketing-agent` | Marketing Agent | ✅ Deployed |
| `/qa-agent` | QA Agent (testing + UX + market intel) | ✅ Deployed — NEW Session 005 |
| `/el-fantasma` | El Fantasma 🎤 | ⏸️ Paused until first revenue |

### QA Agent Skills — `~/.claude/skills/`
| Skill | File | What it does |
|---|---|---|
| `/qa-run` | `qa-run.md` | Full 9-phase QA pass with ship/hold verdict |
| `/ux-audit` | `ux-audit.md` | Nielsen heuristics + user empathy map |
| `/market-scan` | `market-scan.md` | Competitor research + market gap analysis |

### Layer 2 — `~/personal-os/` (shared brain — all tools)
All 14 files present. See `~/personal-os/INDEX.md` for full routing guide.

---

## ❌ What Still Needs Doing

| Item | Phase | Notes |
|---|---|---|
| **List Subscription Tracker on Gumroad** | REVENUE | 🔴 #1 priority — overdue. Run `/qa-run` on it first. |
| Create Normie AI HQ in Claude Cowork | 5 | System prompt ready: `~/Cowork/projects/normie-ai-hq-system-prompt.md`. Upload 11 files from `~/personal-os/` |
| Build n8n Workflow 1: goals-checkin | 4 | Spec: `~/openclaw/agents/agent1-goals-checkin.md`. Sunday 6pm, Claude haiku |
| Build n8n Workflow 2: project-heartbeat | 4 | Spec: `~/openclaw/agents/agent2-project-heartbeat.md`. Monday 9am, Ollama |
| Build n8n Workflow 3: db-maintenance | 4 | Spec: `~/openclaw/agents/agent3-db-maintenance.md`. Nightly 2am, Ollama |
| Update docker-compose.yml volume mounts | 4 | Add personal-os + ai-stack-logs mounts (see AGENT-SETUP-GUIDE.md) |
| Set spend caps | 4 | Anthropic $20/mo, OpenAI $10/mo |
| **Post first content on X + Threads** | BRAND | 🔴 0 posts published |

---

## 🧠 Key Decisions Made So Far

1. **Repo strategy:** Two repos — `ai-stack-setup` (plan + config) and `ai-stack-logs` (memory + logs)
2. **Model routing:** Ollama handles 70-80% of OpenClaw tasks (free), Claude/OpenAI only for complex work
3. **Cost target:** Three tiers — Lean <$30 / Growth <$100 / Power <$200 (currently on Tier 1)
4. **Tool hierarchy:** Cursor → Claude Code → Gemini CLI (in that order for code work)
5. **Knowledge system:** Notion (why/context) + Todoist (what/when) + markdown files (portable)
6. **Dual-layer agent architecture:** `~/.claude/prompts/` (Claude Code slash commands) + `~/personal-os/` (shared brain for all tools). Both populated and in sync.
7. **Session memory system:** CURRENT_STATE.md read at start of every session. No more cold starts.
8. **gstack principles:** Baked into CEO Agent and gstack Advisor ONLY — not into brand-facing files. Brand has its own voice: "el flow de nosotros."
9. **Claude Cowork strategy:** ONE "Normie AI HQ" project with all agents accessible via slash commands (/ceo, /marketing, /brand, etc.) — not 8 separate projects.
10. **Brand voice decision:** All brand/content/marketing OS files rewritten to remove corporate/YC-flavored language. Normie AI voice = bilingual, Colombian, real, Omar talking.
11. **QA Agent architecture:** QA lives as a sub-agent of Technical Guru. Three companion skills (qa-run, ux-audit, market-scan) handle targeted use cases. Skills stored in `~/.claude/skills/`.

---

## 📁 Key File Locations

| File | Purpose |
|---|---|
| `~/personal-os/AGENT-SETUP-GUIDE.md` | Master setup guide for all 3 platforms |
| `~/personal-os/INDEX.md` | Agent roster + routing guide |
| `~/Cowork/projects/normie-ai-hq-system-prompt.md` | Ready-to-paste Cowork system prompt |
| `~/openclaw/agents/agent*.md` | n8n workflow specs |
| `~/openclaw/docker-compose.yml` | OpenClaw container config |
| `~/.config/claude/prompts/qa-agent.md` | QA Agent prompt |
| `~/.claude/skills/qa-run.md` | Full QA pass skill |
| `~/.claude/skills/ux-audit.md` | UX audit skill |
| `~/.claude/skills/market-scan.md` | Market scan skill |
| `~/ai-stack-setup/` | GitHub backup of all OS files + prompts |

---

## 🔮 Next Session — Pick Up Here

**Option A (fastest value — DO THIS FIRST):** List Subscription Tracker on Gumroad
→ Run `/qa-run https://subscription-tracker-alpha-tawny.vercel.app` for confidence check
→ Use the QA report bullet points in your Gumroad listing
→ Copy Gumroad description from: `~/personal-os/marketing-os.md`

**Option B (complete Cowork setup):** Create Normie AI HQ in Claude Cowork
→ Go to claude.ai → New Project → Name: "🧠 Normie AI HQ"
→ Paste system prompt from: `~/Cowork/projects/normie-ai-hq-system-prompt.md`
→ Upload 11 files from `~/personal-os/`

**Option C (complete automation):** Build OpenClaw n8n workflows
→ Open http://localhost:5678
→ Follow `~/personal-os/AGENT-SETUP-GUIDE.md` Part 3 — node by node

**Recommended order:** A → B → C. Revenue first.

---

## 💬 Context About Omar

- GitHub: **mr-tinoco**
- Machine: macOS (Apple Silicon — M-series)
- AMD Linux Infrastructure Engineer — $250K/yr — NON-NEGOTIABLE to protect
- North star: $400K income + $5M net worth by December 31, 2030
- Current side income: $0
- Main editor: Cursor + Claude Code

---

## 🚨 Blockers / Open Questions

- [ ] Notification channel for OpenClaw agents? (Telegram recommended — pick and set up)
- [ ] Gumroad listing for Subscription Tracker — this is the #1 revenue blocker

---

*Update this file at the end of every session. It is the single source of truth for session continuity.*
