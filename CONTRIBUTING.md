# Contributing

This repository is split into three subsystem folders. Governance is enforced using a protected `main` branch and CODEOWNERS.

---

## Branches

### `main`
- Stable, integrated, demo-ready
- No direct pushes
- Pull Requests (PRs) only
- Approvals required
- Code Owner review required

### Subsystem development branches
- `team37/sa-dev` → Team-37 SA (IPOS-SA)
- `team38/ca-dev` → Team-38 CA (IPOS-CA)
- `team39/pu-dev` → Team-39 PU (IPOS-PU)

---

## Subsystem folders

- Team-37 SA works in: `Team_37_IPOS-SA/`
- Team-38 CA works in: `Team_38_IPOS-CA/`
- Team-39 PU works in: `Team_39_IPOS-PU/`

Do not modify another team’s subsystem folder unless explicitly agreed and reviewed.

---

## Shared folder (`shared/`)

Use `shared/` for:
- Interface definitions
- Shared schemas
- Integration documentation

Rules:
- Do not put subsystem implementation code in `shared/`
- Any change to `shared/` must be communicated to all teams
- PRs touching `shared/` require cross-team review (CODEOWNERS)

---

## Pull Requests

All changes into `main` must be via PR.

Each PR should:
- Describe what changed
- Explain why it changed
- Note any cross-subsystem impact

Self-approval is not permitted (GitHub enforces this).

---

## Commit messages

Use descriptive messages.

Good:
- `Add merchant account state checks`
- `Fix invoice total rounding`
- `Document shared catalogue schema`

Avoid:
- `update`
- `fix`
- `changes`

---

## Solo development note (early stage)

If a team has only one member initially, CODEOWNERS may block self-approval. This is expected.
Any temporary relaxation of review rules should be minimal and re-enabled once additional members join.
