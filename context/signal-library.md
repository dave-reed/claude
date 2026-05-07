# Signal Library

> Each signal includes: detection method, point value, decay curve, and first-touch message hook.
> Signals are additive. Combination bonuses noted below.

---

## Tier 1 Signals (High Intent)

### S01 — CircleCI Customer (Confirmed)
- **Points:** 40
- **Decay:** 40 → 20 after 90 days (CircleCI contracts renew annually; urgency fades post-renewal)
- **Detection:** G2 reviews, LinkedIn "CircleCI" in job posts, GitHub Actions migration job posts, engineer LinkedIn profiles listing CircleCI
- **Message hook:** "Saw [Company] is on CircleCI — teams your size are typically spending $8–15K/month on credits and waiting 20–40 min per build. We cut both in half. Worth a quick look?"

### S02 — Jenkins Active Use
- **Points:** 35
- **Decay:** 35 → 25 after 120 days (Jenkins customers move slowly but feel more pain over time)
- **Detection:** GitHub repos with Jenkinsfile, job posts listing Jenkins, BuiltWith / Wappalyzer hits
- **Message hook:** "Noticed [Company] is running Jenkins — modern teams on Jenkins are spending 10+ hours/week on pipeline maintenance. RWX eliminates that overhead. Quick 15 min to show you?"

### S03 — New VP/Director of Engineering Hire
- **Points:** 28
- **Decay:** 28 → 10 after 60 days (new leaders do tooling audits in first 30–60 days; urgency peaks early)
- **Detection:** LinkedIn new role notifications, company blog announcements, job listing removals
- **Message hook:** "Congrats on joining [Company] as [Title] — tooling audits in the first 90 days are table stakes. We've helped a handful of eng leaders in similar positions cut CI/CD costs significantly. Happy to share data if useful."

### S04 — Series B/C Funding Announcement
- **Points:** 30
- **Decay:** 30 → 10 after 60 days (spend decisions cluster in 30–45 days post-close)
- **Detection:** Crunchbase webhook, TechCrunch, LinkedIn posts, press releases
- **Message hook:** "Congrats on the [round] — infrastructure efficiency tends to come into focus right after a raise. We're helping [similar company] run CI/CD at [X]% lower cost. Relevant timing?"

---

## Tier 2 Signals (Moderate Intent)

### S05 — Engineering Headcount Growth +20% (Last 6 Months)
- **Points:** 25
- **Decay:** 25 → 12 after 90 days
- **Detection:** LinkedIn headcount data (Sales Navigator), Clearbit firmographic enrichment
- **Message hook:** "Looks like [Company]'s engineering team has grown significantly — CI/CD pain tends to compound at that pace. We scale effortlessly. Worth a look?"

### S06 — GitHub Actions + Large Test Suite Pain Signals
- **Points:** 22
- **Decay:** 22 → 12 after 60 days
- **Detection:** GitHub repos with complex Actions configs, job posts mentioning "improve CI/CD speed" or "reduce build times," LinkedIn posts complaining about GitHub Actions limits
- **Message hook:** "Saw [Company] is running GitHub Actions at scale — teams your size typically hit the ceiling around [X] engineers. We're 2–5x faster and 50% cheaper. Quick demo?"

### S07 — AI Coding Tools in Stack (Copilot, Cursor, Devin)
- **Points:** 20
- **Decay:** 20 → 10 after 90 days
- **Detection:** Job posts listing Copilot/Cursor/Devin, LinkedIn posts from engineers, GitHub repos with AI tool configs
- **Message hook:** "Noticed [Company] is using AI coding tools — the teams getting the most from them have feedback loops under 5 min. RWX is built specifically for AI-native engineering workflows."

### S08 — Monorepo Adoption Signals
- **Points:** 18
- **Decay:** 18 → 8 after 90 days
- **Detection:** GitHub repos with monorepo structure (Nx config, Turborepo, or single large repo), job posts mentioning monorepo
- **Message hook:** "Saw [Company] is running a monorepo — content-based caching in RWX can cut your rebuild volume by 80%+ on unchanged code. Worth a look?"

### S09 — DevOps / Platform Engineering Role Posted
- **Points:** 15
- **Decay:** 15 → 5 after 45 days (role fills, urgency drops)
- **Detection:** LinkedIn Jobs, Greenhouse, Lever job boards
- **Message hook:** "Saw [Company] is hiring a [Platform/DevOps Engineer] — usually signals a tooling investment cycle. RWX might be worth a look before the role is filled and patterns are set."

---

## Tier 3 Signals (Low Intent / Awareness)

### S10 — Conference Attendance (AWS re:Invent, KubeCon, GitHub Universe)
- **Points:** 10
- **Decay:** 10 → 2 after 14 days
- **Detection:** Event attendee lists, LinkedIn check-ins, speaker lists
- **Message hook:** "[Conference] attendee signal only — use to time outreach, not to lead message]"

### S11 — LinkedIn Post About CI/CD Frustration
- **Points:** 15
- **Decay:** 15 → 2 after 7 days (recency matters)
- **Detection:** LinkedIn keyword alerts ("build times," "CI/CD is slow," "Jenkins nightmare," "CircleCI costs")
- **Message hook:** "Saw your post about [specific pain] — we solved exactly that for [similar company]. Worth a quick conversation?"

### S12 — G2 Review of Competitor (Left Negative Review)
- **Points:** 20
- **Decay:** 20 → 10 after 30 days
- **Detection:** G2 review monitoring on CircleCI, Jenkins, GitHub Actions, Buildkite
- **Message hook:** "Saw your review of [Competitor] — looks like [specific issue] is a sticking point. That's the exact thing RWX was built to solve. Mind if I share how?"

---

## Combination Bonuses

| Signal Combination | Bonus Points | Rationale |
|---|---|---|
| CircleCI (S01) + Funding (S04) | +15 | Budget unlocked + vendor pain = high conversion |
| New Eng Leader (S03) + Headcount Growth (S05) | +12 | Change agent with mandate |
| Jenkins (S02) + AI Tools (S07) | +10 | AI coding velocity hitting legacy CI ceiling |
| Funding (S04) + Platform Role Posted (S09) | +10 | Tooling investment actively underway |
| G2 Negative Review (S12) + CircleCI (S01) | +15 | Actively unhappy = high inbound intent |

---

## Signal Scoring Reference

| Total Score | Priority | Action |
|---|---|---|
| 60+ | P1 — Immediate outreach | Personalized sequence, AE loop-in |
| 40–59 | P2 — Active pursuit | Signal-specific sequence, 5-touch |
| 25–39 | P3 — Monitor | Nurture sequence, 3-touch, track for upgrades |
| <25 | P4 — Hold | Add to watch list, no active outreach |

---

## Signal Performance Log

> Update after each campaign with reply rates by signal. Last updated: ___

| Signal | Sequence Sent | Replies | Reply Rate | Meetings | Notes |
|---|---|---|---|---|---|
| S01 CircleCI | — | — | — | — | — |
| S02 Jenkins | — | — | — | — | — |
| S03 New Leader | — | — | — | — | — |
