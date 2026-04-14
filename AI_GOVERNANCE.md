# AI Governance

This repository uses AI-assisted development tools including GitHub Copilot and Squad.

## Principles

1. **AI can draft; CI decides.** All code, whether human or AI-authored, must pass the same automated quality and security checks.
2. **Human accountability.** The maintainer reviews and owns every merge. AI output is a draft, not a decision.
3. **Verify, don't trust.** Non-obvious claims, configurations, and architecture decisions must be verified against authoritative sources.
4. **Transparency.** Pull requests should disclose meaningful AI assistance so reviewers know what to scrutinize.
5. **No secrets.** AI tools must never be given access to credentials, tokens, or sensitive data in prompts or code.

## What this means in practice

- Every PR must pass CI (lint, tests, security scans) before merge
- Branch protection prevents direct pushes to main
- Dependency scanning (Dependabot) catches known vulnerabilities
- Code scanning (CodeQL) identifies security issues
- PR templates include an AI disclosure checkbox
- Contributors are expected to review AI-generated output for correctness

## AI tools used in this project

- [GitHub Copilot](https://github.com/features/copilot) for code generation and review
- [Squad](https://github.com/bradygaster/squad) by Brady Gaster for agentic AI team orchestration

## Reporting concerns

If you believe AI-generated content in this repository is inaccurate, insecure, or violates attribution requirements, please open an issue or use the [security reporting process](SECURITY.md).
