# How RepoMind Works

RepoMind is local-first repository intelligence for AI coding agents. It scans a developer repository on your machine, builds a local SQLite intelligence index, keeps that index fresh when saved files change, and returns task-focused ContextPack output through CLI or MCP.

## Simplified Architecture

```text
Developer Repository
  -> Scanner / Parsers
  -> Local SQLite Intelligence Index
  -> Automatic Freshness
  -> Intent + Explainable Retrieval
  -> ContextPack
  -> CLI / MCP
  -> Coding Agent
```

## What Happens Locally

- RepoMind locally reads and indexes repository files.
- The local index can include paths, symbols, imports, routes, dependency/caller relationships, architecture facts, and repository memory with evidence/provenance.
- Read commands can check freshness before answering, so saved source changes can be reflected without running a manual refresh command first.
- Bounded snippets can be read locally when requested.
- The source tree remains authoritative. RepoMind output guides discovery; it does not replace normal developer review.

## Privacy Boundary

RepoMind does not upload repository source during normal operation. No external AI API is required for normal indexing or retrieval, and RepoMind does not send telemetry.

If a tester voluntarily shares feedback, reports, screenshots, or issue details, they should remove proprietary source code, secrets, credentials, tokens, internal hostnames, local machine paths, and sensitive business details before posting.

## ContextPack

A ContextPack is task-focused repository context for a coding request. Depending on the repository and command, it can include likely files, symbols, relationships, tests, repository memory, metrics, and explanation signals that help a developer or coding agent inspect why something was selected.

## Explainable Retrieval

RepoMind retrieval is intended to be inspectable. Ranking can include signals such as path matches, symbol matches, graph relationships, route evidence, and repository memory. These signals are discovery aids, not a substitute for reading the relevant source.
