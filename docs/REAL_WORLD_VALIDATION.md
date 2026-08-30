# RepoMind Real-World Validation

RepoMind validation is intended to collect reproducible, sanitized evidence from repositories testers own or are authorized to use.

## Public-Safe Metrics

A validation result may describe:

- anonymous repository ID;
- language/framework;
- expected files defined by the tester;
- expected-file recall;
- approximate context tokens;
- approximate repository tokens;
- represented-context reduction;
- retrieval latency;
- memory facts included.

Token measurements are provider-neutral estimates.

They are not:

- provider tokenizer counts;
- billing tokens;
- account credits;
- guaranteed savings.

## Example Result Shape

```text
repository_id: beta-repo-001
language_framework: Python/FastAPI and TypeScript/React
approximate_repository_size: 500-2,000 files
expected_files_defined_by_tester: yes
expected_file_recall: reported by the validation run
approximate_context_tokens: reported by the validation run
approximate_repository_tokens: reported by the validation run
represented_context_reduction: reported by the validation run
retrieval_latency: reported by the validation run
memory_facts_included: reported by the validation run
```

Do not expose local repository paths, private branch names, proprietary file names, source snippets, credentials, internal hostnames, or customer data in public example results.

## Review Before Sharing

Before posting a validation result:

1. Open the report locally.
2. Confirm it contains no proprietary source code.
3. Confirm it contains no secrets, credentials, private keys, tokens, internal hostnames, or customer data.
4. Redact local user directories and proprietary path segments.
5. Share only the sanitized result unless a smaller private reproduction is arranged separately.

## Interpreting Results

Expected-file recall compares manually expected important files with files returned in task context. Approximate token numbers are local observability estimates. Retrieval latency is local runtime for the measured request. Memory facts included describe how many relevant Repository Memory records were present in the context.

These metrics are useful for comparison and debugging, but they should not be presented as billing results, universal performance claims, or replacement for human review.
