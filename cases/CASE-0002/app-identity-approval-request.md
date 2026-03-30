# CASE-0002 App Identity Approval Request

## Requested external action
Create or install one revocable org-owned/App-owned automation identity for `prettybusysolutions-eng/xzenia-attestation` with the minimum permissions required for bounded verification/automation tasks.

## Exact target
- Repository: `prettybusysolutions-eng/xzenia-attestation`
- Identity type: `<GitHub App | org-owned machine identity>`
- Identity name: `<app-or-identity-name>`
- Intended permission scope: `<minimum-bounded-scope>`

## Why this action is needed
`CASE-0002` targets stronger governance through a combination of:
- a second real human principal for approval separation
- a revocable machine identity for bounded automation and verification

This request covers the machine-identity half of that target state.

## Minimum acceptable result
- identity is revocable
- identity has explicitly bounded permissions
- identity can perform one narrow, GitHub-visible automation or verification action
- identity is not granted broad admin by default unless explicitly justified

## Evidence to capture immediately after approval/execution
1. installation or identity presence visible in GitHub settings/state
2. exact granted permissions/scope
3. first visible bounded action attributable to the identity
4. any resulting GitHub object URL (comment, check, status, workflow-linked output, etc.)

## Honest non-claim
Adding this identity does not substitute for human approval separation. It improves auditability and bounded automation only.

## Approval form
Approved: create or install `<identity-name>` as `<identity-type>` on `prettybusysolutions-eng/xzenia-attestation` with permissions `<scope>` for CASE-0002 automation/verification.
