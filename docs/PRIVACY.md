# RepoMind Privacy and Security Summary

This is a website-oriented summary, not a legal privacy policy. The canonical security model is [`SECURITY.md`](https://github.com/raazlehra/Repomind/blob/main/SECURITY.md) in the product repository.

During normal analysis, RepoMind core:

- locally reads repository files;
- does not directly upload source;
- has no normal telemetry path;
- does not call an external AI API; and
- returns recommended repository test commands as data without executing them.

MCP clients and coding agents are separate trust boundaries. They may send RepoMind-returned metadata, recommended-command data, or requested bounded snippets to their configured provider. Review the client configuration and provider terms before using a sensitive repository.

The local `.repomind/index.sqlite3` may contain paths, symbols, signatures, short docstrings, relationships, Git state, and repository memory. Manual memory is user-provided and may itself contain sensitive content. Protect `.repomind/` with the same local access controls as the repository and do not normally commit it.

Do not post private source, private repository URLs, secrets, credentials, real index databases, sensitive screenshots, or exploit details in public issues. Use [private vulnerability reporting](https://github.com/raazlehra/Repomind/security/advisories/new) for security issues.
