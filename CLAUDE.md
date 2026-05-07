# RWX GTM Repository — CLAUDE.md

> This file is the primary context layer. Claude reads it automatically at session start.
> It should be scannable in under two minutes. For deeper detail, reference the context files linked below.

---

## Company

**RWX** builds Mint, a CI/CD platform for high-velocity engineering teams. Founded by Dan Manges (ex-CTO Root Insurance / Braintree) and Tommy Graves. Headquartered in Columbus, Ohio.

**One-line pitch:** RWX provides CI/CD tools and cloud infrastructure that unlock the speed of AI-powered engineering teams.

**Website:** rwx.com | **Pricing:** Pay per second, no per-user fees, no credits system

---

## ICP Summary

**Sweet spot:** B2B SaaS companies with 20–500 employees, 5–100 engineers, running at least one of: CircleCI, Jenkins, GitHub Actions at meaningful scale.

**Tier 1 (highest priority):** 20–200 employees, 5–50 engineers, Fintech / Insurtech / SaaS, previous vendor = CircleCI or Jenkins, pain = slow/expensive builds.

**Tier 2:** 200–2,000 employees, 50–200 engineers, established SaaS, GitHub Actions at scale, beginning to feel monorepo or test-suite pain.

**Anti-ICP:** <5 engineers, non-tech companies, pre-product stage, no CI/CD in use.

→ Full definition: [context/icp-definition.md](context/icp-definition.md)

---

## Signal Scoring (Top Signals)

| Signal | Points | Source |
|---|---|---|
| CircleCI customer (confirmed) | 40 | G2, LinkedIn, job posts |
| Jenkins active use | 35 | GitHub repos, job posts |
| Series B/C announced (last 60 days) | 30 | Crunchbase |
| New VP/Director of Engineering hire | 28 | LinkedIn |
| Engineering headcount +20% (last 6 months) | 25 | LinkedIn |
| GitHub Actions + large test suite pain signals | 22 | GitHub, job posts |
| AI coding tools in stack (Copilot, Cursor, Devin) | 20 | Job posts, LinkedIn |
| Monorepo adoption signals | 18 | GitHub, job posts |
| DevOps/Platform Eng role posted | 15 | Job boards |
| Conference attendance (AWS re:Invent, KubeCon) | 10 | Event lists |

**Combination bonus:** CircleCI customer + funding event = +15 pts. New Eng leader + headcount growth = +12 pts.

→ Full signal library: [context/signal-library.md](context/signal-library.md)

---

## Current Positioning

**Primary message:** "CI/CD for high-velocity teams. 2–5x faster builds, 50% lower costs."

**What we lead with by persona:**
- VP Engineering: cost reduction + developer productivity (time-to-merge, pipeline reliability)
- Founder/CTO: speed to ship, infrastructure cost as % of revenue
- Director of Engineering: feedback loop speed, engineer satisfaction, no more "push-and-pray"

**What we NEVER say:** We don't say "we're like CircleCI but faster." We reframe the category. We say "CI/CD reimagined from first principles."

→ Full positioning: [context/positioning.md](context/positioning.md)

---

## Team Structure

| Role | Owner |
|---|---|
| Founders / AE | Dan Manges, Tommy Graves |
| GTM / Sales | David Reed |
| ICP Research & Sequences | Claude (via this repo) |

---

## This Week's Priorities

> Update this section every Monday (5 min). Keep it to 3–5 bullet points.

- [ ] Update week of: _______________
- [ ] Top priority:
- [ ] Campaign in flight:
- [ ] Accounts in active research:
- [ ] Blocker:

---

## Repo Quick Reference

```
CLAUDE.md                    ← You are here (the brain)
context/
  profile.md                 ← Company + product + deal profiles
  icp-definition.md          ← Tier definitions, must-haves, red flags
  signal-library.md          ← Signal index with scores, decay, hooks
  positioning.md             ← Messaging matrix, value pillars, what NOT to say
  competitor-radar.md        ← Win/loss patterns by competitor
  personas/
    vp-engineering.md
    founder-cto.md
    director-engineering.md
workflows/
  enrichment.md              ← Data waterfall, source priority, field requirements
  signal-routing.md          ← Decision tree: signal fires → what happens next
  campaign-build.md          ← Campaign process, QA checklist, review schedule
outputs/                     ← Historical archive of research briefs + campaign briefs
```
