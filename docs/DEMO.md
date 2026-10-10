# RepoMind Demo Commands

Use a disposable clone of a public repository or another repository that is safe to show. Let RepoMind report real repository-specific output; do not invent benchmark numbers.

```bash
repomind init
repomind status
repomind context "trace the authentication flow" --explain
repomind stats
repomind test-impact --base main --format markdown
repomind memory list --limit 3
```

Test-impact returns recommended commands as data and does not execute repository tests.

For maintained product instructions, see the canonical [demo guide](https://github.com/raazlehra/Repomind/blob/main/docs/DEMO.md) and [sanitized sample test-impact report](https://github.com/raazlehra/Repomind/blob/main/docs/SAMPLE_TEST_IMPACT_REPORT.md).

Do not show private source, private repository URLs, secrets, credentials, customer information, local user paths, or sensitive architecture details in public demos.
