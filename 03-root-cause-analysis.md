# 03 · Analyze — Root-Cause Analysis

## Pareto Analysis (delay drivers)
Data: [`data/pareto-data.csv`](data/pareto-data.csv)

```
Unclear approval routing    ████████████████████  35.0%   ┐
Manual data entry errors    █████████████         22.9%   │ 75% of delay
Missing PO/GRN match        ██████████            17.1%   ┘ (the "vital few")
No reminders / follow-up    ███████               12.1%
Batch (weekly) reviews      ████                   7.9%
Other                       ███                    5.0%
```

**80/20 insight:** Just **three causes drive ~75%** of delays — unclear routing, manual entry, and missing PO/GRN match. Fixing these yields most of the benefit.

## Fishbone (Ishikawa) — "Why are approvals slow?"

```
   People                Process                 Technology
      │                     │                        │
 unclear owner ──┐   manual routing ──┐    no workflow system ──┐
 batch reviews ──┤   no SLA/reminders ┤    email-based ─────────┤──► SLOW
                 │   manual matching ─┤    no PO/GRN link ──────┘   APPROVALS
   Data                  Environment
      │                     │
 missing PO/GRN ──┘   inboxes as queues ──┘
```

## 5 Whys (for the top cause: unclear routing)
1. **Why** do invoices sit for days? → No one knows who should approve.
2. **Why** is the approver unclear? → Routing is manual and rule-free.
3. **Why** is routing manual? → No workflow system; it's done by email.
4. **Why** is it done by email? → No approval tool was ever configured.
5. **Why** was none configured? → The process grew ad-hoc without ownership.
> **Root cause:** absence of an automated, rule-based approval workflow with clear ownership.

## Conclusion
Target the **vital few**: automate routing, reduce manual entry/matching, and add SLA reminders.
