# Competitor Radar

> Honest win/loss patterns. Updated after each competitive deal. Last updated: May 2026.

---

## Competitor Index
- [GitHub Actions](#github-actions)
- [CircleCI](#circleci)
- [Jenkins](#jenkins)
- [Buildkite](#buildkite)
- [NX / Turborepo](#nx--turborepo)
- [Harness](#harness)
- [GitLab CI/CD](#gitlab-cicd)

---

## GitHub Actions

### We Win When
- Engineering team >15 engineers with complex test suites (>20 min build times)
- Monorepo or multi-service architecture creating caching/parallelization pain
- Team is frustrated with manual cache key management and stale builds
- AI coding tools are in the stack and feedback loop speed is a priority
- Champion is an engineer (not just management) who's felt the pain personally

### We Lose When
- Team is <10 engineers with simple, fast pipelines
- GitHub-native integration is considered a feature (single platform preference)
- No one owns pipeline performance — "it's fine" inertia
- Procurement requires staying within GitHub ecosystem

### Key Differentiators
- Content-based caching (automatic) vs. GitHub's manual cache keys (fragile, stale-prone)
- DAG execution vs. linear job queues
- Local CLI iteration vs. push-to-test loop
- Per-second billing vs. per-minute runner minutes (30% lower effective cost at scale)

### Objection to Use
> "GitHub Actions is free/included in our GitHub plan."
> Response: "It's not free at scale — runner minutes at 10,000+ minutes/month add up fast. We've shown teams your size saving $2–4K/month after switching. And the productivity gain from 2–5x faster builds is hard to put a number on, but engineers feel it immediately."

### Win Language
- "Built for Scale, Not Side Projects"
- "No manual cache keys → RWX infers caches by file + command content"
- "No idle runner tax → you pay only for executed tasks"

---

## CircleCI

### We Win When
- CircleCI credit costs have grown >$5K/month and VP Eng is reviewing spend
- Team is hitting CircleCI's parallelization limits or dealing with flaky cache keys
- Contract is up for renewal (30–60 days out)
- CircleCI downtime / reliability incidents are fresh in buyer's mind
- Recent G2 review left by someone at company shows frustration

### We Lose When
- Contract just renewed (12 months locked in, urgency gone)
- CircleCI is deeply integrated with their deploy process (custom orbs, extensive configuration)
- No internal champion willing to advocate for the switch

### Key Differentiators
- RWX is ~35% cheaper on compute at equivalent workloads
- No credits system — per-second billing is more predictable
- Content-based caching eliminates 40–80% of redundant task runs that CircleCI would bill for
- DAG execution vs. CircleCI's job-level parallelism (coarser-grained)

### Objection to Use
> "We've been on CircleCI for years and everything is configured."
> Response: "We handle the migration — it typically takes 2–4 hours of your team's time. We run in parallel first so you see the delta before you switch anything. The PoC is free."

### Win Language
- "Next-gen CI/CD platform built for speed, efficiency, and scale"
- "Smart caching that works for you — no keys, no stale data, no race conditions"
- "We run free PoCs and handle the migration for you"

---

## Jenkins

### We Win When
- Team is spending 5+ hours/week on Jenkins maintenance (plugin updates, agent management)
- Jenkins is blocking cloud-native or containerized workflows
- New engineering leader inherited Jenkins and sees it as technical debt
- AI coding tools are in play and Jenkins feedback loop is too slow
- Team wants to eliminate self-hosted infrastructure

### We Lose When
- Team has a dedicated infrastructure engineer who "owns Jenkins" and sees it as their domain
- Highly customized Jenkins pipeline that would take significant time to rewrite
- Security/compliance requirements mandate on-prem (not all, but some)
- No budget/appetite for cloud-hosted CI/CD

### Key Differentiators
- Zero infrastructure to manage (serverless vs. self-hosted agents)
- 50–90% faster pipelines without manual optimization
- Modern YAML spec vs. Groovy Jenkinsfile complexity
- Active product development (Jenkins is community-maintained; slow innovation)

### Objection to Use
> "Jenkins is free and we've customized it heavily."
> Response: "Jenkins is free to license, not to run. Factor in the server costs, agent maintenance, and engineer hours — teams your size typically spend $3–8K/month equivalent. And the customization debt compounds. We built a migration path for exactly this."

### Win Language
- "From Legacy to Lightning Fast"
- "Built for 2026, not 2010"
- "Massive speed boost + lower TCO (no servers to manage) + modern local CLI"

---

## Buildkite

### We Win When
- Team is tired of managing Buildkite agents (provisioning, scaling, maintenance)
- Custom cache logic has become a maintenance burden
- Team wants local CLI parity for iteration
- Cost of agent infrastructure + Buildkite licensing is being scrutinized

### We Lose When
- Team has very specific infrastructure requirements that agent-based model serves well (air-gapped, on-prem compliance)
- Buildkite pipeline is deeply customized with plugin ecosystem
- Engineering team strongly prefers "full control" of infrastructure

### Key Differentiators
- No agents to manage (serverless) vs. Buildkite's agent-managed compute
- Automatic content-based caching vs. "Caching as a science project" (custom per-project)
- Local CLI parity vs. push-to-test loop

### Win Language
- "Built to Scale Without the Complexity"
- "RWX gives you the power of Buildkite — without managing agents, writing YAML glue, or debugging custom cache logic"
- "Caching That Isn't a Science Project"

---

## NX / Turborepo

### We Win When
- Team realizes NX only optimizes builds, not full CI/CD pipeline
- Still using GitHub Actions or CircleCI underneath NX — frustrated with the dual-tool setup
- Monorepo build optimization is solved but deploy pipeline is still slow/expensive
- Need polyrepo/microservices support that NX doesn't cover

### We Lose When
- Team is monorepo-only and NX + GitHub Actions is working well enough
- Heavy investment in NX ecosystem (plugins, custom targets)
- Frontend/JS-heavy team already committed to NX toolchain

### Key Differentiators
- RWX is the full CI/CD platform (build + test + deploy); NX is a build optimizer
- Works for polyrepos and microservices; NX is monorepo-only
- RWX is 50–90% faster; NX typically delivers 10–30% improvement
- No need to maintain two tools (NX + underlying CI)

### Win Language
- "Beyond Build & Test Optimization"
- "Mint/RWX is like NX for everything"
- "Stop patching together tools. Full CI/CD with smarter caching and deployment automation."
- "Full CI/CD System vs. NX's Build-Only Optimization"

---

## Harness

### We Win When
- Team is paying Harness seat licenses and not using the full platform
- Harness complexity/overhead is exceeding the team's actual needs
- Cost-conscious buyer who wants "just CI/CD done well" without the platform tax
- Team is skeptical of all-in-one platform lock-in

### We Lose When
- Team is using Harness for feature flags, deployment governance, or compliance workflows beyond CI
- Enterprise with procurement that values single-vendor consolidation
- Dedicated platform team managing Harness with heavy internal investment

### Key Differentiators
- No seat licenses — pay per second for what runs
- No forced bundling — just CI/CD, not a platform suite
- Simpler setup and maintenance

### Win Language
- "Streamlined Power Without Lock-In"
- "No seat licenses. No forced bundling. Just blazing-fast pipelines billed by the second."
- "Pay only for what runs."

---

## GitLab CI/CD

### We Win When
- Team is on GitHub (not GitLab) for VCS and GitLab CI is not native
- GitLab CI YAML complexity is a maintenance burden
- Team wants local CLI iteration (GitLab CI is push-to-test)
- Build performance is the primary pain (GitLab CI has no content-based caching)

### We Lose When
- Team is all-in on GitLab platform (VCS + CI + security scanning in one system)
- GitLab CI's security/compliance scanning features are required
- Single-platform preference (don't want to introduce another tool)

### Key Differentiators
- True DAG execution (GitLab has "needs" keyword but limited)
- Content-based caching (GitLab has none)
- Local CLI parity
- GitHub integration (most RWX ICP uses GitHub, not GitLab)

### Win Language
- "CI/CD Reimagined"
- "True DAG execution → 50–90% faster"
- "Content-based caching → no wasted work"
- "Local runs, breakpoints, interactive" vs. "YAML-heavy, push-to-test, minimal debugging"

---

## Win/Loss Summary Table

| Competitor | Win Rate (estimated) | Primary Win Driver | Primary Loss Driver |
|---|---|---|---|
| CircleCI | High | Cost + renewal timing | Locked-in contracts |
| Jenkins | High | Modernization mandate | Agent owner resistance |
| GitHub Actions | Medium | Scale/perf pain | Small teams, GitHub-native preference |
| Buildkite | Medium | Agent mgmt fatigue | On-prem/compliance requirements |
| NX | High | Full-stack CI/CD need | Monorepo-only, JS ecosystem |
| Harness | Medium | Cost / platform overhead | Enterprise consolidation plays |
| GitLab CI | Medium | GitHub VCS alignment | All-in GitLab shops |
