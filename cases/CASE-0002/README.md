# CASE-0002 — Multi-Principal Governance Migration

## Objective
Remove single-principal/admin-bypass fragility from the attestation surface and move toward real separation-of-duties.

## Why this case exists
`CASE-0001` proved a minimal real GitHub-native attestation loop.
Subsequent hardening proved branch protection is real, but also surfaced the remaining weakness:
- current repo is effectively single-principal
- `enforce_admins=false`
- direct admin bypass remains in the trust model

This case exists to migrate from governance that is partially enforced to governance that has materially stronger separation.

## Success criteria
1. At least one second governed principal exists with meaningful review authority
2. Default-branch changes require PR path in practice, not just policy text
3. Admin bypass is either removed or explicitly reduced to a tightly bounded emergency path
4. Review requirements are satisfiable without collapsing into self-approval theater
5. Repo documentation and System 6 record the exact enforced state and exact remaining boundary

## Honest boundary
This case is not complete when paperwork says it is complete. It is complete only when GitHub state, repo membership, and observed behavior all confirm the stronger governance model.
