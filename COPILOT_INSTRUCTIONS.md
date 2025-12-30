# COPILOT INSTRUCTIONS — PATA

Purpose
- Provide short, actionable guidance for AI coding agents working in this repository.

Repository snapshot
- Current state: Phase 0 — a design/vision repo. Only `README.md` and `LICENSE` exist.
- No source code, build system, or manifests (`package.json`, `pyproject.toml`, etc.) are present yet.

Quick start (first actions)
- Read `README.md` to understand mission, roadmap, and payment targets (Stripe + M-Pesa).
- Ask the maintainer which scaffold they want (frontend, backend, or minimal prototype) before creating files.
- If asked to scaffold, propose a single small scaffold (example: `src/` + minimal `README.md` updates) and list files to create before writing them.

Where to look next
- Root: `README.md`, `LICENSE`.
- When source appears, look for manifests: `package.json`, `pyproject.toml`, `go.mod`, `Cargo.toml`, `Dockerfile`.
- Typical source dirs to check: `src/`, `backend/`, `frontend/`, `cmd/`, `pkg/`.

Project-specific rules & patterns
- Contributions and feature decisions should explicitly respect the project mission: PATA is led by African contributors — call this out when proposing UX or policy changes.
- Roadmap items in `README.md` are authoritative for feature priorities (MVP → partner dashboard → payments → AI features).

Editing and scaffolding rules
- Keep edits minimal and incremental unless the user explicitly requests a larger scaffold.
- When adding runnable code, include a short "How to run" in the repo `README.md` and basic tests in a `tests/` folder or language-idiomatic test harness.
- For payment integrations, add `docs/payments.md` describing provider choices (Stripe, M-Pesa), required secrets (do not commit), and recommended dev/test flows.

Commits & PRs
- Use conventional commit-style messages: `feat:`, `fix:`, `chore:` followed by a concise summary.
- PR description must include: what changed, why, and manual test steps.

Security and operations
- Never create cloud resources, live payment credentials, or commit secrets without explicit maintainer approval.
- When credentials are needed for local testing, prefer environment variables and a `.env.example` file (do not commit real secrets).

When uncertain
- Ask these minimal clarifying questions: desired language/framework, target MVP scope (booking page, operator dashboard, payments), and whether to add CI/deploy scripts.

Examples (how to propose a scaffold)
- Minimal frontend scaffold proposal:
  - `src/web/` with a simple static HTML + CSS + single JS page
  - `README.md` run instructions and `tests/` smoke test
  - Suggested packages and a one-line `npm init` or `pip` plan
- Minimal backend scaffold proposal:
  - `src/api/` with a tiny HTTP server (Flask/Express) and an example `GET /health` route
  - `README.md` run instructions and a small test file

Contact and maintenance
- Refer maintainers to `README.md` for mission context and to this file for agent rules.
- Update this file when the repo acquires source code, manifests, CI, or deployment configuration.

Notes
- This file is intentionally short and actionable. Expand only with concrete, discoverable patterns from the repo (do not add aspirational guidelines).
