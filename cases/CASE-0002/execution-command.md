# CASE-0002 Execution Command

## External mutation command template
```bash
gh api \
  --method PUT \
  -H "Accept: application/vnd.github+json" \
  /repos/prettybusysolutions-eng/xzenia-attestation/collaborators/<github-username> \
  -f permission=push
```

## Notes
- GitHub collaborator permission `push` corresponds to the practical `write` role.
- This is the minimum recommended starting role for `CASE-0002`.
- Do not elevate to admin unless explicitly justified and approved.

## Immediate verification commands
```bash
gh api /repos/prettybusysolutions-eng/xzenia-attestation/collaborators/<github-username>/permission

gh repo view prettybusysolutions-eng/xzenia-attestation --json nameWithOwner,url
```

## Follow-on actions after successful add
1. create a test PR under branch protection
2. have the second governed principal perform a real review
3. capture review URL and resulting merge/close state
4. update CASE-0002 evidence in both repos
```
