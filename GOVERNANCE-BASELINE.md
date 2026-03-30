# Governance Baseline

This document separates **what is already enforced** from **what is still policy-only**.

## Enforced now
- GitHub repository exists with stable public identifiers
- cases, ledger, and reports are committed in git history
- workflow validates the required repository structure
- changes can be surfaced through pull requests
- CODEOWNERS and PR template exist to make review intent explicit
- default branch protection is enabled on `master`
- required status check: `Attestation Check`
- required pull request review count: `1`
- CODEOWNERS review is required by branch protection
- stale reviews are dismissed
- conversation resolution is required
- linear history is required
- force pushes are disabled
- branch deletions are disabled
- merged branches are auto-deleted

## Not enforced yet
- signed commit enforcement
- admin restrictions / bypass controls (`enforce_admins` is still false)
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

## Current honest boundary
The repository now has real branch protection, but it is still a single-principal setup and admins are not yet forced through the same review gate (`enforce_admins=false`). That means governance is materially stronger than before, but not yet strong separation-of-duties proof.
