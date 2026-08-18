# SpendLeak — Engineering Principles

SpendLeak is intentionally small in product scope, but the implementation is held to production-system standards. This page documents the **engineering behaviours**, not the proprietary code that implements them.

## 1. Fail closed around money and access

Checkout, report access and internal operator surfaces should become unavailable when required configuration or verification is missing rather than guessing a safe state.

## 2. Separate observation from judgement

Network/destination observations are evidence. Customer context is input. A reviewed finding is a conclusion. These are represented as different stages so one cannot silently become another.

## 3. Make state transitions explicit

Payment, audit, review, report and follow-up flows are modelled as explicit transitions rather than inferred from UI state or best-effort side effects.

## 4. Treat external providers as independent systems

A timeout after an external write is not proof of success or failure. Ambiguous outcomes are quarantined and reconciled before any retry is considered.

## 5. Design retries to be boring

Where retries are legitimate, operations use stable identifiers, immutable artifacts or idempotent state transitions so repetition does not create duplicate customer effects.

## 6. Bound network and database work

External HTTP work, destination collection and database statements are bounded below the surrounding request/worker lifetime. Slow or adversarial dependencies should terminate rather than consume capacity indefinitely.

## 7. Defend destination collection as untrusted input

Audit targets are user-controlled URLs. Collection therefore applies target validation, redirect re-evaluation, private/special-network protection and bounded response handling before evidence is accepted.

## 8. Freeze delivered evidence

A delivered audit is a historical artifact, not a mutable dashboard row. Follow-up checks compare against the frozen baseline instead of rewriting history.

## 9. Human review is a product boundary

Automation accelerates collection and classification, but the customer-facing report is reviewed before delivery. This is part of the product contract, not merely an internal QA preference.

## 10. Verification before promotion

A green source build is necessary but not sufficient evidence that production is healthy. Changes move through source verification, deployment verification and public/runtime readback before they are treated as live.

## 11. Preserve proof integrity

SpendLeak does not fabricate customer logos, result counts, testimonials or production evidence. Demonstrations are labelled as demonstrations and operational evidence remains separate from marketing claims.

## 12. Keep proprietary implementation private

This repository describes the architecture and engineering model at a useful level for customers, collaborators and technical reviewers. Production source, security-sensitive implementation, provider configuration, database schema and operating runbooks remain private.
