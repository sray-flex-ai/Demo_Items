## ✅ Completed

| Ticket | Description |
|:---|:---|
| [![BILL-441](https://img.shields.io/badge/BILL--441-done-brightgreen)](#) | Wallet balance exhaustion moved to invoice adjustment, reducing load on Portal-API. |
| [![BILL-426](https://img.shields.io/badge/BILL--426-done-brightgreen)](#) | Billing and RPM test cases now run automatically, with Slack notifications on completion. Triggered after RC-cut, before PROD deploy — no manual effort required. |
| [![BILL-117](https://img.shields.io/badge/BILL--117-done-brightgreen)](#) | Billing jobs now run on one dedicated worker instead of every server copy, so scaling servers no longer multiplies the load. |
| [![BILL-79](https://img.shields.io/badge/BILL--79-done-brightgreen)](#) | Media usage now checks the account's real wallet balance and hold status directly, instead of relying on a per-key flag that could go stale. |

---

## 🔍 In Code Review

| Ticket | Description |
|:---|:---|
| [![BILL-458](https://img.shields.io/badge/BILL--458-review-yellow)](#) | `postpaid_invoices.tax_usd` never backfilled — always shows `$0.00` even when Stripe charges real tax. |

---

## 🚧 In Progress

| Ticket | Description |
|:---|:---|
| [![BILL-122](https://img.shields.io/badge/BILL--122-in--progress-blue)](#) | Spend report should account for free-credit usage in the monthly reports. |
| [![BILL-461](https://img.shields.io/badge/BILL--461-in--progress-blue)](https://linear.app/flexai/issue/BILL-461/kafka-poc) | **Kafka Setup — POC** |

---
