# 🗂️ Omar's AI Stack — Session Memory Repo

> **This repo is the long-term memory for all Claude Code sessions.**
> Every session logs what happened, what's pending, and what decisions were made.
> Any new Claude Code session should **read this repo first** to get full context.

---

## 🧭 How To Use This Repo (For Claude Code / New Sessions)

**START OF EVERY SESSION — run this:**
```bash
cat ~/ai-stack-logs/CURRENT_STATE.md
```
This gives you the full picture of where Omar is in the setup.

**END OF EVERY SESSION — do this:**
1. Update `CURRENT_STATE.md` with latest progress
2. Create a new log file in `logs/YYYY-MM-DD-session-NNN.md`
3. Commit and push both files

---

## 📁 Repo Structure

```
ai-stack-logs/
├── README.md               ← You are here. How this repo works.
├── CURRENT_STATE.md        ← Always-updated snapshot. Read this first.
├── TOOLS_REFERENCE.md      ← Master list of all tools in the stack
└── logs/
    └── YYYY-MM-DD-NNN.md   ← Individual session logs (append-only)
```

---

## 🔗 Companion Repos

| Repo | Purpose | URL |
|---|---|---|
| `ai-stack-setup` | Master PLAN.md + templates + agent configs | https://github.com/mr-tinoco/ai-stack-setup |
| `ai-stack-logs` | Session memory, logs, current state | https://github.com/mr-tinoco/ai-stack-logs |

---

## 📜 Rules

1. **Never delete log files** — they are append-only history
2. **Always update `CURRENT_STATE.md`** at end of session — this is the handoff doc
3. **If a new tool is added to the stack**, update `TOOLS_REFERENCE.md` immediately
4. **Commit after every session** — an uncommitted log is a lost memory

---

*This repo exists because context loss between sessions is the #1 productivity killer.*
*With this, every Claude Code session starts at 100% context — not 0%.*
