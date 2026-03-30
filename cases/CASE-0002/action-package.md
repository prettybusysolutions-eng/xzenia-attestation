# CASE-0002 Action Package

## Purpose
Define the exact external-state actions required to advance from single-principal/admin-bypass governance toward stronger separation-of-duties.

## Action Set A — Add second governed human principal

### Required external action
Add one genuinely distinct human GitHub account as a collaborator to `prettybusysolutions-eng/xzenia-attestation` with the minimum role that still permits meaningful pull-request review participation.

### Minimum acceptable outcome
- second principal can access the repo
- second principal can review PRs
- second principal can satisfy CODEOWNERS review where relevant
- second principal does not require admin by default

### Evidence to capture after action
- collaborator presence visible in GitHub repo access state
- GitHub username / role of the second principal
- first real review event by that principal on a test PR

### Non-claim
Adding the collaborator alone does not prove separation-of-duties until a real review event occurs.

## Action Set B — Add org-owned / App-owned automation identity

### Required external action
Create or install a revocable org-owned/App-owned identity with minimum permissions for bounded automation and verification in `prettybusysolutions-eng/xzenia-attestation`.

### Minimum acceptable outcome
- identity is revocable
- permissions are explicitly bounded
- identity can perform one narrow visible automation action

### Evidence to capture after action
- installation or identity presence visible in GitHub settings/state
- explicit permission list
- one real GitHub-visible action attributable to the identity

### Non-claim
This does not substitute for human approval separation.

## Action Set C — Raise enforcement after second principal exists

### Required external action
Re-evaluate branch protection and admin policy after the second principal is active.

### Candidate tightening steps
- set `enforce_admins=true` if the workflow is now operationally safe
- require PR path in practice for normal changes
- run a test PR and review cycle to confirm protections are satisfiable without theater

### Evidence to capture after action
- branch-protection settings visible via GitHub API
- test PR URL
- review event URL
- merge or close event URL

## Approval boundary
These are external-state changes. They require human approval before execution.

## Ready-to-execute request form
When approval is sought, the request should specify:
1. exact identity to add or install
2. target permissions/role
3. exact repo target
4. expected evidence objects to capture after the change
