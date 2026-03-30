# CASE-0002 Approval Options Summary

## Current state
Preparation is complete for both external mutation tracks, but neither has executed yet.

## Option 1 — Add second governed human principal

### External action
Add one genuinely distinct human GitHub account as a collaborator to `prettybusysolutions-eng/xzenia-attestation` with the minimum role that still permits meaningful PR review participation.

### Proof value
**Higher** — this is the first move that can advance real approval separation.

### What it can prove if followed by a real review event
- a second governed principal exists
- review can occur under branch protection
- governance is less dependent on a single actor

### What it still does not prove alone
- mature separation-of-duties without an actual review event
- elimination of admin bypass unless enforcement is tightened afterward

## Option 2 — Add org-owned / App-owned automation identity

### External action
Create or install one revocable machine identity with minimum bounded permissions on `prettybusysolutions-eng/xzenia-attestation`.

### Proof value
**Medium** — improves auditability and bounded automation, but does not create human approval separation.

### What it can prove
- revocable machine identity exists
- bounded automation can operate visibly
- some verification can be externalized from the human operator

### What it does not prove
- human approval separation
- multi-principal governance by itself

## Recommended order
1. **First:** add second governed human principal
2. **Second:** add org-owned / App-owned automation identity
3. **Then:** test PR/review path and re-evaluate `enforce_admins=true`

## Decision rule
If only one external mutation is approved first, choose the option that increases proof value the most.
That is the second governed human principal.

## Exact next approval-ready request
Approved: add collaborator `<github-username>` to `prettybusysolutions-eng/xzenia-attestation` with role `<role>` for CASE-0002 governance migration.
