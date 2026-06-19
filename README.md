# Lifelong Catch & Correct

Offline-first SOC training platform concept for verifiable proof-of-work artifacts.

## Current repository status

This repository is not currently production-ready as a runnable application.

The prior README described a complete desktop application, installers, a `core/` application directory, Tauri build commands, proprietary curriculum folders, and downloadable binaries. Those assets are not currently present in this repository tree, so this repo must be treated as a planning/source-shell repository until the runnable application code is committed and verified.

## Intended product direction

Lifelong Catch & Correct is intended to become an offline-first cybersecurity training platform with:

- local-first SOC labs
- deterministic training flows
- evidence capture
- incident reports and portfolio exports
- mock interview practice
- audit logs
- no required cloud runtime for core learning flows

## Required readiness gates before release

A release cannot be called live-ready until all of the following are present and passing:

1. `core/package.json` or equivalent app manifest
2. reproducible install command
3. reproducible development command
4. reproducible production build command
5. desktop or PWA launch path
6. committed starter curriculum or seed data
7. exportable proof-of-work artifacts
8. lint/type/test workflow in GitHub Actions
9. security policy and dependency audit path
10. release artifact generation with checksums

## Build status

No verified build is currently available from this repository alone.

## Next implementation path

1. Commit the runnable `core/` application source.
2. Add package scripts for `dev`, `build`, `test`, `lint`, and `typecheck`.
3. Add a GitHub Actions workflow that blocks release on install, lint, typecheck, tests, and build.
4. Add a minimal starter lab and evidence export test.
5. Generate release artifacts only after the build is reproducible.

## Operating rule

Do not market this repository as a completed product until the runnable source, tests, and release artifacts are present and verified.
