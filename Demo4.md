# Billing – Project Status

## ✅ Completed / Done

| Ticket | Description |
|---|---|
| [BILL-441](#) | Wallet balance exhaustion moved to invoice adjustment, reducing load on Portal-API. |
| [BILL-426](#) | Billing and RPM test cases now run automatically, with Slack notifications sent on completion. Triggered after RC-cut, before PROD deploy — no manual effort required. |
| [BILL-117](#) | Billing jobs now run on one dedicated worker instead of on every server copy, so scaling servers no longer multiplies the load. |
| [BILL-79](#) | Media usage now checks the account's real wallet balance and hold status directly, instead of relying on a per-key flag that could go out of date. |

## 🔍 Code Review

| Ticket | Description |
|---|---|
| [BILL-458](#) | `postpaid_invoices.tax_usd` never backfilled — always shows $0.00 even when Stripe charges real tax. |

## 🚧 In Progress

| Ticket | Description |
|---|---|
| [BILL-122](#) | Spend report should take into account the use of free credits in the monthly reports. |
