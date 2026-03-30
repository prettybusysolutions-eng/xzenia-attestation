# CASE-0002 Ready-to-Execute Runbook

## Current status
All design and packaging work is complete.

## Sole remaining missing input
- `github_username` of the second governed principal

## On approval
1. run the collaborator-add command with permission `push`
2. verify collaborator permission through GitHub API
3. record collaborator evidence
4. create test PR
5. capture second-principal review event
6. update CASE-0002 and System 6 records with exact refs

## Honest boundary
No further real progress can occur without the actual GitHub username. Any attempt to proceed beyond this point without that identity would require fabrication or unauthorized external mutation.
