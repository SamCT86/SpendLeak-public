# SpendLeak

**Paid Traffic Integrity Assurance for performance teams.**

SpendLeak is a focused, one-off audit that helps agencies and marketing teams verify where paid-traffic destinations actually resolve, capture what changed, and leave with a reviewed, client-forwardable record.

**Live product:** https://spendleak.co.uk  
**Sample report:** https://spendleak.co.uk/sample-report

## Product contract

- one brand/domain per audit
- up to 50 paid destinations
- evidence captured from the destination path
- supplied context kept separate from observed evidence
- reviewed findings before delivery
- prioritised actions in a frozen report
- one eligible follow-up comparison after remediation
- £199 GBP one-off
- no ad-account write access
- no recurring monitoring subscription

Typical use cases include paid-media account takeovers, site migrations, launches, landing-page changes and unexplained performance drops where teams need a dated view of what happened after the click.

## What this public repository is

This repository is the **public product and engineering surface** for SpendLeak. It exists to make the product, architecture and engineering approach inspectable without publishing the proprietary production implementation.

The production source repository, infrastructure configuration, provider integrations, operational workflows, database implementation and internal runbooks remain private by design.

That boundary is intentional: **publicly understandable, privately defensible.**

## Engineering overview

SpendLeak is built as a small production system rather than a static landing page. At a high level it includes:

- a customer-facing web and checkout flow
- bounded audit intake and destination evidence collection
- explicit separation between machine observation and human judgement
- reviewed/frozen report generation
- private report delivery
- a bounded follow-up/recheck path
- fail-closed operational and provider-state handling

See [`docs/architecture.md`](docs/architecture.md) and [`docs/engineering-principles.md`](docs/engineering-principles.md).

## Current status

SpendLeak is live. Checkout availability, current price and product terms are always governed by the live product rather than this repository.

See [`STATUS.md`](STATUS.md) for the public status boundary.

## Repository policy

This is **not an open-source distribution of the production application**. No license to proprietary SpendLeak source code, private infrastructure or internal implementation is granted by this repository.

Security reports should not include secrets or personal data in public issues. See [`SECURITY.md`](SECURITY.md).
