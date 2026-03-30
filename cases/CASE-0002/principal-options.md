# CASE-0002 Principal Options

## Goal
Select the second governed principal form that can actually strengthen repository governance without introducing fake separation.

## Option A — Human personal maintainer account

### Shape
A second real human GitHub account is added as a collaborator/reviewer with meaningful review authority.

### Strengths
- strongest near-term proof of real separation-of-duties
- review is performed by a distinct principal with human judgment
- simplest model for CODEOWNERS + required review to become materially real

### Weaknesses
- depends on a real second human identity existing and participating
- operationally heavier than a bot/app
- may create ambiguity if the second account is still effectively controlled by the same operator

### Honest boundary
Counts as stronger governance only if the second account is genuinely distinct in control and actually performs review actions.

## Option B — Org-owned bot/App identity

### Shape
A revocable GitHub App or org-owned machine identity participates in bounded review/verification workflows.

### Strengths
- auditable
- revocable
- least-privileged by design
- aligns with prior preference for org-owned/revocable identities over assistant-owned personas

### Weaknesses
- weaker than a true second human for separation-of-duties if the same operator controls both sides
- more setup complexity
- may help with verification, but not with meaningful human approval unless paired with another human principal

### Honest boundary
Useful for automation and auditability. Not enough by itself to prove human separation-of-duties.

## Option C — Second governed reviewer identity under the same operator

### Shape
A second account exists and can technically satisfy required review.

### Strengths
- fastest path to make branch protection practically satisfiable
- can unblock stronger GitHub settings quickly

### Weaknesses
- high risk of self-approval theater
- weak proof value if control is not meaningfully separated

### Honest boundary
This may improve operational discipline but should not be overstated as strong governance proof.

## Recommended order
1. **Target state:** Option A + Option B
   - second real human reviewer for approval separation
   - org-owned/App identity for bounded automation and verification
2. **Near-term acceptable bridge:** Option B plus explicit documentation that approval separation is still incomplete
3. **Avoid claiming:** Option C as mature governance proof

## Minimum permission model
Second principal should have only the minimum permissions required to:
- review pull requests
- participate in CODEOWNERS enforcement where appropriate
- not silently bypass governance as admin unless explicitly intended and documented

## Decision rule
Choose the strongest model that is both:
- actually operable now
- honest about who controls which identity
