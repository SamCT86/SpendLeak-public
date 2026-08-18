# SpendLeak

**PPC destination audit for performance agencies.**

Before you own the result, verify where the paid traffic lands.

SpendLeak checks up to 50 paid destinations, captures evidence of what each path actually reaches, keeps supplied context separate from observed evidence, and delivers a human-reviewed, client-forwardable report with one eligible follow-up comparison after remediation.

**Live product:** https://spendleak.co.uk  
**Sample report:** https://spendleak.co.uk/sample-report

## When it is useful

SpendLeak is designed for moments where a performance team needs a dated, defensible view of the post-click path before responsibility becomes ambiguous:

- taking over a new paid-media client
- site migration, relaunch or major web change
- landing-page or destination changes
- unexplained performance drops or destination incidents

## What the audit includes

- one brand/domain per audit
- up to 50 paid destinations
- evidence captured from the destination path
- supplied context kept separate from observed evidence
- reviewed findings before delivery
- prioritised actions in a frozen report
- one eligible follow-up comparison after remediation
- no Google Ads login or ad-account write access required for the core audit
- £199 GBP one-off
- no recurring monitoring subscription

The live product is always the authority for current scope, price, availability and customer-facing terms.

## How SpendLeak treats evidence

The operating principle is simple: **observe first, conclude second.**

Machine-collected destination evidence, customer-supplied context and reviewed findings are deliberately kept as separate stages. Delivered reports are frozen records of a specific audit state; a follow-up creates a comparison rather than rewriting the original evidence.

See [`docs/architecture.md`](docs/architecture.md) for the high-level system boundary.

## What this public repository is

This repository is SpendLeak's **public product and engineering surface**. It exists so customers, collaborators and technical reviewers can understand the product, its evidence model and the engineering principles behind it without exposing the proprietary production implementation.

The production source repository, infrastructure configuration, provider integrations, database implementation, internal workflows and operational runbooks remain private by design.

That boundary is intentional: **publicly understandable, privately defensible.**

## Public engineering docs

- [`docs/architecture.md`](docs/architecture.md) — system boundaries and product flow
- [`docs/engineering-principles.md`](docs/engineering-principles.md) — reliability and evidence principles
- [`STATUS.md`](STATUS.md) — current public product/engineering boundary
- [`SECURITY.md`](SECURITY.md) — security reporting guidance
- [`CHANGELOG.md`](CHANGELOG.md) — high-level public milestones

## Source availability

This is **not an open-source distribution of the SpendLeak production application**. Publication of these documents does not make the private implementation, infrastructure or operating materials public.

Security reports should not include secrets or personal data in public issues. See [`SECURITY.md`](SECURITY.md).
