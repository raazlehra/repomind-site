# RepoMind Public Demo Guide

This public demo guide shows how to present RepoMind without exposing private paths, private repositories, credentials, or proprietary source code.

Use a clean, disposable clone of a public repository or another repository that is safe to show on screen. Let RepoMind print real output from the repository being demonstrated. Do not invent output numbers.

## Future Video Placeholder

Reserved future demo video path:

```text
assets/demo/repomind-demo.mp4
```

The video file is not included yet.

## Command Flow

Run commands from a repository root that is safe to show.

```bash
repomind init
repomind status
repomind context "fix PDF upload validation bug"
repomind context "fix PDF upload validation bug" --explain
repomind stats
repomind memory list --limit 3
```

## Automatic Freshness Demo

1. Save a source change in the demo repository.
2. Do not run `repomind refresh`.
3. Do not run a watch command.
4. Run a read command, such as:

```bash
repomind context "fix PDF upload validation bug" --explain
```

RepoMind checks freshness before answering, then returns context based on the current local repository state.

## Presenter Guardrails

- Do not invent output.
- Do not claim benchmark results, cost reductions, universal speedups, or guaranteed savings.
- Do not show proprietary source, secrets, customer names, internal remotes, environment files, private tickets, or private branches.
- Use generic paths in slides, docs, screenshots, and issue comments.
- Keep the story simple: index once, ask for task context, inspect why files were selected, check stats and memory, then save a source change and query again.
