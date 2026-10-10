# How RepoMind Works

RepoMind follows a local, bounded evidence path:

```text
Repository
  -> eligible files and static analysis
  -> local SQLite intelligence index
  -> bounded context and change-impact evidence
  -> CLI or local MCP
  -> developer or coding agent
```

The source tree remains authoritative. RepoMind output supports discovery, change review, and test planning; it does not replace source inspection or human judgment.

Read the maintained technical explanation in the canonical product documentation: [How RepoMind Works](https://github.com/raazlehra/Repomind/blob/main/docs/HOW_IT_WORKS.md).
