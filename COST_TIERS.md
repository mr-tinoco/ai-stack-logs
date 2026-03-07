# 💰 Omar's AI Stack — Cost Tier Architecture
> **Last updated:** 2026-03-07 | Session 001
> Three tiers designed for different workload levels.
> Start at Tier 1. Only move up when the work demands it — that's a good problem to have.

---

## 🟢 TIER 1 — Lean Stack *(Target: under $30/month)*
> **Use case:** Daily dev work, personal automation, side projects.
> The default. 80%+ of work stays here.

### Model Routing
| Model | Provider | Monthly Cost | Usage |
|---|---|---|---|
| llama3.2 | Ollama (local) | **$0** | 70-80% of all automation tasks |
| qwen2.5-coder:7b | Ollama (local) | **$0** | Local code help, no API needed |
| gpt-4o-mini | OpenAI API | **~$5** | Production features, moderate complexity |
| Claude Pro | Anthropic | **$20** | Architecture, complex reasoning, Claude Code |
| Gemini (free tier) | Google | **$0** | Large doc context, Google ecosystem |

### Tools & Services
| Tool | Cost | Notes |
|---|---|---|
| Cursor | $0 | Free tier |
| Claude Code | $0 | Included with Claude Pro |
| Gemini CLI | $0 | Free |
| Vercel | $0 | Hobby tier (personal projects) |
| Ollama | $0 | Local, your hardware |
| OpenClaw | $0-5 | Run locally via Docker |
| GitHub | $0 | Free tier |
| NotebookLM | $0 | Free |
| Replit | $0 | Free tier for prototyping |

### 💵 Tier 1 Budget Breakdown
```
Ollama (local models)       $0
Gemini CLI / free tier      $0
Cursor free tier            $0
Vercel hobby                $0
GitHub free                 $0
NotebookLM                  $0
─────────────────────────────
Subtotal (free)             $0

Claude Pro subscription     $20
OpenAI API (mini, light)    $5-8
─────────────────────────────
TOTAL TIER 1                ~$25-28/month ✅
```

### Tier 1 Rules
- Ollama handles **all** OpenClaw automation by default
- Claude Pro used for planning/architecture — **never** for repetitive tasks
- OpenAI API only for production user-facing features
- Agent heartbeats minimum 24h intervals
- Hard caps: Anthropic $20, OpenAI $10

---

## 🟡 TIER 2 — Growth Stack *(Target: under $100/month)*
> **Use case:** Active client work, startup building, multiple projects running simultaneously.
> Move here when Tier 1 is bottlenecking real output.

### Model Routing (upgraded)
| Model | Provider | Monthly Cost | Usage |
|---|---|---|---|
| llama3.2 / qwen2.5 | Ollama (local) | **$0** | Still 50-60% of automation |
| qwen2.5-coder:14b | Ollama (local, GPU rig) | **$0** | Heavier local code — if you have a desktop GPU |
| gpt-4o-mini | OpenAI API | **~$15** | Higher volume production features |
| gpt-4o | OpenAI API | **~$20** | Complex production features, quality-critical |
| Claude Pro | Anthropic | **$20** | Architecture + heavy Claude Code usage |
| Gemini Advanced | Google | **$20** | Large context at scale, 1M token window |
| Claude API | Anthropic | **~$10-15** | OpenClaw agents that need premium reasoning |

### Tools & Services (upgraded)
| Tool | Cost | Notes |
|---|---|---|
| Cursor Pro | $20 | Faster models, more context |
| Claude Code | $0 | Included with Claude Pro |
| Gemini CLI | $0 | Free |
| Vercel Pro | $20 | Custom domains, team features, more bandwidth |
| OpenClaw VPS | $10-15 | Run 24/7 on a cloud server (DigitalOcean/Hetzner) |
| GitHub | $0 | Free or Teams $4/mo |
| Supabase | $25 | Postgres + Auth + Storage (if needed) |
| Replit | $0-7 | Free or Core for heavier prototyping |

### 💵 Tier 2 Budget Breakdown
```
Ollama (local)              $0
GitHub                      $0
Gemini CLI                  $0
─────────────────────────────
Subtotal (free)             $0

Claude Pro subscription     $20
Gemini Advanced             $20
Cursor Pro                  $20
Vercel Pro                  $20
OpenClaw VPS (Hetzner)      $10
OpenAI API (gpt-4o-mini)    $15
OpenAI API (gpt-4o bump)    $10
Claude API (agents)         $10
─────────────────────────────
TOTAL TIER 2                ~$85-95/month ✅
```

### When To Move To Tier 2
- [ ] OpenAI API consistently hitting $10+ on Tier 1
- [ ] You're running 5+ active OpenClaw agents
- [ ] Cursor free tier slowing you down on large repos
- [ ] You have a live product with real users
- [ ] Working on multiple client projects simultaneously

---

## 🔴 TIER 3 — Power Stack *(Target: under $200/month)*
> **Use case:** Heavy client load, multiple production products, serious automation, team-level output as a solo dev.
> This is "I'm making real money and the tools need to keep up" territory.
> Getting here means the stack is working — that's the goal.

