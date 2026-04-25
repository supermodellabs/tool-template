# {{TOOL_NAME}} TODO

<!--
  This file tracks active and upcoming work using the POT system
  (Phases > Objectives > Tasks). See AGENTS.md for the full overview
  and the user's `~/.agents/rules/collaborating-on-task-lists.md`
  for the spec.

  Conventions:
    - Phase status markers: 🌀 active, ✅ completed, no marker = unstarted.
    - Only ONE Phase may be active at a time.
    - Objectives within a Phase are parallel-safe; Tasks within an
      Objective are sequential.
    - When a Phase completes: update language, mark ✅, move to the TOP
      of WORKLOG.md with notes, then delete from this file.
    - Tag with `#user` any item only the human can do (deploys, account
      changes, manual installs). Agents must STOP and alert when blocked
      by one of these.

  The Phase below is a generic worked example. Overwrite it with your
  real first Phase when you're ready to start work.
-->

## Phase 1: 🌀 {{FIRST_PHASE_DESCRIPTION}}

{{ONE_OR_TWO_SENTENCES_ON_THE_PHASE_GOAL_AND_WHY_IT_COMES_FIRST}}

### {{FIRST_OBJECTIVE_DESCRIPTION}}

{{ONE_OR_TWO_SENTENCES_ON_WHAT_THIS_OBJECTIVE_DELIVERS_LIKE_A_PR_DESCRIPTION}}

- [ ] {{FIRST_TASK_IN_IMPERATIVE_MOOD}}
- [ ] {{SECOND_TASK}}
- [ ] {{THIRD_TASK}}

### {{SECOND_OBJECTIVE_DESCRIPTION}}

{{ONE_OR_TWO_SENTENCES}}

- [ ] {{FIRST_TASK}}
- [ ] {{SECOND_TASK}}
- [ ] #user {{TASK_ONLY_THE_HUMAN_CAN_DO_EG_PROVISION_THE_REPO_OR_PUBLISH_FIRST_RELEASE}}

## Phase 2: {{SECOND_PHASE_DESCRIPTION}}

{{ONE_OR_TWO_SENTENCES_ON_WHY_THIS_COMES_AFTER_PHASE_1}}

### {{OBJECTIVE_DESCRIPTION}}

- [ ] {{TASK}}
- [ ] {{TASK}}

## Backlog

<!--
  Items here are NOT active work. Agents should consider them when they
  inform active decisions but must NOT start them without user approval
  to promote into a Phase.
-->

- [ ] {{BACKLOG_IDEA_ONE_LINE_DESCRIPTION}}
- [ ] {{BACKLOG_IDEA_ONE_LINE_DESCRIPTION}}
