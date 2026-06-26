# Status Taxonomy

## Purpose

Define the status language used across Logline repositories.

Statuses must be explicit because repository state, experiment state, decision state, RFC state, and cleanup state are different things.

Do not reuse one status list for everything.

## Repository status

Prototype

Working

Stable

Paused

Archived

Internal only

## Public readiness status

BLOCKED

NEEDS_CLEANUP

READY

## Experiment status

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

Draft

Accepted

Superseded

Deprecated

Rejected

## RFC status

Open

Accepted

Rejected

Deferred

Closed

## Cleanup status

BLOCKER

WARNING

OK

## Trust level

Low

Medium

High

## Rules

- Always state which type of status is being used.
- Do not call a prototype stable.
- Do not call a sanitized export production-ready.
- Do not call an experiment verified without evidence.
- If safety is uncertain, use BLOCKED or NEEDS_CLEANUP.
- If a status changes, update the relevant document or create a decision record.
