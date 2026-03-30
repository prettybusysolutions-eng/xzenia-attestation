# CASE-0002 Migration Decision

## Current decision
The clean target model is:
- **approval separation:** a second real governed human principal
- **automation/verification:** an org-owned or app-owned revocable machine identity

## Why
This gives the best balance of:
- real approval separation
- revocable automation
- least privilege
- auditability

## Near-term bridge if target state is not immediately available
If a second real human principal cannot be added yet, the repo may still use an org-owned/App identity to improve auditability and bounded automation, but the documentation must continue to state that strong separation-of-duties has not yet been achieved.

## Explicit non-claim
A second identity that is effectively controlled by the same operator should not be described as mature governance proof.
