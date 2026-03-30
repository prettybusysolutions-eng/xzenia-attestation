# CASE-0002 Approval Boundary

## What can be done without further approval
- define plans, criteria, decision memos, and evidence expectations in local/public repo files
- inspect current GitHub state
- verify existing branch protection and workflow state

## What requires explicit human approval
- adding a collaborator to the repo
- creating or installing a GitHub App / machine identity
- changing collaborator roles or access levels
- changing branch protection in ways that materially alter who can merge or bypass
- any external mutation that changes real account access or governance state

## Why
These actions modify external state and identity/control boundaries. They are governance actions, not just documentation work.
