# SpendLeak — Public Engineering Changelog

This changelog records **high-level product and engineering milestones** suitable for public review. It intentionally omits private repository history, internal identifiers, security-sensitive implementation and commercial pipeline details.

## 2026-08-18 — Public repository positioning pass

- rewrote the README around plain buyer language rather than category jargon
- made the primary use cases and audit deliverable explicit
- clarified the observation → review → frozen-report evidence model
- kept current commercial terms subordinate to the live product as source of truth
- preserved the public/private boundary without exposing production implementation details

## 2026-08 — Paid Traffic Integrity Assurance launch baseline

### Product contract
- narrowed SpendLeak to a one-off Paid Traffic Integrity Assurance audit
- established a clear £199 one-off commercial offer on the live product
- defined a bounded scope of up to 50 paid destinations
- separated customer-supplied context from observed destination evidence
- established reviewed/frozen report delivery and an eligible follow-up comparison

### Production hardening
- added bounded destination/network handling and defensive target validation
- bounded critical external-provider and database work below surrounding execution limits
- hardened duplicate-effect prevention and ambiguous-provider reconciliation
- made deployment promotion reproducible and verification-gated
- verified the audit/review/report/follow-up state model against the hosted production schema using rollback-safe synthetic proof

### Buyer experience
- simplified homepage information architecture around trigger → deliverable → findings → proof → price
- made the report deliverable more explicit
- added direct differentiation from a manual URL-check workflow
- retained methodology as secondary proof rather than primary navigation
- completed live desktop/mobile post-deployment QA and repaired a responsive navigation consistency regression

## Public/private boundary

The production source repository remains private. This public surface exists to expose product intent, system architecture and engineering discipline without publishing the proprietary implementation or internal operational history.
