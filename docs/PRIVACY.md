# RepoMind Privacy & Local-First Model

This page describes RepoMind's local-first privacy model. It is an engineering summary, not a legal privacy policy.

## Local Index

RepoMind builds a local SQLite intelligence index for a repository. The index can include repository paths, symbols, relationships, architecture facts, metrics, and repository memory with evidence/provenance.

RepoMind locally reads and indexes repository files. Bounded snippets can be read locally when requested by a command.

## Source Uploads

RepoMind does not upload repository source during normal operation.

The source tree remains authoritative. RepoMind output is discovery guidance for developers and coding agents.

## Telemetry and AI APIs

RepoMind does not send telemetry.

No external AI API is required for normal indexing or retrieval.

## Reports and Feedback

Validation reports and local results remain local until a user voluntarily shares them. Before sharing any report, issue, screenshot, terminal output, or support detail, remove sensitive information.

Do not post proprietary source code, credentials, API keys, tokens, private keys, environment files, local machine paths, customer data, internal hostnames, or sensitive business details in public issues.

## Public Issues

The public issue forms are for access requests, setup requests, audit requests, and sanitized feedback. They should not contain source uploads, private repository URLs, secrets, or sensitive repository details.
