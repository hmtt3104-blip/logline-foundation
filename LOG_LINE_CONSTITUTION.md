# Logline Constitution

## Purpose

Define the engineering principles that guide every Logline experiment and public repository.

This document is the baseline for how Logline thinks, documents, publishes, and changes its own standards.

The constitution defines principles. The templates and gates define operating details.

## Principles

### 1. Reality over assumptions

Every experiment starts from a real problem, observed behavior, or testable question.

Assumptions are allowed, but they must be marked as assumptions.

Observations, assumptions, interpretations, and conclusions must not be mixed together.

### 2. Evidence over preference

A claim is stronger when it is connected to observations, experiment records, incidents, constraints, or reproducible behavior.

Preference can guide exploration, but it must not be presented as evidence.

If evidence is weak, missing, or indirect, that uncertainty must be stated.

### 3. Process over presentation

The public artifact is not only the final result.

The public artifact is the documented path from problem to hypothesis, experiment, data, conclusion, and next question.

### 4. Failures are evidence when they teach something

A failed experiment is worth publishing only when it adds useful information:

- a wrong assumption was exposed;
- a boundary was found;
- a method was invalidated;
- a next question became clearer.

Failure without context is noise. Failure with context is data.

### 5. Public repositories must be sanitized

Public Logline repositories are curated engineering records, not live working directories.

They must not include:

- secrets;
- private runtime configuration;
- private network maps;
- production logs;
- personal images;
- old unsafe history;
- deployment notes that expose live systems.

### 6. Reproducibility is preferred over completeness

A small experiment that can be understood and repeated is more valuable than a large undocumented system.

Completeness is useful only after the experiment is reproducible enough to inspect.

If full reproduction depends on private infrastructure, the public repository should state the smallest safe reproduction path and name what cannot be reproduced publicly.

### 7. Security before convenience

Convenient publication is not allowed to override safety.

When in doubt, keep live configuration, credentials, logs, and private operational details out of public repositories.

If public safety is uncertain, public readiness should remain BLOCKED or NEEDS_CLEANUP until the uncertainty is resolved or documented.

### 8. Decisions must be traceable

Important engineering decisions should be documented.

A future reader should be able to see:

- what was decided;
- why it was decided;
- what evidence supported it;
- which assumptions remained;
- which alternatives were rejected;
- what trade-offs were accepted;
- what would trigger a review.

### 9. Standards evolve through documented decisions

Templates and standards are not fixed forever.

They may change when practice shows a better method, but meaningful changes should be recorded through decision records.

Small wording fixes may be committed directly when they do not change the meaning of a standard.

### 10. Foundation standards apply across repositories

Every public Logline repository should follow the shared standards unless there is a documented reason not to.

The goal is not uniformity for its own sake.

The goal is that every repository can be read as part of the same engineering journal.

### 11. Code is one artifact

Code matters, but it is not the only output.

Other first-class artifacts include:

- experiment records;
- data notes;
- architecture notes;
- decision records;
- failures;
- safety boundaries;
- known limitations;
- next questions.

## Scope

This constitution applies to public Logline repositories and public-facing exports.

Private working repositories may be messier, but anything published under Logline should be cleaned, documented, and reviewed against these principles.

## Related standards

Use this constitution together with:

- `README_TEMPLATE.md` for public repository landing pages;
- `EXPERIMENT_RECORD_TEMPLATE.md` for experiment evidence;
- `DECISION_RECORD_STANDARD.md` for traceable decisions;
- `PUBLIC_REPO_CLEANUP_CHECKLIST.md` for publication safety;
- `QUALITY_GATE.md` for promotion gates;
- `STATUS_TAXONOMY.md` for status language.

## Amendments

Changes to this constitution should be introduced through a documented decision record when they change the meaning of a principle.

Each amendment should explain:

- the problem with the current wording;
- the evidence or practice that exposed the problem;
- the proposed change;
- the expected consequence;
- the affected repositories or templates.

## Status

`Working document`
