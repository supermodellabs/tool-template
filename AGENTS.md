# {{TOOL_NAME}} — Agent Context

Welcome. This file is the entry point for agents working on {{TOOL_NAME}}. Read it first; it points at everything else.

## What this project is

{{TOOL_NAME}} is a [Supermodel Labs](https://github.com/supermodellabs) tool — part of a small family of source-available and open source CLIs for **agentic analytics engineering**. The brand brief, in short:

- Single portable binary, distributed via Homebrew (`supermodellabs/tap`) and Linux package managers.
- Friendly, ergonomic CLI UX: pretty output, helpful errors that link to docs, agent-friendly verbose modes, and just enough delight (animated splash screens, ASCII art, tasteful color) to make the command line feel alive without tipping into gimmick.
- Tools compose where it makes sense — assume a user may have several Supermodel tools installed and lean on shared conventions.

Edit `README.md` for the user-facing pitch; this file is for collaborators and agents.

## Repo baseline

Every Supermodel Labs repo ships with the same baseline. Rely on it; don't reinvent it locally.

| Surface | Where | Notes |
| --- | --- | --- |
| Issue templates | `.github/ISSUE_TEMPLATE/` | Two forms: bug + suggestion. Everything else routes to Discussions via `config.yml`. |
| PR template | `.github/PULL_REQUEST_TEMPLATE.md` | Conventional Commits title, summary, related, testing, checklist. |
| Discussion categories | Provisioned by `provision-repo.ts` | Announcements 🤗, Ideas 🧐, Help 🤠, Share 😍. |
| Labels | Provisioned by `provision-repo.ts` | `type:`, `status:`, plus `good first issue`, `help wanted`, `duplicate`. |
| Workflows | `.github/workflows/` | Standard CI, release, and homebrew-tap publish flows. |
| Contributing guide | Inherited from `supermodellabs/.github` | Don't add a per-repo `CONTRIBUTING.md` unless this tool genuinely diverges. |
| Security policy | Inherited from `supermodellabs/.github` | Same — only override if this tool has a meaningfully different threat model. |

When in doubt, prefer to update the org-level defaults over forking them per repo.

## How we plan and track work

This project uses the **POT (Phases > Objectives > Tasks)** system. The full spec lives in the user's rules at `~/.agents/rules/collaborating-on-task-lists.md`; the summary below is enough to be productive.

| Level | Markdown | Role | Execution |
| --- | --- | --- | --- |
| **Phase** | `## Phase N: description` | Sequential project checkpoint | Serial — finish one before starting the next |
| **Objective** | `### description` | Declarative goal (well-scoped, like a PR) | Parallel within a Phase — safe to assign to subagents |
| **Task** | `- [ ] description` | Imperative step inside an Objective | Sequential within an Objective |

**Status markers on Phases:** 🌀 active, ✅ completed, no marker = unstarted. Only one Phase active at a time.

**Files:**

- `TODO.md` — active and upcoming work. The current Phase is at the top; Backlog at the bottom.
- `WORKLOG.md` — completed Phases in **reverse-chronological** order, with implementation notes, decisions, and ADR-style context where useful.

**The lifecycle:** when a Phase is done, (1) update its language to reflect what actually shipped, (2) mark it ✅, (3) move it to the *top* of `WORKLOG.md` with notes, (4) delete it from `TODO.md`.

**A few rules that matter:**

- `#user`-tagged items are for the human (deploys, manual installs, account changes). Don't attempt them — if one blocks you, **stop and alert the user**.
- Don't commit pure `TODO.md` or `WORKLOG.md` updates — fold them into the substantive commit. If a subagent leaves a `docs(todo): ...` commit, squash it.
- Backlog items are not active work. Don't start them without user approval to promote into a Phase.
- If wording is ambiguous, an approach feels risky, or a task looks low-value — pause, flag it, agree on the change, persist to `TODO.md`, *then* do the work.

See the existing entries in `TODO.md` and `WORKLOG.md` for shape — they're written as worked examples for a fresh project.
