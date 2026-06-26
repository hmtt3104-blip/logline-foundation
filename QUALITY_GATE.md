# Quality Gate

## Purpose

Define the minimum checks a Logline repository must pass before it can be treated as:

- Public-ready
- Pinned
- Flagship
- Release-ready

Quality gates are not labels for promotion.

They are evidence checks.

## Public-ready gate

Required checks:

- README exists
- Repository status is explicit
- Public readiness status is explicit
- Trust level is explicit when claims or results are presented
- Safety / security notes exist
- No secrets
- No private IPs
- No production configs
- No personal images
- No unsafe history
- No logs/backups/runtime outputs
- Public export status is clear
- Foundation link exists
- Repository map exists
- Known limitations exist
- Next questions exist

Minimum evidence:

- Cleanup checklist completed or clearly summarized
- README states what was sanitized or excluded
- Any non-reproducible part is named directly

## Pinned repository gate

Must pass Public-ready gate.

Additional checks:

- Project is understandable in 30 seconds
- At least one experiment record exists
- Architecture is documented
- Issues or README show next work
- README explains relation to Logline
- Known failures are documented if they affected the current design

Minimum evidence:

- One reader can understand the repository purpose, safety boundary, and next question from the README alone

## Flagship repository gate

Must pass Pinned repository gate.

Additional checks:

- Multiple experiment records exist
- Main safety boundaries are documented
- Known failures are documented
- Reproducibility path exists
- Related repositories are linked
- No misleading production-ready claims
- Important decisions are traceable through decision records or README notes

Minimum evidence:

- The repository shows an engineering path, not just a final code snapshot

## Release-ready gate

Must pass Public-ready gate.

Additional checks:

- Version is meaningful
- Changelog or release notes are updated
- Setup is reproducible
- Known limitations are listed
- Release does not include secrets, logs, or private configs
- Release notes explain what was tested
- Release notes explain what was not tested

Minimum evidence:

- A reader can reproduce the safe public version without private infrastructure

## Public readiness status

Allowed values:

BLOCKED

NEEDS_CLEANUP

READY

Use these values only for the final public readiness decision.

For individual cleanup findings, use the cleanup finding statuses from `STATUS_TAXONOMY.md`.

## Rules

Do not promote a repository by feeling.

Use gates.

If a gate fails, document why.

If safety is uncertain, public readiness status is BLOCKED or NEEDS_CLEANUP.

If evidence is missing, do not upgrade the gate.
