# Status Taxonomy

## Purpose

Define the status language used across Logline repositories.

Statuses must be explicit because repository state, experiment state, decision state, RFC state, cleanup findings, public readiness, and trust level are different things.

Do not reuse one status list for everything.

## Repository status

Use this for the overall state of a repository.

Prototype

Working

Stable

Paused

Archived

Internal only

## Public readiness status

Use this to state whether a repository can be public.

BLOCKED

NEEDS_CLEANUP

READY

## Experiment status

Use this for one experiment record.

Idea

Planned

Running

Observed

Documented

Repeatable

Verified

Invalidated

Superseded

## Decision status

Use this for decision records.

Draft

Accepted

Superseded

Deprecated

Rejected

## RFC status

Use this for proposed standards or larger design changes.

Open

Accepted

Rejected

Deferred

Closed

## Cleanup finding status

Use this for individual cleanup checklist findings, not for the final public readiness decision.

BLOCKER

WARNING

OK

## Trust level

Use this for confidence in an experiment, result, or claim.

Low

Medium

High

## How these statuses relate

A repository can be `Working` and still have public readiness `NEEDS_CLEANUP`.

A cleanup finding can be `WARNING` while the final public readiness status is still `READY`, if the warning is documented and accepted.

An experiment can be `Documented` with trust level `Low` when observations exist but evidence is weak.

A decision can be `Accepted` and later become `Superseded`; do not silently rewrite the old decision.

## Rules

- Always state which type of status is being used.
- Do not call a prototype stable.
- Do not call a sanitized export production-ready.
- Do not call an experiment verified without evidence.
- If public safety is uncertain, use `BLOCKED` or `NEEDS_CLEANUP` for public readiness.
- If a cleanup item is unsafe, mark the finding as `BLOCKER`.
- If a status changes, update the relevant document or create a decision record.
