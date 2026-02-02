# Contributing to IPOS Group Project

This document defines how team members should work in this repository.
These rules exist to protect subsystem boundaries and ensure clean integration.

---

## Branch Rules

- `main`
  - Stable, integrated, demo-ready branch
  - No direct pushes allowed
  - All changes must be merged via Pull Request (PR)

- Subsystem development branches
  - `team37/sa-dev` – IPOS-SA (Team 37)
  - `team38/ca-dev` – IPOS-CA (Team 38)
  - `team39/pu-dev` – IPOS-PU (Team 39)

All development should happen on your team’s branch.

---

## Folder Ownership

Each subsystem has a dedicated folder:

- `Team_37_IPOS-SA/` – owned by Team 37
- `Team_38_IPOS-CA/` – owned by Team 38
- `Team_39_IPOS-PU/` – owned by Team 39

Ownership is enforced using **CODEOWNERS**.

Do not modify another team’s folder unless explicitly agreed and reviewed.

---

## Shared Folder Rules (`shared/`)

The `shared/` folder is for:
- Interface definitions
- Shared schemas
- Integration documentation

Rules:
- Do not place subsystem-specific implementation code here
- Any change to `shared/` must be communicated to all teams
- Pull Requests touching `shared/` require cross-team review

---

## Pull Request Rules

All changes must be submitted via Pull Request.

Each PR should:
- Clearly describe **what changed**
- Explain **why the change was made**
- Mention if it affects other subsystems
- Be as small and focused as possible

Self-approval is not permitted.

---

## Commit Message Guidelines

Use clear, descriptive commit messages.

Good examples:
- `Add merchant account suspension logic`
- `Fix invoice total calculation`
- `Document shared catalogue schema`

Avoid vague messages such as:
- `update`
- `fix`
- `changes`

---

## Early Solo Development Note

During early stages, some teams may have only one member.

In this situation:
- CODEOWNERS may temporarily block self-approval
- This is expected behaviour
- Any temporary relaxation of review rules should be deliberate and re-enabled once additional members join

---

## Final Note

These rules are part of the project governance model.
They should not be changed without agreement from all teams and the project maintainer.
