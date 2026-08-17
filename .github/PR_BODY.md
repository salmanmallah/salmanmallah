## Summary
Restored repository profile content by rolling `README.md` back to commit `d58de7531ccf92c018af8c36a4a9c0457bdd2c8d` to resolve regressions introduced after the original restore attempt.

## Diagnosis
- README content in the active PR path diverged from the requested known-good snapshot.
- A dedicated PR body file was needed to document the restore scope and verification.

## Files changed
- `README.md` — restored to the state from commit `d58de7531ccf92c018af8c36a4a9c0457bdd2c8d`.
- `.github/PR_BODY.md` — added/updated PR report for this draft update.

## Local verification
1. `git fetch origin`
2. `git checkout restore-readme-d58de7`
3. `git show 9fb618f5d64cda1b4a54ebab60c9ee3f18991b2b:README.md`
4. `git show HEAD:README.md`
5. Confirm both outputs match (the README restore commit equals current branch state).

Original PR: #1  
Reference commit: `d58de7531ccf92c018af8c36a4a9c0457bdd2c8d`
