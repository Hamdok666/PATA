# Copilot instructions — PATA

Purpose
- Give fast, actionable guidance for AI coding agents working in this repository.

Repository snapshot
- Current repo contains only the high-level project brief: [README.md](README.md).
- PATA is currently a design/vision project ("Phase 0") with no source code or build system present.

First actions for any AI agent
- Read [README.md](README.md) thoroughly (mission, roadmap, payment targets: Stripe + M-Pesa).
- Confirm intent before scaffolding: ask whether to create a frontend, backend, or minimal prototype.
- If asked to scaffold, propose a single, small scaffold (example: `src/` + minimal `README.md` updates) and show the files you will create before writing them.

Where to look next (typical places in this repo)
- Root: README.md, LICENSE.
- If present later: `package.json`, `pyproject.toml`, `go.mod`, `Cargo.toml`, `Dockerfile` — prefer reading these to detect language/tooling.
- Typical source locations: `src/`, `backend/`, `frontend/`, `cmd/`, `pkg/`.

Project-specific constraints & examples
- This project is led by African contributors (see README sections on participation and roadmap). Prioritize design and feature decisions that align with that mission and explicitly note when you need cultural or domain clarification.
- Roadmap references in README: update the "Where We Are Right Now" and "Next Steps" sections if you change scope or add an MVP plan.

Practical rules for edits
- Small, incremental edits only unless the user explicitly asks for a large scaffold.
- When adding code, include a short `How to run` in the repo README and add basic test commands (`tests/` or language-idiomatic test files).
- When implementing payments or external integrations, reference the roadmap: add a `docs/payments.md` that explains chosen providers (Stripe, M-Pesa) and the integration approach.

Commit & PR guidance
- Commit message style: `feat:`, `fix:`, `chore:` followed by a clear one-line summary and 1–2 sentence body when necessary.
- Pull request description should include: what changed, why, and manual test steps.

What the agent must not do without permission
- Don't create production infrastructure (cloud accounts, live payments) or commit secrets.
- Don't assume a language or framework; ask first if the repo has no manifest files.

If you need clarification
- Ask these minimal questions: desired language/framework, target MVP scope (booking page, operator dashboard, payments), and whether to add CI or deploy scripts.

Contact points
- Point maintainers to README.md for mission context and to this file for engineering rules.

End
-- Keep this file short; update when the repo gains source code or CI.
