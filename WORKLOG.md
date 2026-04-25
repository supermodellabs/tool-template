# {{TOOL_NAME}} WORKLOG

<!--
  Completed Phases land here in REVERSE-CHRONOLOGICAL order — newest at
  the top, oldest at the bottom. See AGENTS.md for the POT system overview.

  When a Phase finishes:
    1. Update its Objectives and Tasks to reflect what actually shipped
       (no stale descriptions).
    2. Mark the Phase ✅.
    3. Move it to the TOP of this file.
    4. Add an "Implementation notes" subsection with decisions, trade-offs,
       surprising findings, and ADR-style context worth preserving.
    5. Delete the Phase from TODO.md.

  The example Phase below shows the expected shape. Overwrite it as you
  complete real Phases.
-->

## Phase 0: ✅ Repo bootstrap (example entry — overwrite when you ship your first real Phase)

Stood up the repo from `tool-template`: README, AGENTS, TODO/WORKLOG scaffolding, issue and PR templates, and a first run of `provision-repo.ts` to align labels and Discussions with the org standard.

### Repo scaffolding from template

Cloned `supermodellabs/tool-template`, replaced placeholders, and committed the baseline.

- [x] Replace `{{TOOL_NAME}}` and other placeholders across README, AGENTS, TODO, WORKLOG
- [x] Confirm `.github/ISSUE_TEMPLATE/` and `PULL_REQUEST_TEMPLATE.md` render correctly on GitHub
- [x] First green CI run on `main`

### Org standard provisioning

- [x] #user Run `provision-repo.ts {{TOOL_NAME}}` to reconcile labels and Discussion categories
- [x] #user Enable Discussions and verify Announcements / Ideas / Help / Share categories exist
- [x] #user Confirm inheritance of `CONTRIBUTING.md` and `SECURITY.md` from `supermodellabs/.github`

### Implementation notes

{{ANY_DECISIONS_TRADEOFFS_OR_SURPRISES_WORTH_REMEMBERING_LATER}}

For example: which name we picked and why, any deviations from the standard org baseline, the shape of the first Phase 1 we're now starting in `TODO.md`.
