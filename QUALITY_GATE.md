# Quality Gate

## Purpose

Define the minimum checks a Logline repository must pass before it can be treated as:

- Public-ready
- Pinned
- Flagship
- Release-ready

## Public-ready gate

Required checks:

- README exists
- Current status is explicit
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
- Next questions exist

## Pinned repository gate

Must pass Public-ready gate.

Additional checks:

- Project is understandable in 30 seconds
- At least one experiment record exists
- Architecture is documented
- Issues show next work
- README explains relation to Logline

## Flagship repository gate

Must pass Pinned repository gate.

Additional checks:

- Multiple experiment records exist
- Main safety boundaries are documented
- Known failures are documented
- Reproducibility path exists
- Related repositories are linked
- No misleading production-ready claims

## Release-ready gate

Must pass Public-ready gate.

Additional checks:

- Version is meaningful
- Changelog is updated
- Setup is reproducible
- Known limitations are listed
- Release does not include secrets, logs, or private configs
- Release notes explain what was tested

## Cleanup status

Allowed values:

BLOCKED

NEEDS_CLEANUP

READY

## Rules

Do not promote a repository by feeling.

Use gates.

If a gate fails, document why.

If safety is uncertain, status is BLOCKED or NEEDS_CLEANUP.
