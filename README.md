# Xzenia Attestation

A reality-binding repository for Xzenia.

This repository exists to prove one thing: whether the system can bind recommendation, approval, execution, verification, and outcome to externally visible, stable identifiers under real governance.

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
