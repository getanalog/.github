# Agent guide — Analog organization profile

Operating rules for any AI agent working in this repository, regardless of
vendor or harness. `CLAUDE.md` is a symlink to this file. `profile/README.md`
is the public organization profile GitHub renders.

## AI co-authorship disclosure

Every commit an AI agent produces or materially assists carries a
`Co-Authored-By` trailer naming the exact model active at commit time, in the
provider's format:

```
Co-Authored-By: Claude <model display name> <noreply@anthropic.com>
Co-Authored-By: Codex <model display name> <noreply@openai.com>
```

Resolve the model at commit time; never attribute work to a generic tool name.
Co-authorship stated only in a PR body, review comment, or session log does
not count — the merged commit is the record GitHub renders. This repository
squash-merges with the constituent commit messages as the body, so a trailer
on every commit reaches the merged commit; do not change that merge setting.
The rule holds for every Analog repository, public or private.

## Working rules

- Branches, commits, and PR titles follow Conventional Commits 1.0.0.
- Open pull requests; a human merges them.
- The profile is public copy: describe what Analog does for the reader,
  never internal systems, vendors, or unreleased surfaces.
