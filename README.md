# Demo Items

## Week 3

### ✅ Completed

| Ticket | Description |
|:---|:---|
| [![BILL-441](https://img.shields.io/badge/BILL--441-done-brightgreen)](#) | Wallet balance exhaustion moved to invoice adjustment, reducing load on Portal-API. |
| [![BILL-426](https://img.shields.io/badge/BILL--426-done-brightgreen)](#) | Billing and RPM test cases now run automatically, with Slack notifications on completion. Triggered after RC-cut, before PROD deploy — no manual effort required. |
| [![BILL-117](https://img.shields.io/badge/BILL--117-done-brightgreen)](#) | Billing jobs now run on one dedicated worker instead of every server copy, so scaling servers no longer multiplies the load. |
| [![BILL-79](https://img.shields.io/badge/BILL--79-done-brightgreen)](#) | Media usage now checks the account's real wallet balance and hold status directly, instead of relying on a per-key flag that could go stale. |

---

### 🔍 In Code Review

| Ticket | Description |
|:---|:---|
| [![BILL-458](https://img.shields.io/badge/BILL--458-review-yellow)](#) | `postpaid_invoices.tax_usd` never backfilled — always shows `$0.00` even when Stripe charges real tax. |

---

### 🚧 In Progress

| Ticket | Description |
|:---|:---|
| [![BILL-122](https://img.shields.io/badge/BILL--122-in--progress-blue)](#) | Spend report should account for free-credit usage in the monthly reports. |
| [![BILL-461](https://img.shields.io/badge/BILL--461-in--progress-blue)](https://linear.app/flexai/issue/BILL-461/kafka-poc) | **Kafka Setup — POC** |

---

## Week 2

### ✅ Done

| Ticket | Description |
|:---|:---|
| [![BILL-422](https://img.shields.io/badge/BILL--422-done-brightgreen)](#) | Suppress `KeyAbusePatternDetected` alerts for automation users. |
| [![BILL-140](https://img.shields.io/badge/BILL--140-done-brightgreen)](#) | Token service: consume stored FlexAI price from artifacts instead. |
| [![BILL-75](https://img.shields.io/badge/BILL--75-done-brightgreen)](#) | Fix stale tax zone on postpaid invoice charges after a billing cycle. |
| [![BILL-148](https://img.shields.io/badge/BILL--148-done-brightgreen)](#) | Activate postpaid usage billing (Layer 1 wire loop) — enable flags in staging. |
| [![BILL-150](https://img.shields.io/badge/BILL--150-done-brightgreen)](#) | Revenue tracker: pending optimizations. |
| [![BILL-88](https://img.shields.io/badge/BILL--88-done-brightgreen)](#) | Add postpaid usage option to billing page (behind feature flag). |

---

## Week 1

### ✅ Done

| Ticket | Description |
|:---|:---|
| [![ENG-1904](https://img.shields.io/badge/ENG--1904-done-brightgreen)](#) | **Bypass Topup With 0.5 USD** — Fixed: `Team QA Prod Automation's Workspace` User Only Can Recharge 0.5 USD to Bypass Costly Recharges For Testing Purpose. |
| [![ENG-1823](https://img.shields.io/badge/ENG--1823-done-brightgreen)](#) | **RPM Improvement, Audio and Image To Use Key's RPM** — Audio and image endpoints now read the key's configured `rpm_limit` instead of falling back to the tier-default constant of 100 RPM. Elevated quotas set by admins now apply uniformly across chat, audio, and image requests on a shared key. |
| [![ENG-1860](https://img.shields.io/badge/ENG--1860-done-brightgreen)](#) | **Admin UI Shows Archived Orgs** — Fixed it: Admin -> Users Now Don't Show Archived Orgs and View is Much Cleaner Now. |
| [![ENG-1903](https://img.shields.io/badge/ENG--1903-done-brightgreen)](#) | **Admin UI Orgs Show Hardcoded 100 Data** — Added pagination now: Admin Orgs Now is Paginated Giving Better User Experience. |
| [![ENG-1691](https://img.shields.io/badge/ENG--1691-done-brightgreen)](#) | Current Status: [tokens.flex.ai/admin](https://tokens.flex.ai/admin)<br>Bug: [ENG_1691_Data](https://github.com/sray-flex-ai/ENG_1691_Data)<br>Fixed Status: [tokens-dev.flexsystems.ai/admin](https://tokens-dev.flexsystems.ai/admin) |
| [![BILL-149](https://img.shields.io/badge/BILL--149-done-brightgreen)](#) | **Billing and RPM Test Automation** — Current Status: [workflow](https://github.com/flexaihq/automation/actions/workflows/token-service-billing-rpm-tests.yml)<br>Sample Run: [logs](https://github.com/flexaihq/automation/actions/runs/30251555196/job/89930512176#logs)<br>Sample Test Status: `test_partial_refund_reduces_balance_by_exactly_the_refunded_amount` |
