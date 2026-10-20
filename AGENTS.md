# Agent instructions

## Commit attribution

- Do not add AI authorship attribution to commits or pull requests. Omit
  `Co-authored-by` trailers for Claude, Codex, Copilot, Cursor or other AI
  tools, and omit footers such as "Generated with Claude Code". Keep human
  coauthors.

`scripts/check-ai-attribution.sh` enforces this in CI (the `AI attribution` workflow) and in a local `commit-msg` hook. Enable the hook once per clone with `git config core.hooksPath .githooks`. Cursor and Copilot add attribution through per-user settings, so turn it off there too.
