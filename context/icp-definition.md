# ICP Definition

> Last reviewed: May 2026 | See evolution log at the bottom for changes over time.

---

## Tier 1 — Core ICP (Highest Priority)

**Profile:** Fast-growing B2B SaaS companies where engineering velocity is a competitive differentiator and CI/CD is a known pain point.

### Firmographic Criteria
- **Employee count:** 20–200
- **Engineer count:** 5–50
- **Growth rate:** 20%+ headcount growth in last 12 months (or recent funding event)
- **Funding stage:** Seed+ (typically Series A or B)
- **Geography:** US-first; open to Canada, EU

### Technographic Signals
- Active CircleCI or Jenkins customer (strongest indicator)
- GitHub as primary VCS
- Using Docker for containerized builds
- Any AI coding tool in stack (Copilot, Cursor, Devin, Cody) — indicates velocity pressure

### Organizational Signals
- Dedicated DevOps, Platform Engineering, or SRE function exists
- Engineering headcount growing faster than revenue headcount
- CTO or VP Engineering in an active hiring mode (job posts visible)

### Industries (Highest Concentration in ICP)
- Fintech / Insurtech
- B2B SaaS (vertical software)
- Healthcare tech / HealthTech
- Marketing tech / Data platforms
- Logistics / Supply chain software

### Buyer Titles (Tier 1)
- Founder/CTO (companies <50 employees)
- VP of Engineering (companies 50–500 employees)
- Director of Engineering
- Director of Platform Engineering

---

## Tier 2 — Strong Fit (Active Pipeline)

**Profile:** Mid-market engineering organizations with established CI/CD infrastructure beginning to feel performance or cost ceiling.

### Firmographic Criteria
- **Employee count:** 200–2,000
- **Engineer count:** 50–200
- **Funding stage:** Series B–D or bootstrapped profitable

### Technographic Signals
- GitHub Actions at meaningful scale (10+ pipelines, complex workflows)
- Monorepo with growing test suite (build times exceeding 20 minutes)
- Buildkite or self-hosted Jenkins

### Organizational Signals
- Platform Engineering team (2+ people)
- Recent VP Engineering hire (new leader, often initiates tooling review)
- Open roles for DevOps/Platform Eng signal active infrastructure investment

### Buyer Titles (Tier 2)
- VP of Engineering
- Engineering Manager (Platform/Infrastructure)
- Staff or Principal Engineer

---

## Anti-ICP — Do Not Work

| Signal | Reason to Exclude |
|---|---|
| <5 engineers total | Not enough CI/CD complexity to justify RWX |
| No CI/CD in use at all | Too early; not worth the education cost |
| Non-tech company (e.g., retail, manufacturing) | Wrong buyer context; no engineering-led decisions |
| Pre-revenue / pre-product | No infrastructure spend to justify; wrong stage |
| Using GitLab CI natively (without pain) | Tight integration makes displacement very hard |
| Large enterprise with multi-year Jenkins contracts | Sales cycle too long; change management risk |
| Explicit "happy with current CI/CD" without new leadership | No entry point |

---

## Qualification Framework

### Must-Haves (All Required for Active Pursuit)
- [ ] At least 5 engineers
- [ ] Active CI/CD tool in use
- [ ] Engineering-led buying process (not IT-procurement-led)
- [ ] At least one of: cost pain, build speed pain, or new engineering leader

### Strong-to-Have (Any 2+ = Strong Pursuit)
- [ ] CircleCI or Jenkins as current tool
- [ ] Recent funding event (last 90 days)
- [ ] Engineering headcount growing
- [ ] AI coding tools in stack
- [ ] Identified champion (Director+) who controls CI/CD decisions

### Red Flags (Deprioritize if Present)
- Active 12-month+ contract with current vendor and no renewal pain
- IT/procurement-led buying process
- Strong internal objection to cloud-hosted CI/CD (data residency concerns)
- Engineering team is primarily mobile (iOS/Android only — limited CI/CD complexity)

---

## ICP Evolution Log

| Date | Change | Reason |
|---|---|---|
| May 2026 | Added AI coding tools as Tier 1 technographic signal | Teams using AI coding tools ship faster and feel CI/CD lag more acutely — strong leading indicator |
| May 2026 | Set Tier 1 engineer floor at 5 (was 3) | Deals with <5 engineers stall; not enough pipeline complexity to create urgency |
| Initial | Established core ICP based on first 30 closed/lost deals | CircleCI customers closed at 3x the rate of GitHub Actions; Jenkins 2x |
