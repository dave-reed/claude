# RWX — Company Profile

## Product: Mint CI/CD

RWX builds **Mint**, a CI/CD platform that replaces traditional linear pipeline tools (CircleCI, Jenkins, GitHub Actions, Buildkite) with a DAG-based execution engine and content-based caching layer. The result: 2–5x faster builds, 50–90% lower compute costs, and a developer experience engineers actually enjoy.

### How It Works

1. **DAG Execution** — Pipelines are expressed as task graphs. Tasks run in parallel automatically, based on dependency order — no manual parallelization config required.
2. **Content-Based Caching** — Tasks are cached by content, not by manual cache keys. If inputs + command haven't changed, the result is reused. No stale cache. No race conditions. No cache key management.
3. **Serverless Autoscaling** — Compute scales to exactly what the pipeline needs, per task. Pay per second. No idle runners. No per-user fees. No credits system.
4. **Local CLI** — The same run definition executes locally, enabling engineers to iterate without pushing. No "push-and-pray."
5. **Semantic Outputs** — Structured output (test failures, compiler errors) readable by humans and AI agents alike.

### Key Differentiators vs. Category

| Feature | RWX | GitHub Actions | CircleCI | Jenkins | NX |
|---|---|---|---|---|---|
| Content-based caching | ✅ Automatic | ❌ Manual keys | ❌ Manual keys | ❌ Manual keys | ✅ Build-only |
| DAG execution | ✅ | ❌ Linear jobs | ❌ Parallel jobs only | ❌ | ✅ Build-only |
| Full CI/CD scope | ✅ Build+Test+Deploy | ✅ | ✅ | ✅ | ❌ Build only |
| Local CLI parity | ✅ | ❌ | ❌ | ❌ | Partial |
| Serverless autoscaling | ✅ | ❌ Metered runners | Partial | ❌ Self-hosted | ❌ |
| Monorepo + polyrepo | ✅ | Partial | Partial | Partial | Monorepo only |
| Per-second billing | ✅ | ❌ Per-minute | ❌ Credits | ❌ Self-hosted | N/A |

---

## Founding Story

Founded by **Dan Manges** (ex-CTO Root Insurance, Braintree) and **Tommy Graves**. The platform emerged from real pain: Root Insurance's engineering team rebuilt CI/CD from scratch and found the category fundamentally broken. RWX is the productized version of that work — blending deep infrastructure expertise with a focus on developer happiness.

Contact: dan@rwx.com

---

## Proof Points & Customer Results

| Customer | Outcome | Migrated From |
|---|---|---|
| ClickFunnels | 14x reduction in deploy cycle times, $60K+ infrastructure savings | Enterprise CI |
| Tropic | 67% CI runtime reduction, 3x faster PR-to-deploy velocity | GitHub Actions |
| Healia Health | Shipping frequency: 1–2x/day → 4–6x/day | — |
| Anonymous (75-person team) | "My mind is blown at DAG structure for CI/CD" | CircleCI |
| Anonymous (35-person team) | Build times: 30 min → 7 min | — |
| Verkada | Customer (2,000 employees, 539 engineers) | — |
| PayNearMe | Customer (250 employees, 58 engineers) | — |
| Bonusly | Customer | — |

**Aggregate metrics (sales deck):**
- 90% of companies evaluating RWX choose it
- 35% average cost reduction migrating from other platforms
- 90% max cost savings with monorepos
- 10x faster pipeline development iteration

---

## Deal Profiles by Segment

### SMB (20–200 employees, 5–50 engineers)
- **Deal driver:** Founder or CTO feeling infrastructure cost pain or slow iteration speed
- **Sales motion:** Fast PoC → side-by-side perf report → close
- **Champion:** Director of Engineering or Founder/CTO
- **Typical pain:** CircleCI bills growing, build times 30–60 min, engineers complaining
- **Close signal:** They do the PoC and see the number

### Mid-Market (200–1,000 employees, 50–200 engineers)
- **Deal driver:** VP Engineering initiative to improve developer productivity or cut infra spend
- **Sales motion:** Discovery → PoC → champion-driven internal sell → close
- **Champion:** Director of Platform Engineering or Staff Engineer
- **Typical pain:** GitHub Actions at scale, flaky test management, monorepo sprawl
- **Close signal:** Platform team gets internal sponsor

### Enterprise (1,000+ employees, 200+ engineers)
- **Deal driver:** Platform team mandate from VP/SVP Engineering
- **Sales motion:** Longer discovery → pilot on one team → expand
- **Champion:** Staff/Principal Engineer or DevOps Lead
- **Typical pain:** Jenkins legacy, multi-year technical debt in CI/CD infra, build cost optimization initiative

---

## Reference Customers (Name-Droppable)
- Verkada (security surveillance tech, 2,000 employees)
- ClickFunnels (SaaS, 469 employees)
- Tropic (spend management SaaS, 300 employees)
- PayNearMe (fintech/payments, 250 employees)
- Bonusly (HR tech, 87 employees)
- Healia Health (healthcare tech)
- Honeycomb (observability)
- nCino (banking tech)
- Avant (fintech)
