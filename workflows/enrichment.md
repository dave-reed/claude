# Enrichment Workflow

> Data waterfall for account enrichment. Follow source priority order. Fill required fields before activating any sequence.

---

## Required Fields Before Account Activation

An account is not ready for outreach until all required fields are populated:

| Field | Required | Source Priority |
|---|---|---|
| Company name | ✅ | Manual |
| Website / domain | ✅ | Manual |
| Total employee count | ✅ | LinkedIn → Clearbit → Apollo |
| Engineer count (estimated) | ✅ | LinkedIn Sales Nav → Clearbit → Apollo |
| Current CI/CD tool | ✅ | GitHub (Jenkinsfile/Actions YAML) → G2 → Job posts → Apollo |
| Primary VCS | ✅ | GitHub profile → Job posts |
| Funding stage + last round | ✅ | Crunchbase → PitchBook → LinkedIn |
| Buyer name + title | ✅ | LinkedIn → Apollo |
| Buyer email | ✅ | Apollo → Hunter.io → RocketReach → Clearbit |
| Buyer LinkedIn URL | ✅ | LinkedIn |
| ICP tier (1/2/Anti) | ✅ | Assigned after enrichment |
| Signal score | ✅ | Calculated from signal-library.md |

---

## Source Priority (Data Waterfall)

### Firmographic Data
1. **LinkedIn** (headcount, engineer ratio, growth signals) — most accurate, slowest
2. **Clearbit** (enrichment API, firmographic snap) — fast, moderately accurate
3. **Apollo** (bulk enrichment option) — acceptable accuracy, use for volume
4. **Crunchbase** (funding history, founding date) — authoritative for funding data

### Technographic Data (CI/CD Tool Detection)
1. **GitHub** — check repo for `Jenkinsfile`, `.github/workflows/`, `.circleci/config.yml`, `.buildkite/`
2. **Job postings** — search for "CircleCI", "Jenkins", "GitHub Actions", "Buildkite" in JDs
3. **G2** — look for reviews left by company employees on competitor products
4. **Wappalyzer / BuiltWith** — CI/CD tech detection (limited accuracy, useful signal)
5. **LinkedIn posts** — engineers sometimes post about their stack

### Contact Data
1. **LinkedIn** — name, title, LinkedIn URL (always accurate)
2. **Apollo** — email (primary source; verify before sending)
3. **Hunter.io** — email verification + pattern inference
4. **RocketReach** — fallback if Apollo/Hunter miss
5. **Clearbit** — real-time enrichment for high-priority accounts

---

## Email Infrastructure Requirements

### Domain Setup (Before Any Sending)
- Primary domain: rwx.com (limit: 50 outbound emails/day)
- Sending domain: send.rwx.com (warmed separately)
- Warm-up period: 30 days minimum before volume sending
- Sending limit: Start at 10/day, increase by 10/week, max 100/day per mailbox

### Quality Thresholds
- Email validity: Only send to verified addresses (Apollo confidence >80% or Hunter verified)
- Bounce threshold: Pause sequence if domain bounce rate >3%
- Spam complaint threshold: Pause and review if rate >0.1%

### Unsubscribe / Suppression
- Maintain global suppression list: `/Marketing/Do not contact/`
- Check against: Dan's LinkedIn Connections, HubSpot CRM exports, existing customers
- Suppress all: Current customers, active opportunities (route to AE), contacts who replied "not interested" in last 6 months

---

## Enrichment Quality Check (Before Activating Sequence)

Run this checklist before activating any account:

- [ ] Employee count confirmed from LinkedIn (not just Clearbit estimate)
- [ ] Engineer count estimated (LinkedIn headcount filter: "Engineering" function)
- [ ] CI/CD tool confirmed from at least one source (not just assumed)
- [ ] Buyer email verified (not just pattern-inferred)
- [ ] Account not in suppression list
- [ ] Signal score calculated (minimum 25 to activate)
- [ ] ICP tier assigned
- [ ] Correct sequence selected based on signal + persona

---

## Enrichment Log Template

Use this format when logging enrichment sessions:

```
Date: ___________
Accounts enriched: ___
Tier 1: ___ | Tier 2: ___ | Anti-ICP (excluded): ___
Primary signal driving Tier 1: ___
Data gaps (fields still missing): ___
Actions needed: ___
```
