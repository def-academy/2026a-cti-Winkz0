# M01 Reading

Read these. Nothing here is summarised for you on purpose. Roughly 2.5 hours.

| Source | Why it is on the list |
|---|---|
| GitHub Docs: Reusing workflows | You are being graded by one. Understand `workflow_call`, inputs, and why `secrets: inherit` is dangerous |
| GitHub Docs: Security hardening for GitHub Actions | Read the sections on script injection and `pull_request_target`. Relevant again in DFIR M06 |
| Michael Nygard, "Documenting Architecture Decisions" (2011) | The original ADR post. Short. The format you are required to use |
| pre-commit.com: Introduction + Supported hooks | Hook ordering is not arbitrary |
| gitleaks README: configuration and allowlisting | You will get a false positive in M03 on an API base URL. Know how to allowlist it correctly rather than disabling the hook |
| mypy: Strict mode reference | Know what `strict` actually turns on before you claim it in your ADR |

## Ungraded but recommended

- Renovate configuration docs. If you pin your pre-commit revs (you should), something has to bump them.
