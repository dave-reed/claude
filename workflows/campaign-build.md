# Campaign Build Workflow

> Full process for building a campaign from audience definition through launch and review.

---

## Phase 1 — Audience Definition

### Step 1.1 — Define the Signal / Trigger
What signal is this campaign responding to?
- [ ] Signal identified (from signal-library.md)
- [ ] Signal score threshold defined (minimum to enroll)
- [ ] Suppression rules confirmed

### Step 1.2 — Define the Audience Segment
- [ ] ICP tier (Tier 1 / Tier 2)
- [ ] Persona (Founder/CTO / VP Eng / Director of Eng)
- [ ] Industry filter (if applicable)
- [ ] Company size range (employee count / engineer count)
- [ ] Geography filter (US only / open to international)
- [ ] Estimated audience size: ___ accounts

### Step 1.3 — Enrichment Checkpoint
Before building copy, confirm:
- [ ] Sample of 10 accounts enriched and verified ICP-compliant
- [ ] Email deliverability confirmed (valid emails, domain not flagged)
- [ ] Suppression list checked

---

## Phase 2 — Campaign Brief

Complete this brief before writing any copy:

```
Campaign Name: ___________
Signal: ___ (Sxx from signal-library.md)
Persona: ___________
ICP Tier: ___________
Estimated Audience: ___ accounts
Primary Value Prop: ___________
Proof Point to Use: ___________
CTA: ___________
Sequence Length: ___ touches over ___ days
Owner: ___________
Launch Date: ___________
Review Date: ___________
```

---

## Phase 3 — Sequence Copy

### Touch Structure (5-Touch Default — Tier 1)

**Touch 1 — Day 1 (Signal Hook)**
- Subject: Short, specific, signal-relevant
- Body: 3–4 sentences max. Lead with the signal. Connect to a proof point. One CTA.
- Personalization: Company name, specific signal observed, proof point from similar company

**Touch 2 — Day 4 (Value Shift)**
- Subject: Different angle from Touch 1
- Body: Different value pillar than Touch 1. Include a stat or customer result.
- Personalization: Reference any engagement from Touch 1 (if applicable)

**Touch 3 — Day 8 (Peer Proof)**
- Subject: Name a reference customer
- Body: Short case study excerpt. What they were doing, what they switched to, what changed.
- Personalization: Pick reference customer in same industry or similar size

**Touch 4 — Day 14 (Risk Reduction)**
- Subject: Address the objection (migration risk, contract lock-in, etc.)
- Body: "We run the PoC in parallel — no risk to your current pipeline."
- Personalization: Address the most common objection for this persona

**Touch 5 — Day 21 (Low-Friction Ask)**
- Subject: Short, direct
- Body: One sentence. "Worth a quick look?" or "Is this even on your radar?" — give them an easy out.
- Personalization: Minimal — this is a breakup email pattern

### Touch Structure (3-Touch Default — Tier 2)

**Touch 1 — Day 1:** Signal hook + proof point + CTA
**Touch 2 — Day 6:** Peer proof (reference customer)
**Touch 3 — Day 14:** Low-friction ask / breakup

---

## Phase 4 — QA Checklist (Before Launch)

### Copy QA
- [ ] No spelling errors or broken variables ({{company}}, {{first_name}} resolve correctly)
- [ ] Tone check: Does this sound like a human wrote it? Not like a press release?
- [ ] Approved language used (see positioning.md — "What We Say")
- [ ] No banned phrases (see positioning.md — "What We NEVER Say")
- [ ] CTA is singular and clear (one ask per email)
- [ ] Proof point is accurate (verify stat against profile.md)

### Technical QA
- [ ] Sending domain is warmed (check sending limits)
- [ ] Suppression list loaded
- [ ] Test send completed and reviewed in inbox
- [ ] Sequence timing confirmed (no sends on weekends unless approved)
- [ ] Reply routing confirmed (replies go to monitored inbox)

### Approval
- [ ] Copy reviewed by: ___________
- [ ] Launch approved by: ___________

---

## Phase 5 — Launch

**Ramp schedule:** Do not blast full audience on Day 1.
- Day 1: 10% of audience (validation batch)
- Day 3: Check bounce rate (<3%) and complaint rate (<0.1%); pause if exceeded
- Day 5: 50% of audience if Day 3 metrics clear
- Day 10: Full audience if metrics remain clean

---

## Phase 6 — Review Schedule

**Weekly (first 4 weeks):**
- Open rate, reply rate, meeting rate
- Bounce rate (flag if >3%)
- Best-performing touch (which email drove replies?)

**At sequence completion:**
- [ ] Log results in outputs/ folder using campaign log template
- [ ] Update signal-library.md with actual reply rate for signal used
- [ ] Note any messaging that outperformed or underperformed

### Campaign Log Template (Save to `outputs/`)

```
Campaign: ___________
Signal: ___________
Persona: ___________
Launch Date: ___________
Audience Size: ___ accounts

Results:
  Touch 1 open rate: ___% | reply rate: ___%
  Touch 2 open rate: ___% | reply rate: ___%
  Touch 3 open rate: ___% | reply rate: ___%
  Total replies: ___
  Meetings booked: ___
  Meeting rate: ___%

Signals that drove meetings: ___________
Best-performing touch: Touch ___
Best subject line: ___________
Calls to action that worked: ___________
What to change next time: ___________
```
