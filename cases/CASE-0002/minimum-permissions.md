# CASE-0002 Minimum Permissions

## Second governed human principal
Recommended starting role: the least role that still permits pull-request review participation and CODEOWNERS satisfaction.

### Must be able to
- view repository contents
- review pull requests
- participate in required-review flow

### Should not require by default
- unrestricted admin
- branch-protection editing
- collaborator management
- settings mutation

## Org-owned / App-owned automation identity
Recommended starting scope: read-focused permissions plus only the narrow write capabilities needed for bounded verification/comment/status actions.

### Must be able to
- read repo metadata
- read workflow runs and statuses
- act only within the explicitly defined bounded automation role

### Should not require by default
- repo admin
- collaborator management
- branch-protection editing
- unrestricted content writes

## Honesty rule
If a stronger permission level is used for operational convenience, document that fact explicitly instead of pretending least privilege was achieved.
