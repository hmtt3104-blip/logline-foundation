# Logline Foundation

Public standards, templates, and operating model for the Logline engineering journal.

Logline Foundation defines how engineering experiments are documented, reviewed, sanitized, and published across Logline repositories.

## Purpose

This repository does not publish product code.

It publishes the methodology behind the code.

Logline Foundation exists so every public Logline repository can be read as part of the same engineering journal: what problem was tested, what was built, what failed, what was learned, and what should be asked next.

## Core method

Problem → Hypothesis → Experiment → Data → Conclusion → Next question

## Start here

Use these documents first:

1. [Logline Constitution](LOG_LINE_CONSTITUTION.md) — baseline principles for public Logline work.
2. [README Template](README_TEMPLATE.md) — standard public repository landing page structure.
3. [Public Repository Cleanup Checklist](PUBLIC_REPO_CLEANUP_CHECKLIST.md) — safety review before publication.
4. [Quality Gate](QUALITY_GATE.md) — promotion criteria for public-ready, pinned, flagship, and release-ready repositories.
5. [Status Taxonomy](STATUS_TAXONOMY.md) — shared language for repository, experiment, decision, RFC, cleanup, and trust states.

Then use the record templates when documenting work:

- [Experiment Record Template](EXPERIMENT_RECORD_TEMPLATE.md)
- [Decision Record Standard](DECISION_RECORD_STANDARD.md)

## Repository contents

Current foundation documents:

| Document | Role |
| --- | --- |
| [LOG_LINE_CONSTITUTION.md](LOG_LINE_CONSTITUTION.md) | Principles and scope for public Logline repositories. |
| [README_TEMPLATE.md](README_TEMPLATE.md) | Standard README structure for public exports. |
| [PUBLIC_REPO_CLEANUP_CHECKLIST.md](PUBLIC_REPO_CLEANUP_CHECKLIST.md) | Safety checklist before a repository becomes public. |
| [QUALITY_GATE.md](QUALITY_GATE.md) | Minimum checks for public-ready, pinned, flagship, and release-ready states. |
| [STATUS_TAXONOMY.md](STATUS_TAXONOMY.md) | Controlled status language used across repositories. |
| [EXPERIMENT_RECORD_TEMPLATE.md](EXPERIMENT_RECORD_TEMPLATE.md) | Template for documenting one engineering experiment. |
| [DECISION_RECORD_STANDARD.md](DECISION_RECORD_STANDARD.md) | Standard format for architectural and process decisions. |

Planned documents are candidates, not mandatory backlog items. Create them only when repeated use in real Logline repositories proves that a separate standard is needed.

Current candidates:

- SECURITY_TEMPLATE.md
- CONTRIBUTING_TEMPLATE.md
- ROADMAP_TEMPLATE.md
- REPOSITORY_RELATIONSHIPS.md
- RFC_STANDARD.md
- ENGINEERING_GLOSSARY.md
- NAMING_STANDARD.md

## Used by

Current public Logline repositories:

| Repository | Verified baseline | Public readiness |
| --- | --- | --- |
| logline-greenhouse-ai | Local-only Flask/mock-sensor smoke test passed. | NEEDS_CLEANUP |
| logline-greenhouse-edge | Dry-run config load and tests passed. | NEEDS_CLEANUP |
| logline-greenhouse-firmware | Arduino compile passed for ESP32S3 Dev Module. | NEEDS_CLEANUP |

These verified baselines prove basic reproducibility only. They do not prove production readiness, hardware safety, live greenhouse operation, authentication, LAN exposure safety, or release readiness.

Planned Logline repositories:

- logline-calcocr

## Working principle

Code is one artifact.

The main artifact is the documented engineering process.

Every public Logline repository should explain:

- what problem was tested;
- what hypothesis was used;
- what was built;
- what data or observations were collected;
- what failed;
- what decision followed;
- what question comes next.

## Change rule

Foundation standards may evolve, but meaningful changes should be traceable.

Use decision records when a change affects repository structure, safety policy, public readiness, status language, or the way Logline repositories are reviewed.

Small wording fixes may be committed directly when they do not change the meaning of a standard.

## Status

Repository status: Working.

Foundation standards are allowed to evolve, but changes should be documented through decision records when they change the method, not just the wording.

## License

MIT License. See [LICENSE](LICENSE).
