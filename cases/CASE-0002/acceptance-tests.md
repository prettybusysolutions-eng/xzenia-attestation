# CASE-0002 Acceptance Tests

## Test 1 — Second principal exists
**Pass when:** a second governed human principal is visible in repository access state.

## Test 2 — Review path is real
**Pass when:** a real pull request receives a review from the second governed principal.

## Test 3 — No self-approval theater
**Pass when:** the approval event used to satisfy branch protection is not merely a second identity effectively standing in for the same undifferentiated actor without explicit boundary disclosure.

## Test 4 — Admin-bypass boundary is reduced or explicitly bounded
**Pass when:** either admin bypass is removed for normal flows, or the remaining emergency/bypass path is explicitly documented as a narrow exception rather than normal governance.

## Test 5 — Automation identity is honest
**Pass when:** any App/org-owned identity has explicit permissions, revocability, and a bounded function, and is not misrepresented as approval separation.

## Test 6 — Evidence is externally resolvable
**Pass when:** collaborator/review/app-installation effects are represented by GitHub-visible objects that can be checked again later.
