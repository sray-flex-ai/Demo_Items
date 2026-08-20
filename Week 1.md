# Demo Items 

### ENG-1904 — Bypass Topup With 0.5 USD
**Status:** Done
  - **Fixed** `Team QA Prod Automation's Workspace` User Only Can Recharge 0.5 USD to Bypass Costly Recharges For Testing Purpose.

### ENG-1823 — RPM Improvement, Audio and Image To Use Key's RPM
**Status:** Done
  - **Fixed** Audio and image endpoints now read the key's configured `rpm_limit` instead of falling back to the tier-default constant of 100 RPM. Elevated quotas set by admins now apply uniformly across chat, audio, and image requests on a shared key.

### ENG-1860 — Admin UI Shows Archived Orgs
**Status:** Done — Fixed it
  - **Fixed in Admin UI** Admin -> Users Now Don't Show Archived Orgs and View is Much Cleaner Now.

### ENG-1903 — Admin UI Orgs Show Hardcoded 100 Data
**Status:** Done — Added pagination now
  - **Fixed** Admin Orgs Now is Paginated Giving Better User Experience

### ENG-1691
**Status:** In Progress

- **Current Status:** https://tokens.flex.ai/admin
- **Bug:** https://github.com/sray-flex-ai/ENG_1691_Data
- **Fixed Status:** https://tokens-dev.flexsystems.ai/admin

### BILL-149 — Billing and RPM Test Automation
**Status:** In Progress
  - **Current Status** https://github.com/flexaihq/automation/actions/workflows/token-service-billing-rpm-tests.yml
  - **Sample Run** https://github.com/flexaihq/automation/actions/runs/30251555196/job/89930512176#logs
  - **Sample Test Status** test_partial_refund_reduces_balance_by_exactly_the_refunded_amount
