# Signal Routing

> Decision tree for what happens when a signal fires. Follow this exactly.

---

## Step 1 — Signal Fires. Check Suppression First.

Before ANY action on a signal, run through this gate:

```
Is this account a current customer?
  → YES: Do nothing. Log the signal. Notify AE if relevant.
  → NO: Continue.

Is there an active opportunity in HubSpot for this account?
  → YES: Notify AE. Do NOT enroll in outbound sequence.
  → NO: Continue.

Has this account been contacted in the last 90 days?
  → YES (replied "not interested"): Suppress for 180 days total. Log.
  → YES (no reply): Check cooldown: 45-day minimum between sequence restarts.
  → NO: Continue.

Is this account in the Do Not Contact list?
  → YES: Suppress permanently. Log.
  → NO: Continue to Step 2.
```

---

## Step 2 — Score the Account

Calculate signal score using [context/signal-library.md](../context/signal-library.md).

Apply combination bonuses where applicable.

```
Score ≥ 60 → P1: Immediate personalized outreach (within 24 hours)
Score 40–59 → P2: Active sequence enrollment (within 48 hours)
Score 25–39 → P3: Nurture sequence (within 1 week)
Score < 25 → P4: Add to watch list. No outreach. Monitor for score increase.
```

---

## Step 3 — Assign ICP Tier

Check account against [context/icp-definition.md](../context/icp-definition.md).

```
Tier 1 ICP → Full outreach (all personas, full sequence)
Tier 2 ICP → Standard outreach (primary buyer persona, shorter sequence)
Anti-ICP → Do NOT pursue. Log reason. Remove from active list.
```

---

## Step 4 — Select Sequence by Signal + Persona

| Signal | Tier 1 — Founder/CTO | Tier 1 — VP Eng | Tier 2 — Director |
|---|---|---|---|
| S01 CircleCI | CircleCI-Founder-5touch | CircleCI-VP-5touch | CircleCI-Director-3touch |
| S02 Jenkins | Jenkins-Founder-5touch | Jenkins-VP-5touch | Jenkins-Director-3touch |
| S03 New Leader | — | NewLeader-VP-5touch | NewLeader-Director-3touch |
| S04 Funding | Funding-Founder-5touch | Funding-VP-5touch | — |
| S05 Headcount | Headcount-Founder-3touch | Headcount-VP-3touch | — |
| S07 AI Tools | AITools-Founder-3touch | AITools-VP-3touch | AITools-Director-3touch |
| S09 DevOps Role | — | Platform-VP-3touch | Platform-Director-3touch |

---

## Step 5 — Cooldown & Re-Routing Rules

### After Sequence Completion (No Reply)
- Wait 90 days minimum
- Re-enroll only if a NEW signal fires (not the same one)
- Upgrade sequence tier if additional signals fire during cooldown

### After "Not Interested" Reply
- Suppress for 180 days
- Log reason in HubSpot
- Remove from active signal watch for that contact

### After Meeting Booked
- Pause all outbound sequences for this account
- Route to AE in HubSpot
- Log signal that drove meeting in outputs/ folder

### After No-Show / Ghost
- Single follow-up email within 24 hours
- If no response in 7 days, restart top-of-sequence with new signal hook (if available)
- If no new signal, wait 45 days

---

## Signal Routing Log Template

When a signal fires and routing decision is made, log here or in outputs/:

```
Date: ___________
Account: ___________
Signal: ___ (Sxx)
Score: ___ pts
Tier: ___
Suppression check: PASS / FAIL (reason: ___)
Action: Enrolled in ___ sequence / Routed to AE / Suppressed / Watch list
Notes: ___________
```
