# 🟢 Current State — Omar's AI Stack
> **Last updated:** 2026-04-11 | **Session:** 010 | **gstack Audit:** April 5, 2026
> **Read this at the start of every Claude Code session.**

---

## 🏗️ gstack Advisor Audit — April 5, 2026

> **Ecosystem Score: 63/100** — Functional but needs significant work.
> **Critical finding:** Gumroad listing has been #1 priority for 2+ sessions. Still not done. This is the only blocker to first revenue.

### CEO: Read This Before Planning Anything

**The system is over-built for $0 revenue.** Everything needed to list SubTracker on Gumroad exists. The only missing piece is the act of doing it. Every session that ends without a Gumroad listing is execution failure, not a planning problem.

**May 1 milestone scope has been reset (Mode 4 applied):**

| Milestone | Original | Revised |
|---|---|---|
| SubTracker on Gumroad | May 1 | This week — non-negotiable |
| First paying customer | May 1 | Attempt by May 1 |
| Social content started | "consistent" by May 1 | First posts same day as Gumroad |
| Vercel Analytics | May 1 | This week (5 min task) |
| NomadTracker V1 | May 1 | **Deferred to June** — not realistic |
| $500+/month | May 1 | **Deferred to June** — not realistic from cold launch |
| OpenClaw full automation | May 1 | After first revenue, as planned |

**This week's single action:** SubTracker live on Gumroad + 3 social posts published.
**No new agents, tools, or automations until first revenue lands.**

**Bilingual opportunity flagged:** Post launch content in Spanish too. EN/ES toggle is already built. Use it in the brand.

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

**Active Phase:** SubTracker monetization — V1.2 shipped, Gumroad listing is next
**Last completed action (Session 007):** Full SubTracker V1.2 landing page overhaul deployed to Vercel. Also fixed a critical deploy issue — Vercel was watching the wrong repo.

### SubTracker Status:
| Item | Status |
|---|---|
| V1.1 features (edit, CSV, charts, dark mode, EN/ES, USD/COP) | ✅ Live |
| V1.2 landing page (dark mode, budget positioning, new sections) | ✅ Live — deployed today |
| Gumroad listing | 🔴 NOT DONE — #1 priority next session |
| Real screenshot swap (replace CSS mockup) | 🟡 Pending — do alongside Gumroad |
| Vercel Analytics (1 line of code) | 🟡 Pending |

### Stack Phase Progress:
| Phase | Name | Status |
|---|---|---|
| 1 | Foundations (Notion + Todoist) | ✅ COMPLETE |
| 2 | Dev Environment | ✅ COMPLETE |
| 3 | Local AI (Ollama) | ✅ COMPLETE |
| 4 | Automation (OpenClaw) | ✅ COMPLETE — all 3 agents built, tested, and active |
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
| OpenClaw (n8n) | ✅ | Running at http://localhost:5678 via Docker — 4 agents active |
| API Keys | ✅ | Anthropic + OpenAI + Google + Telegram + Discord — in ~/openclaw/.env |
| Vercel CLI | ✅ | Authenticated as mr-tinoco |
| OpenAI Codex CLI | 0.120.0 | ✅ Installed — `codex` command, config at ~/.codex/config.toml |
| Telegram Bot | NormieClaw | ✅ @mr_tinoco_bot — dispatcher live |
| Ollama custom models | normie-daily / normie-coder / normie-reason | ✅ Context-aware local models |

---

## 🤖 Agent Ecosystem — 13 Active + 1 Paused + 4 OpenClaw

### Layer 1 — `~/.claude/commands/` (Claude Code slash commands)
| Slash Command | Agent | Status |
|---|---|---|
| `/notion-agent-optimizer` | Notion Agent Optimizer (OS health + sync) | ✅ Deployed — NEW Session 008 |
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
| `/qa-agent` | QA Agent (testing + UX + market intel) | ✅ Deployed — Session 005 |
| `/el-fantasma` | El Fantasma 🎤 | ⏸️ Paused until first revenue |

