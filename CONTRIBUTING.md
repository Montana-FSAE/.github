# Contributing to Montana FSAE repos

## Creating a repo

- Name it `<subsystem>-<project>` (see the org README for prefixes).
- Keep it **private**. Only leads make repos public.
- Add a `README.md` with: what it is, how to build/run it, and who owns it.
- Add a `.gitignore` (GitHub's templates for C, Python, etc. are fine).
- Give your subsystem's GitHub team access under Settings → Collaborators and teams.

## Branches & commits

- `main` should always build / be the last known-good version.
- Work on a branch: `yourname/short-description` or `feature/short-description`.
- Open a pull request to merge into `main`; get at least one teammate to review for anything going on the car.
- Commit messages: short imperative summary, e.g. `Add INA228 current limit config`.

## Hardware / CAD files

- Altium projects: commit the `.PrjPcb`, schematics, PCB, and libraries. Ignore `History/`, `Project Logs for */`, `__Previews/`, and `*.SchDocPreview` / `*.PcbDocPreview`.
- Tag every board you order: `git tag pdm-rev-b` and attach Gerbers/BOM to a GitHub Release.
- Large binaries (STEP, logs, videos) → use Git LFS or the team drive, not plain git.

## Data

- Don't commit raw logging data over ~50 MB. Store it on the team drive and link to it.

## Secrets

- Never commit passwords, API keys, or sponsor-confidential documents. If you do, tell a lead immediately — deleting the file doesn't remove it from history.

## Questions

Ask your subsystem lead or post in the team chat.
