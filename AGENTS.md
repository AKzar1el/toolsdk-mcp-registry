# Registry Agent Instructions

When reviewing or merging registry pull requests, follow `docs/PR_REVIEW.md`.
Use `.agents/skills/check-mcp-json/SKILL.md` for the reusable review, repair, and squash-merge
workflow and its read-only helper scripts.

- Use the validator from the trusted `main` branch to inspect pull request JSON. Do not execute
  scripts from a contributor branch.
- Never install or run an MCP package submitted by a pull request.
- Never merge, enable auto-merge, close, comment on, or modify a pull request without the user
  authorizing that specific action.
- Before an approved merge, refresh the pull request state and validation result.
- Use squash merge. Never bypass checks with `--admin`.
- Review and merge pull requests serially against the latest `main` so key collision checks remain
  current.
