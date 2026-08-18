# SpendLeak — Public Status

## Product

**Live:** https://spendleak.co.uk

SpendLeak is live as a focused **PPC destination audit for performance agencies**. The live site is the authority for current price, ordering availability, scope and customer-facing terms.

Current public product scope:

- one brand/domain
- up to 50 paid destinations
- destination-path evidence captured and reviewed
- customer-supplied context kept separate from observed evidence
- prioritised actions in a client-forwardable frozen report
- one eligible follow-up comparison after remediation
- no Google Ads login or ad-account write access required for the core audit

Typical use cases are new-client takeovers, site migrations/relaunches, destination changes and unexplained performance incidents.

## Engineering

The production application is actively maintained in a private source repository. This public repository contains intentionally sanitised product and architecture material and does not mirror private source history.

Public engineering posture:

- production web application on managed infrastructure
- server-side checkout/payment flow
- PostgreSQL-backed state model
- bounded destination evidence collection
- explicit observation → review → frozen-report boundary
- private delivery and follow-up workflow
- CI/build and post-deployment verification gates

## Proof boundary

This repository does **not** use unsupported customer counts, revenue claims, case-study results or third-party endorsements as proof.

Screenshots and sample artifacts should be interpreted according to the labels shown on the live product. The public sample report is a demonstration, not customer proof.

## Source availability

Production source code, internal workflows, database implementation, provider configuration and security-sensitive operating details remain proprietary and private.
