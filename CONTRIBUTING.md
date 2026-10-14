# Contributing to Montana FSAE repos

## Creating a repo

- Name it `<prefix>-<project>` (see the org README for prefixes).
- Keep it **private**. Only leads make repos public.
- Add a `README.md` with: what it is, how to build/run it, and who owns it.
- Add a `.gitignore` (GitHub's templates for C, Python, etc. are fine).
- Give your subsystem's GitHub team access under Settings → Collaborators and teams.

## Branches & commits

- `main` should always build / be the last known-good version.
- Work on a branch: `yourname/short-description` or `feature/short-description`.
- Open a pull request to merge into `main`; get at least one teammate to review for anything going on the car.
- Commit messages: short imperative summary, e.g. `Add CAN timeout handling`.

## Large files

**Do not store large files in git** — data logs, STEP files, CAD parts/assemblies, videos, etc. Keep them on the team drive and link to them.

Add them to your `.gitignore` so they can't be committed by accident:

```gitignore
# Data logs
*.log
*.mf4
*.ld
logs/

# CAD
*.step
*.stp
*.sldprt
*.sldasm
*.slddrw
*.iges
*.igs
*.stl
```

## Secrets

- Never commit passwords, API keys, or sponsor-confidential documents. If you do, tell a lead immediately — deleting the file doesn't remove it from history.

## Questions

Ask your subsystem lead or post in the team chat.
