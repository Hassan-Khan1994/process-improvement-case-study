# 02 · Measure — Current-State Analysis

## As-Is Process (with time per step)

```
Invoice received (email)      → 0.5 day   (manual download, save to shared drive)
Manual data entry             → 1 day     (re-keyed into finance system)
Match to PO & GRN             → 2 days    (manual lookup, often incomplete)
Route to approver (email)     → 3 days    (unclear who; sits in inboxes)
Approver reviews & approves   → 4 days    (no reminders; batch reviews weekly)
Post for payment              → 1.5 day   (manual posting)
─────────────────────────────────────────
Total average cycle time      ≈ 12 days
```

## Baseline Metrics (measured over 3 months, 480 invoices)

| Metric | Value |
|--------|-------|
| Average cycle time | 12.0 days |
| On-time approval (≤ agreed SLA) | 62% |
| Rework rate (returned/corrected) | 21% |
| Invoices with missing PO/GRN match | 34% |
| Early-payment discounts captured | 18% |

## Key Observations
- The **routing** and **approver review** steps consume **~7 of 12 days** — the biggest opportunity.
- **Manual data entry and matching** introduce errors that drive a 21% rework rate.
- No **reminders or visibility** — invoices sit unseen in inboxes.

## Data Collection Method
- Extracted timestamps from the finance system and email logs.
- Sampled 480 invoices across three months for cycle-time and rework analysis.
