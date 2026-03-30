# CASE-0002 Next Approval Request

## Immediate next external mutation
Add a second governed human GitHub principal to `prettybusysolutions-eng/xzenia-attestation` with the minimum role that still permits meaningful pull-request review participation.

## Why this is first
This is the highest-proof-value next move because it is the first mutation that can advance real approval separation rather than only automation.

## Required missing input
1. `github_username` — the exact GitHub account to add

## Recommended starting role
Use **`write`** as the starting collaborator role.

Rationale:
- strong candidate for the minimum practical role that still supports meaningful PR review participation
- avoids overshooting to admin by default
- reduces the risk of a paper-only review path that is not operationally sufficient

## Exact approval text
Approved: add collaborator `<github-username>` to `prettybusysolutions-eng/xzenia-attestation` with role `write` for CASE-0002 governance migration.

## Expected immediate post-approval actions
1. add collaborator
2. verify collaborator presence/role through GitHub state
3. create test PR under branch protection
4. capture second-principal review event
5. record exact refs and remaining boundary in both repos

## Honest boundary
Until the username and role are provided and approved, no further real governance migration can occur without inventing identity or mutating external state beyond authorization.
