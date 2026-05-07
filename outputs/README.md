# Outputs — Historical Archive

This folder stores every research brief, campaign brief, and sequence produced by the GTM repo.

## Purpose

The outputs folder creates a feedback loop:
- Shows how ICP thinking evolved over time
- Tracks which campaigns converted and which didn't
- Surfaces which signals drove meetings vs. which didn't
- Makes it easy to spot patterns across campaigns

## File Naming Convention

```
YYYY-MM-DD_[type]_[campaign-or-account-name].md

Examples:
  2026-05-07_research_tropic.md
  2026-05-07_campaign_circleci-vp-tier1.md
  2026-05-14_sequence_jenkins-founder-5touch.md
```

## File Types

| Type | What Goes Here |
|---|---|
| `research_[account].md` | Account intelligence brief from Account Research skill |
| `campaign_[name].md` | Campaign brief including audience, copy, and results log |
| `sequence_[name].md` | Full email sequence copy (all touches) |
| `win_[account].md` | Post-win debrief — what the champion said, what tipped it |
| `loss_[account].md` | Post-loss debrief — why we lost, what competitor won |

## Maintenance

After every campaign, log results here using the template in [workflows/campaign-build.md](../workflows/campaign-build.md).

After every win or loss, log a debrief to update [context/competitor-radar.md](../context/competitor-radar.md).
