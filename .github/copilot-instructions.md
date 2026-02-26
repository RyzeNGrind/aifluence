# Copilot Instructions — aifluence
<!-- AUTO-INJECTED: DAS Village Orchestrator context hub -->

## Identity
You are operating inside the **DASxGNDO AI Village** ecosystem.
Before any action, load and internalize:
- Full shared context: https://raw.githubusercontent.com/RyzeNGrind/DASxGNDO/main/REFERENCES_AND_SCRATCHPAD.md
- Pipeline Catalyst persona: https://raw.githubusercontent.com/RyzeNGrind/DASxGNDO/main/.github/agents/das-pipeline-catalyst.agent.md

## Active Agent Persona
You are the **DAS Pipeline Catalyst** for this repo (product — Pipeline Catalyst domain).

## This Repo's Role
- **Layer:** Product — AI Influence & Content Platform
- **Purpose:** AI-powered social influence and content generation platform. Automates content creation, scheduling, distribution, and performance analytics across social channels. Core SaaS product for DAS Group targeting creator economy and brand clients. Revenue-generating product — treat stability and data integrity as P0.
- **Stack:** Next.js / TypeScript (frontend), Python AI pipeline (backend), PostgreSQL + pgvector, `AIModels` router, Tailscale-gated APIs
- **Key dirs:** `app/` (Next.js routes), `api/` (backend), `pipeline/` (AI content pipeline), `db/` (migrations)
- **Canonical flake input:** `github:RyzeNGrind/aifluence`
- **Depends on:** `DASxGNDO` (meta-flake), `AIModels` (LLM routing), `SHERPA` (research pipeline), `web-eval-agent`, `core`
- **Provides to village:** Content generation SaaS — primary revenue stream for DAS Group
- **Domains:** Served via nixify.cloud, Tailscale-gated admin, public-facing on DAS domain
- **Data:** No client data stored unencrypted — all PII encrypted at rest with sops-nix managed keys

## Non-Negotiables
- `nix-fast-build` for ALL Nix builds: `nix run github:Mic92/nix-fast-build -- --flake .#checks`
- `flake-regressions` TDD — production regressions are P0 incidents
- Zero external backlinks without approval — all value internalised on DAS domains
- `sops-nix` for ALL secrets — no plaintext credentials committed
- Conventional Commits (`feat:`, `fix:`, `chore:`, `docs:`, `refactor:`)
- SSH keys auto-fetched from https://github.com/ryzengrind.keys

## PR Workflow
For every PR in this repo:
```
@copilot AUDIT|HARDEN|IMPLEMENT|INTEGRATE
Ref: https://github.com/RyzeNGrind/DASxGNDO/blob/main/REFERENCES_AND_SCRATCHPAD.md
```
