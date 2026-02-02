# IPOS Group Project Repository

This repository contains the implementation of the InfoPharma Ordering System (IPOS), developed as a group project.
The system is divided into three subsystems, each owned and implemented by a dedicated team.

The repository is public to enable enforced governance features (CODEOWNERS and branch protection) on GitHub Free.

---

## Repository Structure


├── Team_37_IPOS-SA/   (IPOS-SA: Server / Admin subsystem)

├── Team_38_IPOS-CA/   (IPOS-CA: Merchant desktop application)

├── Team_39_IPOS-PU/   (IPOS-PU: Public online portal)

├── Shared/            (Shared schemas, interfaces, documentation)

├── .github/           (CODEOWNERS and GitHub configuration)

└── README.md

Each subsystem folder is owned by its respective team.
Ownership and review responsibility are enforced via CODEOWNERS.

---

## Branches and Their Purpose

main
- Stable, demo-ready branch
- Represents the integrated system
- No direct pushes allowed
- All changes must be merged via Pull Request (PR)

Subsystem development branches
- team37/sa-dev → Team 37 (IPOS-SA)
- team38/ca-dev → Team 38 (IPOS-CA)
- team39/pu-dev → Team 39 (IPOS-PU)

These are the primary working branches for each team.

---

## Project Governance

Repository governance, ownership boundaries, and review rules are documented in: [Docs/governance.md](Docs/governance.md)

---

## Rules for Working in This Repository

### 1. Do not push directly to main
All changes must go through a Pull Request.
This ensures code review, auditability, and controlled integration.

### 2. Work only in your team’s folder
Each team must make changes only inside their own subsystem folder and avoid editing other teams’ folders unless explicitly agreed.

Examples:
- Team 37 works in Team_37_IPOS-SA/
- Team 38 works in Team_38_IPOS-CA/
- Team 39 works in Team_39_IPOS-PU/

### 3. Use your team’s development branch
Normal workflow:
- Make changes in your local copy
- Push to your team branch (e.g. team37/sa-dev)
- Open a Pull Request into main

### 4. CODEOWNERS enforcement (important)
This repository uses CODEOWNERS to enforce responsibility.

- Changes to a subsystem folder require approval from that subsystem’s team
- You cannot approve your own Pull Requests
- Cross-team changes require explicit review by the affected team

This applies even if you are an admin or organization owner.

### 5. Shared folder rules (Shared/)
The shared folder is for:
- Interface definitions
- Shared data schemas
- Integration notes
- Cross-subsystem documentation

Rules:
- Do not place subsystem-specific implementation code here
- Any change to shared should be communicated to all teams
- Pull Requests touching shared may require multiple approvals

### 6. Commit message expectations
Use clear, descriptive commit messages that explain what changed and why.

Avoid vague messages such as:
- update
- fix
- changes

### 7. Pull Request expectations
Every Pull Request should:
- Clearly state what changed
- Explain why the change was made
- Mention if it affects other subsystems

Small, focused Pull Requests are preferred over large ones.

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

- main is protected
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
