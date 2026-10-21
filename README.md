# SOC Analyst Journey — Hands-on Code & Labs

[![GitHub](https://img.shields.io/badge/GitHub-orioninsist-181717?logo=github)](https://github.com/orioninsist)
[![Blog](https://img.shields.io/badge/Technical%20Blog-orioninsist.org-blue)](https://orioninsist.org/)

This is my **hands-on cybersecurity engineering workspace** while building practical skills for Junior SOC Analyst (L1) roles. It holds **working scripts, reproducible exercises, configuration examples, test fixtures, and verified lab evidence** — **not a daily diary or a collection of study notes**.

> **Learning notes and long-form explanations:** [orioninsist.org](https://orioninsist.org/)  
> **Blog Markdown sources:** [orioninsist/orioninsist.github.io](https://github.com/orioninsist/orioninsist.github.io)  
> **GitHub profile and selected work:** [github.com/orioninsist](https://github.com/orioninsist)

## What belongs here

- Small, functional **Python/Bash scripts** and reproducible experiments.
- Authorized **Linux, networking, log-analysis and SOC labs** with runnable code, sanitized sample inputs, and expected outputs.
- Tests, configuration examples, and automation prototypes that do not yet require a dedicated repository.
- Brief task-level READMEs explaining **how to run and verify code**, rather than general theory.

## Repository layout

Directories will be created **when the first real, tested artifact exists**:

```text
soc-analyst-journey/
├── labs/             # Self-contained, authorized, reproducible labs
├── scripts/          # Small reusable Python/Bash utilities
├── experiments/      # Focused prototypes and exercises
└── tests/            # Shared tests and synthetic fixtures as needed
```

Each lab should ideally include its source code, required setup, a safe sample dataset, a run command, and a reproducible verification result. No unverified achievements or fabricated screenshots.

## SOC L1 practical build queue

These are **planned exercises, not completed projects**. A lab is added to this repository only after its commands, sample inputs, and expected outputs have been tested.

| Order | Lab | Practical skill | Minimum reproducible evidence |
| --- | --- | --- | --- |
| 1 | Windows failed-logon triage | Event ID 4625, account/IP/time correlation | Synthetic event dataset, parsing script, assertions |
| 2 | DNS investigation | DNS queries, suspicious patterns, context | Sanitized DNS log, filter script, expected matches |
| 3 | Web access log triage | HTTP status codes, bursts, user agents | Synthetic access log, detection query, test cases |
| 4 | Sigma detection validation | Rule conditions, false positives | Sigma rule, synthetic positive/negative events |
| 5 | SIEM query practice | SPL/KQL filtering and aggregation | Queries, sample schema, expected results |
| 6 | SOC incident reporting | Evidence, scope, severity, escalation | Sanitized case report based on a verified lab |

### Definition of done for every lab

- [ ] Scope, assumptions, and authorized test environment are documented.
- [ ] Sample inputs are synthetic or properly sanitized.
- [ ] Exact setup and run commands are included.
- [ ] Expected output is provided and reproducible.
- [ ] Positive and negative test cases are included where applicable.
- [ ] Detection limitations and possible false positives are explained.
- [ ] No secrets, private logs, or unverified investigation claims are published.

### Recommended investigation workflow

`Alert → validate telemetry → establish timeline → enrich indicators → assess impact → document findings → escalate when warranted`

For SOC L1 work, prioritize evidence-backed triage and clear escalation over premature attribution. An IOC reputation hit or a single event ID alone does not establish malicious activity.

## When to create a separate repository

**Not every script needs its own repository.** Keep small exercises here. Extract a project into its own public repository only when it becomes a meaningful standalone tool or portfolio piece, with clear scope, independent usage instructions, tests, and maintainable code.

Selected standalone projects can then be linked from this README and my [GitHub profile](https://github.com/orioninsist).

## Writing and publishing

- **Technical articles and learning notes:** Hugo Markdown in [orioninsist.github.io](https://github.com/orioninsist/orioninsist.github.io), published on [orioninsist.org](https://orioninsist.org/).
- **Practical code and lab artifacts:** this repository.
- **Standalone, substantial tools:** separate repositories when justified.
- **Progress, decisions and workflow metrics:** the private master operations Google Sheet, not this public repository.

## Responsible security practice

Only use owned systems and authorized training environments. Never commit credentials, tokens, SSH keys, sensitive network details, confidential logs, or personal data. Use synthetic or properly sanitized examples.

---

**Principle:** Build it → test it → document how to run it → publish the technical explanation on [orioninsist.org](https://orioninsist.org/).