### Notion Agent Optimizer Skills — `~/.claude/skills/`
| File | Sub-Routine | Auto-triggers when |
|---|---|---|
| `notion-agent-optimizer-session-start.md` | SR-1: Session Briefing | Every session start |
| `notion-agent-optimizer-weekly-health.md` | SR-2: Weekly Health Check | Friday/Sunday or "weekly check" |
| `notion-agent-optimizer-drift-detect.md` | SR-3: Project Drift Detection | Project names mentioned |
| `notion-agent-optimizer-sync-check.md` | SR-4: Database Sync Check | "sync", files out of date |
| `notion-agent-optimizer-transition-check.md` | SR-5: Transition Readiness | Milestones/deadlines mentioned |

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
| **List SubTracker on Gumroad** | REVENUE | 🔴 #1 priority. Copy is ready: `~/Documents/Claude/Projects/Normie AI HQ/subtracker-marketing-audit.md` |
| **Take real dark-mode screenshot** | REVENUE | Open app.html, add sample subs, screenshot at 1280px, save as screenshot.png, swap CSS mockup |
| **Add Vercel Analytics** | REVENUE | 1 line in index.html `<head>`: `<script defer src="/_vercel/insights/script.js"></script>` + enable in Vercel dashboard |
| **Post launch content on X + Threads** | BRAND | 🔴 3 ready-to-paste posts in marketing audit file |
| Create Normie AI HQ in Claude Cowork | 5 | System prompt ready: `~/Cowork/projects/normie-ai-hq-system-prompt.md`. Upload 11 files from `~/personal-os/` |
| Set spend caps | 4 | Anthropic $20/mo, OpenAI $10/mo — still unset |

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
12. **Portable OS:** Full stack restores on any Mac or Linux machine with one curl command. `bootstrap.sh --cloud` = 15 min. `bootstrap.sh --full` = full Ollama stack. Mac mini stays as always-on server (OpenClaw + Telegram Dispatcher keep running regardless).

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
| `~/ai-stack-setup/bootstrap.sh` | **One-command restore on any Mac or Linux machine** |

---

## 🧳 Portable Setup — New Machine in 15 Minutes

**One-liner (paste on any Mac or Linux terminal):**
```bash
bash <(curl -s https://raw.githubusercontent.com/mr-tinoco/ai-stack-setup/main/bootstrap.sh)
```

**Two modes:**
| Mode | Command | Time | What you get |
|---|---|---|---|
| Cloud | `./bootstrap.sh` (default) | ~15 min | Claude + Gemini + Codex + dotfiles + CURRENT_STATE.md |
| Full | `./bootstrap.sh --full` | 2-4 hrs | Everything + Docker + Ollama models (~25GB) |

**What the script installs automatically:**
- brew (Mac) or detects apt/dnf/pacman/zypper/apk (Linux)
- Node.js via nvm (universal, all Linux distros)
- Claude Code, Gemini CLI, OpenAI Codex CLI
- All dotfiles: .zshrc, .gemini/GEMINI.md, AGENTS.md, .codex/config.toml
- Clones ai-stack-setup + ai-stack-logs (gets CURRENT_STATE.md immediately)
- Prompts once for API keys → saves to ~/openclaw/.env

**API keys:** Keep in phone notes or password manager. Script prompts once per machine.

**Key fact:** Mac mini stays running at home. Telegram Dispatcher (@mr_tinoco_bot) and all OpenClaw agents keep working regardless of what machine you're on.

---

## 🔮 Next Session — Pick Up Here

### 🔴 #1 PRIORITY — List SubTracker on Gumroad

This is the revenue unlock. Everything is ready. Just needs to be done.

1. Go to gumroad.com → New Product → Digital Product
2. Title: `Stop Throwing Money at Subscriptions You Forgot About`
3. Price: $12 (one-time)
4. Description: copy from `~/Documents/Claude/Projects/Normie AI HQ/subtracker-marketing-audit.md` → section "Gumroad Listing Copy"
5. Cover image: take a dark-mode screenshot of the app (see below)
6. Once live → update href in index.html (both Gumroad buttons) + push to `mr-tinoco/subscription-tracker`

### 🟡 #2 — Take Real Screenshot (do this before Gumroad listing)

1. Open https://subscription-tracker-alpha-tawny.vercel.app/app.html
2. Toggle to dark mode
3. Add sample subs: Netflix $15.99, Spotify $9.99, Claude Pro $20, GitHub Pro $4, ChatGPT $20, Notion $10
4. Screenshot at 1280px wide
5. Save as `screenshot.png` in `~/Normieai/subscription-tracker/`
6. In index.html replace the entire `.mockup-card` div with:
```html
<div class="mockup-card">
  <img src="screenshot.png" class="rounded-2xl shadow-2xl w-full border border-slate-700" alt="SubTracker — budget tracker for subscriptions, dark mode screenshot" />
</div>
```
7. Push to `mr-tinoco/subscription-tracker`

