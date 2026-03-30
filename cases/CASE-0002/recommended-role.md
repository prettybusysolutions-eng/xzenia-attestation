# CASE-0002 Recommended Collaborator Role

## Recommendation
Use **`write`** as the starting collaborator role for the second governed human principal.

## Why `write`
It is the strongest candidate for the minimum practical role because the second principal must be able to:
- access the repository
- review pull requests in a meaningful way
- participate in the CODEOWNERS/required-review workflow without falling into a fake or non-satisfiable path

## Why not admin by default
Admin would overshoot least-privilege and preserve too much bypass power in the second identity before it is justified.

## Why not weaker by default
A weaker role risks creating a review path that exists on paper but is not operationally sufficient for the governance checks we actually need to test.

## Honest boundary
This is a recommended starting role, not a claim that GitHub governance is solved. Real proof still requires:
1. collaborator addition
2. real review event by the second governed principal
3. observed branch-protection behavior under the stronger model
