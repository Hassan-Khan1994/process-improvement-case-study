# 01 · Define — Problem Statement & SIPOC

## Problem Statement
> The invoice approval process at Vantage Services takes an average of **12 days** (target: ≤ 5), with only **62%** approved on time. This delays supplier payments, forfeits early-payment discounts, and damages vendor relationships. The goal is to reduce average cycle time to **5 days** and on-time approval to **≥ 90%** within one quarter.

## Goal Statement (SMART)
- **Specific:** Reduce invoice approval cycle time.
- **Measurable:** From 12 → 5 days; on-time from 62% → ≥ 90%.
- **Achievable:** Via workflow automation and clearer routing.
- **Relevant:** Protects cash flow and vendor trust.
- **Time-bound:** Within one quarter (12 weeks).

## Scope
- **In scope:** Invoice receipt → validation → approval → posting for payment.
- **Out of scope:** Vendor onboarding, actual payment disbursement, contract negotiation.

## SIPOC

| Suppliers | Inputs | Process | Outputs | Customers |
|-----------|--------|---------|---------|-----------|
| Vendors | Invoice, PO, GRN | Receive → Validate → Route → Approve → Post | Approved invoice, payment record | Finance, Vendors |
| Procurement | Purchase orders | | Exceptions/queries | Managers |
| Warehouse | Goods receipt notes | | Audit trail | Auditors |

## Project CTQs (Critical to Quality)
1. Approval cycle time ≤ 5 days
2. On-time approval ≥ 90%
3. Rework/rejection rate ≤ 10%
