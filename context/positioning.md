# Positioning

> How RWX talks about itself. What we say, what we don't say, and why.

---

## Core Positioning Statement

**"RWX provides CI/CD tools and cloud infrastructure for unlocking the speed of AI-powered engineering teams."**

Secondary: "The CI/CD platform for high-velocity teams — 2–5x faster builds, 50% lower costs, built from first principles."

---

## Why We Exist (The Category Reframe)

Traditional CI/CD was designed in 2010–2018 for human-paced development. Engineers committed code, waited 30–60 minutes, and moved on to something else. That model is broken now:

1. AI coding tools (Copilot, Cursor) mean engineers generate code 5–10x faster
2. More commits per day = more pipeline runs = exponential compute cost growth
3. 30-minute feedback loops are a bottleneck when AI can write the next PR in 10 minutes
4. Traditional tools (linear job queues, manual cache keys) weren't built for this pace

**RWX's reframe:** We didn't build a faster version of GitHub Actions. We rebuilt CI/CD from first principles for the era of AI-powered engineering.

---

## Value Pillars

### 1. Speed (Primary)
- DAG-based execution: automatic parallelization, zero wasted compute
- Content-based caching: tasks are skipped when inputs haven't changed — no cache keys, no stale data
- Feedback loops compress from 30–60 min → 2–10 min
- **Proof:** ClickFunnels 14x deploy cycle reduction; Tropic 67% runtime reduction

### 2. Cost (Secondary — often leads in ICP discovery)
- Content-based caching eliminates redundant builds (pay for nothing you don't run)
- Per-second billing; no per-user fees; no credits system
- 35% average cost reduction migrating from other platforms; up to 90% with monorepos
- **Proof:** ClickFunnels $60K+ infrastructure savings; anonymous 75-person team off CircleCI

### 3. Developer Experience (Tertiary — champion-builder)
- Local CLI: run the same pipeline spec locally; no "push-and-pray"
- Minimal YAML; DAG execution eliminates boilerplate parallelization config
- Semantic outputs: see only failing tests, not endless raw logs
- Engineers onboard and own pipelines within hours, not days
- **Proof:** "This is the first CI/CD tool I actually enjoy using." — Senior Engineer, 120-person team

### 4. Agent-Native (Emerging — leading edge of positioning)
- Built for workflows where AI generates code and requires immediate validation feedback
- Structured outputs readable by AI agents (not just humans)
- CLI enables agents to run pipelines, iterate, and validate without pushing
- Blog: "Truly continuous integration: ensuring pull requests from agents have passing builds"

---

## Messaging Matrix by Persona

| Persona | Lead With | Proof Point | CTA |
|---|---|---|---|
| Founder/CTO | Infrastructure cost as % of revenue, speed to ship | ClickFunnels $60K savings, 14x cycles | "Free PoC — we produce a cost report" |
| VP Engineering | Developer productivity + cost reduction | Tropic 67% runtime, team morale | "We handle the migration" |
| Director of Engineering | Feedback loop speed, no more babysitting pipelines | Build times 30 min → 7 min | "Demo: local CLI iteration" |
| Staff/Principal Engineer | Local CLI, DAG execution, semantic outputs | "First CI/CD I actually enjoy" | "Try the CLI — 15 min setup" |

---

## What We Say (Approved Language)

- "CI/CD reimagined from first principles"
- "Content-based caching — no keys, no stale data, no race conditions"
- "Pay only for work that actually runs"
- "DAG execution: automatic parallelization, zero waste"
- "Agent-native CI/CD"
- "The platform teams switch to after outgrowing [CircleCI/GitHub Actions/Jenkins]"
- "We run free PoCs and handle the migration for you"
- "50–90% faster pipelines"
- "2–5x faster builds"
- "50% lower CI/CD costs"

---

## What We NEVER Say

| Phrase | Why Not | Use Instead |
|---|---|---|
| "We're like CircleCI but faster" | Positions us as a feature upgrade, not a category shift | "CI/CD reimagined from first principles" |
| "Better than GitHub Actions" | Makes the conversation about them, not us | "Built for teams who've outgrown GitHub Actions" |
| "Enterprise-grade" | Vague, overused | Specific proof points — customer names, metrics |
| "Cutting-edge" / "Next-gen" / "Revolutionary" | Buzzwords that erode credibility | Let the data speak: "67% runtime reduction" |
| "We integrate with everything" | Sounds like a platform sales pitch | Name the specific integrations relevant to the prospect |
| "Our platform..." | Impersonal, enterprise-ish | "RWX" or "Mint" by name |

---

## Objection Handling (Key Scenarios)

### "We're already invested in GitHub Actions"
> "Teams your size typically hit the GitHub Actions ceiling around 20–30 engineers. When build times cross 20 minutes and cache management becomes a part-time job, that's the inflection point. Happy to show you what the delta looks like for a team similar to yours."

### "We just signed a new contract with CircleCI"
> "Totally understand. Most teams we talk to are in the same boat — let me share what the migration timeline looks like so you're ready when renewal comes up. The PoC is free and takes 2 hours."

### "We use NX / Turborepo and it works fine"
> "NX is a build optimizer inside a CI/CD system — you still need GitHub Actions or CircleCI to actually execute and deploy. RWX is the full CI/CD platform. It's the difference between 10% faster and 50–90% faster."

### "How are you different from Buildkite?"
> "Buildkite gives you powerful agent-based infrastructure but you're still managing agents, writing custom cache logic, and maintaining YAML glue. RWX eliminates all of that — content-based caching is automatic, no agents to manage, and you get local CLI parity."

### "What's the migration like?"
> "We handle it. Free PoC: we run your pipeline in RWX in parallel, produce a side-by-side cost and performance report, and you see the numbers before you commit to anything."

---

## Proof Point Quick Reference

| Stat | Source | Use For |
|---|---|---|
| 14x deploy cycle reduction | ClickFunnels | Speed conversations |
| $60K+ infrastructure savings | ClickFunnels | Cost conversations |
| 67% CI runtime reduction | Tropic | Speed + GitHub Actions objection |
| 4–6x daily shipping frequency | Healia Health | Velocity / AI-native story |
| 90% companies evaluating choose RWX | Internal | Confidence / social proof |
| 35% average cost reduction | Internal | Cost conversations |
| 90% max savings with monorepos | Internal | Monorepo leads |
| 10x faster pipeline iteration | Internal | Dev experience conversations |
