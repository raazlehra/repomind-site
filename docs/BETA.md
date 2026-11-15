# RepoMind Public Beta

RepoMind is an Apache-2.0 open-source public beta. The current release is [`v2.0.0b13`](https://github.com/raazlehra/Repomind/releases/tag/v2.0.0b13), a prerelease hardening beta.

RepoMind Free is available directly from the public GitHub Release. Download the release wheel and follow the canonical [installation guide](https://github.com/raazlehra/Repomind/blob/main/docs/INSTALLATION.md).

b13 improves Python test selection, TypeScript shared-harness recovery, and component-aware filename matching. Go dependency-graph extraction, runner integration, and native test selection remain unsupported; results report unknown coverage rather than fabricate Go test commands. See the release notes for qualification details and limitations.

Verify the downloaded `repomind-2.0.0b13-py3-none-any.whl` before installing. Its SHA-256 is `6152d1fa9761dd55662defe68a77d02cd50e7dd22bc4c013f62a1b7080601bd9`; the release also includes `SHA256SUMS.txt`.

Do not use plain `pip install repomind`; the package with that name on PyPI is a different project.

Use the [product repository](https://github.com/raazlehra/Repomind) for source, technical documentation, releases, and sanitized product feedback. Report security issues through [GitHub private vulnerability reporting](https://github.com/raazlehra/Repomind/security/advisories/new), not a public issue.
