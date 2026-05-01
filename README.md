# Xzenia Attestation

Cryptographic and systemic verification protocols for zero-trust environments.

Xzenia Attestation is part of the operator kit for binding claims, actions, verification, and outcomes to durable evidence under governed conditions.

## Role in the system
Trust is not assumed.
It is established through visible, verifiable state transitions.

## Standard
Bind the claim.
Verify the action.
Preserve the evidence.

## What this repo is
- A public attestation surface
- A governed audit trail
- A testbed for real consequence loops on GitHub

## What this repo is not
- A product repo
- A marketing repo
- A vanity demo

## Proof standard
A claim counts only when it is tied to:
1. a stable external identifier
2. an authenticated principal or review action
3. an externally visible state transition
4. a verification path that resolves
5. an outcome record with evidence reference

## Core objects
- `cases/` — one folder per attested case
- `ledger/` — append-only event records
- `reports/` — generated summaries
- `schemas/` — JSON schemas for case/action/outcome/verification
- `.github/workflows/` — verification and attestation workflows
- `.github/CODEOWNERS` — ownership baseline for governed review
- `.github/pull_request_template.md` — claim/verification discipline for PRs
- `GOVERNANCE-BASELINE.md` — separates enforced controls from policy-only intent

## First objective
Close `CASE-0001` through the full governed loop:
- case created
- recommendation recorded
- approval recorded
- execution visible
- verification passes
- outcome recorded

## Doctrine
Build from truth, not performance.
