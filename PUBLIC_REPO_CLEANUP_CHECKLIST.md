# Public Repository Cleanup Checklist

## Purpose

Define the safety checklist that every repository must pass before becoming a public Logline export.

## Public readiness status values

Use these values for the final publication decision:

BLOCKED

NEEDS_CLEANUP

READY

## Cleanup finding status values

Use these values for individual checklist findings:

BLOCKER

WARNING

OK

## Secrets

Check for:

- .env
- API keys
- Telegram tokens
- Firebase configs
- service account JSON
- private keys
- passwords
- Wi-Fi credentials

Finding status:

BLOCKER / WARNING / OK

## Network / deployment details

Check for:

- private IPs
- VPN/Tailscale details
- production hostnames
- live dashboard URLs
- Raspberry usernames
- local absolute paths
- deployment maps
- operational runbooks

Finding status:

BLOCKER / WARNING / OK

## Files and artifacts

Check for:

- logs
- backups
- runtime state files
- sqlite/database files
- APK/debug builds
- binary artifacts
- screenshots
- personal images
- EXIF metadata
- generated outputs

Finding status:

BLOCKER / WARNING / OK

## Git history

Check:

- old commits do not contain removed secrets
- old commits do not contain removed images
- old commits do not contain configs
- repo was created as clean export if history is unsafe

Finding status:

BLOCKER / WARNING / OK

## Documentation

Check:

- README exists
- Foundation link exists
- Current status is explicit
- Safety notes exist
- Repository map exists
- Related repositories are listed
- Next questions are listed
- Known failures are documented

Finding status:

BLOCKER / WARNING / OK

## Decision

Final public readiness status:

BLOCKED / NEEDS_CLEANUP / READY

Reason:

Reviewer:

Date:

## Rules

If secrets were public, rotate them.

If sensitive files were in history, clean export is preferred over risky history rewrite.

Do not publish working directories directly.

Public Logline repositories are curated exports.

If any finding is `BLOCKER`, final public readiness should be `BLOCKED` or `NEEDS_CLEANUP` until the blocker is removed or explicitly accepted with a documented reason.
