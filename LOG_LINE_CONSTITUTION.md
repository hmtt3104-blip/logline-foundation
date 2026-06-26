# Logline Constitution

## Purpose

Define the engineering principles that guide every Logline experiment and public repository.

This document is the baseline for how Logline thinks, documents, publishes, and changes its own standards.

## Principles

### 1. Reality over assumptions

Every experiment starts from a real problem, observed behavior, or testable question.

Assumptions are allowed, but they must be marked as assumptions.

### 2. Process over presentation

The public artifact is not only the final result.

The public artifact is the documented path from problem to hypothesis, experiment, data, conclusion, and next question.

### 3. Failures are evidence when they teach something

A failed experiment is worth publishing only when it adds useful information:

- a wrong assumption was exposed;
- a boundary was found;
- a method was invalidated;
- a next question became clearer.

Failure without context is noise. Failure with context is data.

### 4. Public repositories must be sanitized

Public Logline repositories are curated engineering records, not live working directories.

They must not include:

- secrets;
- private runtime configuration;
- private network maps;
- production logs;
- personal images;
- old unsafe history;
- deployment notes that expose live systems.

### 5. Reproducibility is preferred over completeness

A small experiment that can be understood and repeated is more valuable than a large undocumented system.

Completeness is useful only after the experiment is reproducible enough to inspect.

### 6. Security before convenience

Convenient publication is not allowed to override safety.

When in doubt, keep live configuration, credentials, logs, and private operational details out of public repositories.

### 7. Decisions must be traceable

Important engineering decisions should be documented.

A future reader should be able to see:

- what was decided;
- why it was decided;
- which alternatives were rejected;
- what trade-offs were accepted.

### 8. Standards evolve through documented decisions

Templates and standards are not fixed forever.

They may change when practice shows a better method, but meaningful changes should be recorded through decision records.

### 9. Foundation standards apply across repositories

Every public Logline repository should follow the shared standards unless there is a documented reason not to.

The goal is not uniformity for its own sake.

The goal is that every repository can be read as part of the same engineering journal.

### 10. Code is one artifact

Code matters, but it is not the only output.

Other first-class artifacts include:

- experiment records;
- data notes;
- architecture notes;
- decision records;
- failures;
- safety boundaries;
- next questions.

## Scope

This constitution applies to public Logline repositories and public-facing exports.

Private working repositories may be messier, but anything published under Logline should be cleaned, documented, and reviewed against these principles.

## Amendments

Changes to this constitution should be introduced through a documented decision record.

Each amendment should explain:

- the problem with the current wording;
- the proposed change;
- the expected consequence;
- the affected repositories or templates.

## Status

`Working document`
