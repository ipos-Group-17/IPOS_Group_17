# IPOS Group Project Repository

This repository contains the implementation of the InfoPharma Ordering System (IPOS), developed as a group project.
The system is divided into three subsystems, each owned and implemented by a dedicated team.

The repository is public to enable enforced governance features (CODEOWNERS and branch protection) on GitHub Free.

---

## Repository Structure

- `Team_37_IPOS-SA/` - IPOS-SA (Server/Admin subsystem)
- `Team_38_IPOS-CA/` - IPOS-CA (Merchant desktop subsystem)
- `Team_39_IPOS-PU/` - IPOS-PU (Public portal subsystem)
- `shared/` - shared schemas, interfaces, integration documentation
- `docs/` - governance and project documentation
- `.github/` - GitHub config (e.g., CODEOWNERS)


Each subsystem folder is owned by its respective team.
Ownership and review responsibility are enforced via CODEOWNERS.

---

## Branches and Their Purpose

### `main`
- Stable, demo-ready branch
- Represents the integrated system
- No direct pushes allowed
- All changes must be merged via Pull Request (PR)

### Subsystem development branches
- `team37/sa-dev` → Team-37 SA (IPOS-SA)
- `team38/ca-dev` → Team-38 CA (IPOS-CA)
- `team39/pu-dev` → Team-39 PU (IPOS-PU)

These are the primary working branches for each subsystem team.

---

## Project Governance

Repository governance, ownership boundaries, and review rules are documented in: [docs/governance.md](docs/governance.md)

---

## Rules for Working in This Repository

1. Do not push directly to `main`.
2. Work on your subsystem branch:
   - Team-37 SA → `team37/sa-dev`
   - Team-38 CA → `team38/ca-dev`
   - Team-39 PU → `team39/pu-dev`
3. Only modify files inside your subsystem folder:
   - Team-37 SA → `Team_37_IPOS-SA/`
   - Team-38 CA → `Team_38_IPOS-CA/`
   - Team-39 PU → `Team_39_IPOS-PU/`
4. Any PR that touches another team’s folder requires approval from that team (enforced via CODEOWNERS).
5. Any PR that touches `shared/` requires cross-team review.
6. Keep PRs small and focused; explain what changed and why.
7. Do not commit build output, IDE files, or credentials; these are excluded via `.gitignore`.

---

## Temporary Solo Development Note

During early development, some teams may have only one member.

In this case:
- CODEOWNERS enforcement may temporarily block self-approval
- This is expected behaviour
- Protections may be briefly relaxed only when necessary
- Protections must be re-enabled once additional team members join

Any temporary relaxation should be documented.

---

## Governance Summary

- `main` is protected
- CODEOWNERS enforces subsystem ownership
- No one can silently change another team’s code
- Public visibility is used to enable these controls on GitHub Free

---

## Questions or Changes

If a change affects:
- Another subsystem
- Shared interfaces
- Integration behaviour

Raise it early via:
- Pull Request discussion
- Issue
- Team discussion

Do not merge first and explain later.

---

This structure is intentional and should not be changed without agreement from all teams.