### 🟡 #3 — Vercel Analytics (5 minutes)

Add to `index.html` inside `<head>`:
```html
<script defer src="/_vercel/insights/script.js"></script>
```
Then go to Vercel dashboard → subscription-tracker project → Analytics → Enable.

### ✅ DONE — OpenClaw Full Ecosystem (Sessions 009–010)

All 4 agents active in n8n (localhost:5678):

| Agent | ID | Schedule | Model | Output |
|---|---|---|---|---|
| Agent 1 — Goals Check-in | BYmFjNa7NugAddPO | Sunday 6 PM | claude-haiku-4-5-20251001 | `~/ai-stack-logs/weekly-reviews/` |
| Agent 2 — Project Heartbeat | openclaw2heartbeat | Monday 9 AM | qwen2.5:14b (free) | `~/ai-stack-logs/heartbeats/` |
| Agent 3 — DB Maintenance | openclaw3maintain | Nightly 2 AM | llama3.2 (free) | `~/ai-stack-logs/maintenance/` |
| Agent 4 — The Dispatcher | openclaw4dispatcher | Every 1 min | Routes auto | Telegram + Discord replies |

**Session 010 additions:**
- Telegram bot: NormieClaw (@mr_tinoco_bot) — token + chat ID in ~/openclaw/.env
- Discord webhook wired to all 4 agents
- Agent 2 upgraded to auto-discover git repos (no more hardcoding)
- Agent 4 (Dispatcher): routes Telegram messages to CEO/Technical/Status/Crisis/Brand/Financial/Infra agents
- Task queue: ~/ai-stack-logs/task-queue/ — phone tasks auto-executed at next Claude Code session
- Technical Guru session_boot updated to read task queue automatically

### ✅ DONE — Unified AI OS (Session 010)

All LLMs now share context via CURRENT_STATE.md as single source of truth:

| Tool | How it loads context | Command |
|---|---|---|
| Claude Code | session_boot reads CURRENT_STATE.md | `claude` |
| Gemini CLI | ~/.gemini/GEMINI.md auto-loaded | `gemini` |
| OpenAI Codex | ~/.codex/config.toml auto-loaded | `codex` |
| Ollama (daily) | Baked into normie-daily Modelfile | `ai-daily` |
| Ollama (code) | Baked into normie-coder Modelfile | `ai-code` |
| Ollama (reason) | Baked into normie-reason Modelfile | `ai-reason` |
| OpenAI quick | Injects CURRENT_STATE.md per call | `ai "question"` |
| Phone | Telegram @mr_tinoco_bot dispatcher | Message bot |

**New shell commands (open new terminal to activate):**
- `ai-route` — shows which tool to use for any task
- `stack-status` — Ollama models + OpenClaw + task queue depth
- `ai-daily` / `ai-code` / `ai-reason` — context-aware local models
- `ai "question"` — OpenAI gpt-4o-mini with full context
- `checkpoint "note"` — save mid-session progress note
- `resume-context` — prints context to paste into any AI tool

**New files created this session:**
- `~/.gemini/GEMINI.md` — Gemini global context
- `~/.codex/config.toml` — Codex CLI config
- `~/AGENTS.md` — Codex global context
- `~/personal-os/model-routing.md` — routing guide for all tools
- `~/openclaw/GEMINI.md` — project Gemini context
- `~/Normieai/subscription-tracker/GEMINI.md` — project Gemini context
- `~/ai-stack-logs/task-queue/` — phone task queue directory
- Ollama custom models: normie-daily, normie-coder, normie-reason
- OpenAI Codex CLI installed: v0.120.0

**Key infra facts:**
- n8n model API: use `claude-haiku-4-5-20251001` (NOT claude-3-5-haiku)
- HTTP Request body: use `contentType: raw` + `rawContentType: application/json`
- Code nodes: use `var` not `const`, no template literals, no `await`
- File I/O: `require('fs')` works (NODE_FUNCTION_ALLOW_BUILTIN=fs,path,child_process)
- Workflow management: `docker exec openclaw n8n import:workflow`
- All API keys load from ~/openclaw/.env via .zshrc on every terminal open

### 🔴 #4 — Post Launch Content

3 posts ready to paste in `~/Documents/Claude/Projects/Normie AI HQ/subtracker-marketing-audit.md` → "Launch Post Copy" section.
Post on X and Threads the same day as Gumroad listing goes live.

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
