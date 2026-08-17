The issue requested rolling back profile content to a known-good commit (`d58de7531ccf92c018af8c36a4a9c0457bdd2c8d`). This PR restores `README.md` to that revision’s content where recent regressions had removed key links and social sections.

What I changed

- Restored README.md exactly to the content from commit `d58de7531ccf92c018af8c36a4a9c0457bdd2c8d`.

Files changed:
- README.md — restored profile links and social sections, re-added HackerRank banner image link, fixed NULL placeholders to actual links.

How to verify locally

1. git fetch origin
2. git checkout restore-readme-d58de7
3. cat README.md  # should match content from commit d58de7531ccf92c0

Notes

- I left the PR as draft and did not merge. If you'd like I can open this PR for review or merge it after your approval.
