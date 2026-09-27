# 04 · Improve — Improvement Plan

## Solutions (mapped to root causes)

| Root cause | Solution | Expected impact |
|------------|----------|-----------------|
| Unclear routing | **Automated approval workflow** with rules by amount & department | −3 to −4 days |
| Manual data entry | **OCR / e-invoice capture** into the finance system | −1 day, fewer errors |
| Missing PO/GRN match | **3-way auto-match** (invoice ↔ PO ↔ GRN) with exception flags | −1.5 days, less rework |
| No reminders | **SLA-based reminders & escalation** | fewer stalls |
| Batch reviews | **Continuous approval** via mobile/web queue | smoother flow |

## To-Be Process

```
e-Invoice captured (OCR)   → 0.2 day   (auto-extract, no re-keying)
Auto 3-way match           → 0.3 day   (system matches PO & GRN)
Auto-route by rules        → 0.1 day   (right approver instantly)
Approve (with reminders)   → 3 days    (SLA + escalation; mobile approve)
Auto-post for payment      → 0.4 day   (system posts)
──────────────────────────────────────
Total target cycle time    ≈ 4–5 days
```

## Implementation Steps
1. Configure the approval workflow tool (rules, roles, SLAs).
2. Enable OCR/e-invoice capture and 3-way matching.
3. Pilot with one department for 2 weeks; refine rules.
4. Roll out company-wide with training and comms.

## Risks & Mitigations
- **Adoption:** train approvers; make mobile approval easy.
- **Exceptions:** design a clear exception queue so edge cases don't stall the main flow.
- **Data quality:** validate PO/GRN data before go-live.
