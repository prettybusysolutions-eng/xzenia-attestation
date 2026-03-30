# CASE-0002 Onboarding Checklist

## Objective
Make addition of the second governed principal and optional automation identity executable, auditable, and minimally privileged.

## Track A — Second governed human principal

### Preconditions
- candidate GitHub account exists
- account is controlled by a genuinely distinct human principal
- principal understands the repo’s truth boundary and review role

### Minimum required capability
- can access the repo
- can review pull requests
- can satisfy CODEOWNERS review where required
- does **not** require admin unless explicitly justified

### Setup sequence
1. add collaborator with the minimum role that still permits meaningful review participation
2. verify the account appears in repo/collaborator state
3. open a test PR that requires review
4. have the second principal perform a real review action
5. merge or close based on actual review outcome
6. record the observed behavior and exact GitHub refs in the case evidence

### Acceptance checks
- second principal is visible in GitHub repo access state
- review event is performed by that principal on a real PR
- review satisfies branch protection without self-approval theater
- documentation records the principal class and honest remaining boundary

## Track B — Org-owned / App-owned automation identity

### Preconditions
- identity is revocable and owned by the governed account or org
- permissions can be bounded narrowly
- automation purpose is explicit (verification, evidence collection, bounded checks)

### Minimum required capability
- read repository metadata and workflow state
- optionally comment or update status in tightly bounded ways
- should not be granted broad admin unless specifically required and justified

### Setup sequence
1. create or install the App / org-owned machine identity
2. grant minimum permissions needed for bounded automation
3. verify installation or identity presence in repo settings/state
4. run one bounded action and record the resulting GitHub object
5. document exact permissions and non-claims

### Acceptance checks
- identity is revocable
- permissions are explicitly documented
- at least one bounded action is visible through GitHub state
- documentation distinguishes automation from approval separation

## Non-claim rule
Completing Track B alone does not satisfy strong separation-of-duties proof.
