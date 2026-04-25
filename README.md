<!--
  Starter README for a new Supermodel Labs tool.

  Replace every {{PLACEHOLDER}} as you go. Delete sections that don't apply
  yet and add them back when they do — the goal is a tight, useful README
  from day one, not a fully-populated skeleton.

  Conventions used across Supermodel Labs READMEs:
    - One short tagline under the title.
    - Table of contents only once the README is long enough to need one.
    - Install instructions lead with Homebrew, then a release binary, then source.
    - Reference material (command tables, flag tables) lives later in the doc.
    - Always end with an "Issues vs. Discussions" section + a license line.

  When you're ready to publish, delete this comment block.
-->

# {{TOOL_NAME}}

> {{ONE_LINE_TAGLINE}}

{{TOOL_NAME}} is {{SHORT_DESCRIPTION_ONE_OR_TWO_SENTENCES}}.

## Table of contents

- [Install](#install)
- [Quick start](#quick-start)
- [Key commands](#key-commands)
- [Philosophy](#philosophy)
- [Issues vs. Discussions](#issues-vs-discussions)
- [License](#license)

## Install

{{TOOL_NAME}} ships as a single static binary per platform.

```bash
# Homebrew (macOS / Linux)
brew install supermodellabs/tap/{{TOOL_NAME}}

# Download a release binary
# https://github.com/supermodellabs/{{TOOL_NAME}}/releases

# From source
git clone https://github.com/supermodellabs/{{TOOL_NAME}}
cd {{TOOL_NAME}}
{{BUILD_COMMAND}}
```

Verify the install:

```bash
{{TOOL_BINARY}} --version
{{TOOL_BINARY}} --help
```

## Quick start

```bash
# 1. {{STEP_ONE_DESCRIPTION}}
{{TOOL_BINARY}} {{STEP_ONE_COMMAND}}

# 2. {{STEP_TWO_DESCRIPTION}}
{{TOOL_BINARY}} {{STEP_TWO_COMMAND}}

# 3. {{STEP_THREE_DESCRIPTION}}
{{TOOL_BINARY}} {{STEP_THREE_COMMAND}}
```

## Key commands

```text
{{TOOL_BINARY}} {{COMMAND_GROUP_ONE}}   [subcommands...]
{{TOOL_BINARY}} {{COMMAND_GROUP_TWO}}   [subcommands...]
{{TOOL_BINARY}} {{TOP_LEVEL_COMMAND}}   ← {{ONE_LINE_DESCRIPTION}}
```

A few highlights:

| Command | What it does |
| --- | --- |
| `{{TOOL_BINARY}} {{EXAMPLE_COMMAND_ONE}}` | {{ONE_LINE_DESCRIPTION}} |
| `{{TOOL_BINARY}} {{EXAMPLE_COMMAND_TWO}}` | {{ONE_LINE_DESCRIPTION}} |
| `{{TOOL_BINARY}} {{EXAMPLE_COMMAND_THREE}}` | {{ONE_LINE_DESCRIPTION}} |

Run `{{TOOL_BINARY}} <command> --help` for full flags and examples.

## Philosophy

{{TWO_OR_THREE_PARAGRAPHS_ON_THE_OPINIONATED_DESIGN_CHOICES}}

A few principles that shape the tool:

- **{{PRINCIPLE_ONE}}.** {{ONE_OR_TWO_SENTENCES}}
- **{{PRINCIPLE_TWO}}.** {{ONE_OR_TWO_SENTENCES}}
- **{{PRINCIPLE_THREE}}.** {{ONE_OR_TWO_SENTENCES}}

## Issues vs. Discussions

We use **Discussions** for ideas, questions, and "what if {{TOOL_NAME}} did X?" — the conversational stuff that benefits from threading and isn't yet a concrete change. Start there if you're not sure.

We use **Issues** for concrete, reproducible change requests: a bug with a repro, a missing flag with a clear shape, a doc inaccuracy. An issue should describe the change well enough that a contributor could pick it up cold.

We close — warmly — issues and PRs that don't engage with the [contribution guidelines](./CONTRIBUTING.md). This isn't gatekeeping; it's care for the OSS ecosystem. A maintained project needs a steady signal-to-noise ratio, and we'd rather have a smaller queue we can actually serve than a large one we can't. If your issue or PR gets auto-closed, the bot will point you at the relevant section of CONTRIBUTING.md — please reopen after addressing the feedback.

## License

Apache 2.0. See [LICENSE](./LICENSE).
