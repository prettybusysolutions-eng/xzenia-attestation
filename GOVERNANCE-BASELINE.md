# Governance Baseline

This document separates **what is already enforced** from **what is still policy-only**.

## Enforced now
- GitHub repository exists with stable public identifiers
- cases, ledger, and reports are committed in git history
- workflow validates the required repository structure
- changes can be surfaced through pull requests
- CODEOWNERS and PR template exist to make review intent explicit

## Not enforced yet
- protected default branch
- required approving review before merge
- required status checks for merge
- signed commit enforcement
- admin restrictions / bypass controls
- multi-principal review separation

## Current branch reality
The repository currently uses `master` as the default branch. Policy language should be interpreted against the **current default branch** until an explicit branch migration is executed.

## Planned hardening order
1. require PR path for material changes
2. require status checks on default branch
3. require review before merge
4. migrate from single-principal to multi-principal approval
5. prefer signed commits and stronger identity attestation

## Honesty rule
A governance claim counts only if GitHub settings or public repo state actually enforce it. Policy text alone is not proof.