### Model Routing (full power)
| Model | Provider | Monthly Cost | Usage |
|---|---|---|---|
| llama3.1:70b | Ollama (desktop GPU rig) | **$0** | Heavy local inference on powerful hardware |
| qwen2.5-coder:32b | Ollama (desktop GPU rig) | **$0** | Near-GPT-4 code quality, zero API cost |
| gpt-4o | OpenAI API | **~$30-40** | High-volume production, multiple products |
| o3-mini | OpenAI API | **~$10-15** | Reasoning-heavy tasks at lower cost than o3 |
| Claude Pro | Anthropic | **$20** | Architecture + maximum Claude Code usage |
| Claude API (Sonnet) | Anthropic | **~$20-25** | Premium OpenClaw agents, critical pipelines |
| Gemini Advanced | Google | **$20** | Massive context windows (2M tokens) |
| Gemini API | Google | **~$10** | High-volume doc processing |

### Tools & Services (full power)
| Tool | Cost | Notes |
|---|---|---|
| Cursor Pro | $20 | Essential at this level |
| Claude Code | $0 | Included with Claude Pro |
| Vercel Pro | $20 | Production hosting for multiple projects |
| OpenClaw VPS (beefier) | $20-30 | Hetzner CX31 or DigitalOcean 4GB — 10+ agents |
| GitHub Teams | $4 | Better CI/CD, protected branches |
| Supabase Pro | $25 | Scale beyond free tier |
| Doppler / 1Password | $8-10 | Secrets management across projects |
| Replit Teams | $15-20 | If using Replit heavily for client demos |
| Monitoring (Sentry free) | $0-10 | Error tracking on production apps |
| Domain / DNS | $10-15 | Namecheap or Cloudflare for multiple projects |

### 💵 Tier 3 Budget Breakdown
```
Ollama (local — desktop rig)     $0
GitHub (free or Teams)           $0-4
─────────────────────────────────
Subtotal (free/near-free)        $0-4

Claude Pro subscription          $20
Claude API (Sonnet, agents)      $20-25
Gemini Advanced                  $20
Gemini API (volume)              $10
OpenAI API (gpt-4o production)   $35-40
OpenAI (o3-mini reasoning)       $10
Cursor Pro                       $20
Vercel Pro                       $20
OpenClaw VPS (Hetzner CX31)      $20
Supabase Pro                     $25
Secrets mgmt (Doppler)           $8
Domain + DNS                     $12
─────────────────────────────────
TOTAL TIER 3                     ~$175-195/month ✅
```

### When To Move To Tier 3
- [ ] Billing multiple clients simultaneously
- [ ] Running production apps with real traffic
- [ ] Need 10+ OpenClaw agents running 24/7
- [ ] Local Ollama models not powerful enough even with GPU rig
- [ ] Time saved > cost of tools by 5x or more
- [ ] Monthly revenue from projects > $2,000

---

## 📈 Tier Upgrade Decision Framework

```
CURRENT SITUATION                          → ACTION
────────────────────────────────────────────────────────────
API costs consistently over $25/month      → Consider Tier 2
Running more than 5 active agents          → Move to Tier 2 VPS
Have paying clients or live users          → Move to Tier 2
Making $2K+/month from this work           → Move to Tier 3
Running 10+ agents + multiple products     → Move to Tier 3
Desktop GPU available (RTX 3080+)          → Add big Ollama models (saves $40-60/mo)
```

---

## 🎯 Smart Upgrades That Pay For Themselves

Regardless of tier, these moves save more than they cost:

| Upgrade | Cost | Saves | ROI |
|---|---|---|---|
| Ollama instead of API for 70% of tasks | $0 | $30-60/mo in API fees | ♾️ |
| Claude Pro instead of Claude API for personal use | $20 flat | vs $50+ pay-per-token | 2.5x |
| Hetzner VPS vs AWS/DO for OpenClaw | $10 | $15-25/mo vs other hosts | 2x |
| Agent heartbeats at 24h vs 1h | $0 | 24x fewer API calls | ♾️ |
| gpt-4o-mini vs gpt-4o for 80% of tasks | $0 | 20x cheaper per token | 20x |

---

## 🔔 Cost Guardrails (All Tiers)

1. **Always set hard monthly caps** in Anthropic + OpenAI dashboards
2. **Weekly spend check** (5 min): console.anthropic.com + platform.openai.com
3. **Red flag:** Any single agent using >$5/week → investigate immediately
4. **Ollama first** — if a local model can do it, use it
5. **Subscriptions over tokens** for heavy personal use (Claude Pro is the clearest win)

```
TIER 1 CAPS:   Anthropic $20 | OpenAI $10
TIER 2 CAPS:   Anthropic $40 | OpenAI $35
TIER 3 CAPS:   Anthropic $60 | OpenAI $55
```

---

## 🏁 Starting Position

Omar is currently set up for **Tier 1**.
Moving to Tier 2 or 3 is straightforward — it's mostly:
1. Upgrade subscriptions (Cursor Pro, Gemini Advanced, Vercel Pro)
2. Move OpenClaw from local Docker → VPS
3. Increase API spend caps
4. Pull heavier Ollama models (if desktop GPU rig available)

*The architecture doesn't change — just the limits do.*

---

*Last updated: 2026-03-07 | Session 001*
*Cross-reference: `~/ai-stack-setup/PLAN.md` for setup phases*
