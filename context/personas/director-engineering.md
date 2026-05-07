# Persona: Director of Engineering / Staff Engineer

---

## Who They Are

**Titles:** Director of Engineering, Director of Platform Engineering, Staff Engineer, Principal Engineer, Engineering Manager (Platform/Infrastructure)
**Company size:** 50–2,000 employees; typically managing 5–30 engineers or acting as individual technical lead
**Background:** Deeply technical; has personally felt the pain of slow CI/CD; often the one who maintains pipelines
**Role in deal:** Usually the **champion** — they want RWX, but need VP Eng or Founder to sign off on budget

**ICP examples from our accounts:**
- Director of Engineering at ClickFunnels (migrated from enterprise CI, 14x speed improvement)
- Director of Devops at Tropic (67% runtime reduction)
- Staff Engineer at Grid (57 employees)
- Director of Engineering at Curri (195 employees)

---

## What They Care About

### Primary Goals
1. **Feedback loops:** They write and review code daily; every minute waiting for CI is a minute lost
2. **No more pipeline babysitting:** Flaky tests, cache misses, random failures — they're tired of it
3. **Engineer respect:** If they introduce a tool engineers love, they're a hero. If it sucks, they hear about it.
4. **Career credibility:** Championing a successful migration is a career win. Championing a failed one is not.

### How They Measure Success
- Time from commit to test feedback (target: <5 minutes for unit tests, <15 for full suite)
- Number of pipeline-related engineer interruptions per week
- Cache hit rate (content-based caching reduces this dramatically)
- Hours/week spent maintaining pipelines (should approach zero)

### Decision Criteria
- **Technical credibility first:** They want to understand how it works before they advocate for it
- **Local CLI is a key feature:** Being able to iterate locally without pushing is the single biggest DX win
- **Proof, not promises:** They'll run the PoC themselves and form their own opinion
- **Internal selling:** They need help packaging the ROI for their VP Eng or Founder

---

## How They Buy

- Evaluates technically first (PoC, GitHub repos, documentation)
- Not the final decision maker — needs to bring a business case up
- Timeline: 2–6 weeks to internal decision after champion is convinced
- **Key to winning:** Help them build the internal sell. Give them the ROI numbers. Make them look smart.
- Entry point: GitHub, documentation, engineering blogs, conference talks, word of mouth

---

## Attention Triggers (What Gets a Reply)

1. A specific technical pain they've felt: "Cache misses eating your build reliability? We've solved that."
2. An engineer at a company they respect vouching for RWX
3. The local CLI: "Run your full pipeline locally in 15 minutes — no pushes required."
4. The semantic output story: "See only the failing tests. Not 10,000 lines of logs."
5. A specific GitHub repo signal: "Saw your Jenkinsfile in [repo] — we can eliminate that entire maintenance burden."

---

## Outreach Hooks by Signal

| Signal | Opening Hook |
|---|---|
| DevOps role posted | "Saw [Company] is hiring a Platform Engineer — usually signals a tooling investment. Before the role is filled and patterns are set, might be worth a look at RWX." |
| Jenkins Jenkinsfile in repo | "Found [Company]'s Jenkinsfile in [repo] — that usually means 5+ hrs/week of pipeline maintenance. We eliminate that entirely. Quick 15 min demo of how?" |
| GitHub Actions + large suite | "Saw [Company]'s GitHub Actions config — complex workflows at that scale usually mean 25–40 min build times and manual cache wrangling. RWX automates both. Worth a look?" |
| Monorepo signal | "Noticed [Company] is running a monorepo — content-based caching in RWX skips rebuilding anything that hasn't changed. Teams see 70–90% fewer redundant builds. Interested?" |
| AI tools in stack | "Saw [Company] is using [Cursor/Copilot] — if engineers are shipping code faster, CI/CD is usually the new bottleneck. RWX is built for exactly this workflow." |

---

## Help Them Sell Internally

When a Director/Staff Eng is sold, give them:
1. **The cost math:** "Here's how to calculate your current CircleCI spend vs. what RWX would cost."
2. **The peer proof:** "Here's what [Tropic/ClickFunnels] saw. Both are [similar profile to your company]."
3. **The risk mitigation:** "We run in parallel for the PoC — no risk to your current pipeline until you're ready."
4. **The migration story:** "We handle the migration. Your team's time investment is ~2–4 hours."

---

## What to Avoid

- Don't skip the technical explanation — they want to understand the mechanism (DAG + content-based caching)
- Don't make it seem like a management/cost play only — the DX story matters to them personally
- Don't require a full RFP or formal process — offer a quick PoC first
- Do acknowledge the migration risk — they're thinking about it even if they don't say it
