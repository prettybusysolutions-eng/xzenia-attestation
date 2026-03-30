# CASE-0002 Execution Plan

## Phase 1 — Principal model
- identify the second governed principal form
  - human personal maintainer account
  - org-owned bot/App identity
  - or another revocable governed reviewer identity
- define minimum permissions required

## Phase 2 — GitHub enforcement migration
- add the second principal/collaborator
- verify CODEOWNERS/review settings remain satisfiable
- decide whether `enforce_admins=true` is now safe
- test PR path under the stronger model

## Phase 3 — Evidence
- record the real collaborator or reviewer identity
- record the first PR/review event under multi-principal governance
- update outcome and System 6 reports with observed behavior, not aspiration

## Non-goal
Do not pretend separation-of-duties exists before a second governed principal actually participates.
