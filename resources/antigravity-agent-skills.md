# Agent Skills in Google Antigravity

> Source: [Google Antigravity Docs — Agent Skills](https://antigravity.google/docs/skills?app=antigravity-ide)
>
> This is a Markdown adaptation of the official web documentation. The structure
> and wording have been simplified for teaching purposes; it is not an official
> Markdown export.

Agent Skills are reusable packages of instructions and resources that extend
what an Antigravity agent can do. Skills follow an open standard and are loaded
when their description matches the user's task.

## What is a skill?

A skill is a folder whose main file is named `SKILL.md`. It can provide:

- Instructions for completing a particular kind of task
- Domain-specific knowledge, conventions, and best practices
- Optional scripts, examples, templates, and other resources

At the beginning of a conversation, the agent receives the names and
descriptions of available skills. When a skill appears relevant, the agent reads
its complete instructions and uses them while performing the task.

## Where skills live

Antigravity supports workspace-specific and global skills.

| Scope | Location | Intended use |
| --- | --- | --- |
| Workspace | `<workspace-root>/.agents/skills/<skill-folder>/` | Project-specific workflows and conventions |
| Global | `~/.gemini/config/skills/<skill-folder>/` | Personal utilities shared across workspaces |

Antigravity now uses `.agents/skills` by default for workspace skills. The older
`.agent/skills` location remains supported for backward compatibility.

## Create a skill

Create a directory under one of the supported skill locations, then add a
`SKILL.md` file:

```text
.agents/skills/
└── my-skill/
    └── SKILL.md
```

A basic `SKILL.md` looks like this:

```markdown
---
name: my-skill
description: Helps with a specific task. Use when you need to do X or Y.
---

# My Skill

Detailed instructions for the agent go here.

## When to use this skill

- Use this when...
- This is helpful for...

## How to use it

Describe the workflow, conventions, and decisions the agent should follow.
```

## Frontmatter fields

| Field | Required | Description |
| --- | --- | --- |
| `name` | No | Unique identifier, normally lowercase with hyphens; defaults to the folder name |
| `description` | Yes | Explains what the skill does and when the agent should use it |

The description is the primary signal the agent uses to decide whether a skill
is relevant. Write it in the third person and include concrete task keywords.

## Add supporting resources

Only `SKILL.md` is required, but a skill may include additional files:

```text
.agents/skills/my-skill/
├── SKILL.md
├── scripts/
├── examples/
└── resources/
```

- `scripts/` contains executable helpers.
- `examples/` contains reference implementations.
- `resources/` contains templates and other supporting assets.

The agent reads supporting files only when they are needed.

## How Antigravity uses skills

Skills follow a progressive-disclosure workflow:

1. **Discovery:** The agent sees each skill's name and description.
2. **Activation:** When a skill matches the task, the agent reads its
   `SKILL.md`.
3. **Execution:** The agent follows the instructions and accesses supporting
   resources as needed.

The agent can select a relevant skill automatically. A user may also mention a
skill by name to request its use explicitly.

## Best practices

### Keep each skill focused

A skill should do one thing well. Prefer several focused skills over one large
skill that tries to cover unrelated workflows.

### Write a clear description

State both what the skill does and when it should be used. Include terms that
are likely to appear in relevant user requests.

### Treat scripts as tools

When a skill contains helper scripts, instruct the agent to inspect their
command-line help before reading the full implementation. This keeps context
focused on the task.

### Include decision guidance

For workflows with multiple valid approaches, add a decision tree or explicit
criteria that help the agent select the right path.

## Example: code review skill

```markdown
---
name: code-review
description: Reviews code changes for bugs, style issues, and best practices. Use when reviewing pull requests or checking code quality.
---

# Code Review

Review the changes using this checklist:

1. **Correctness:** Does the code behave as intended?
2. **Edge cases:** Are failures and unusual inputs handled?
3. **Style:** Does the code follow project conventions?
4. **Performance:** Are there obvious inefficiencies?

When reporting findings:

- Identify the exact code that needs attention.
- Explain why it is a problem.
- Suggest a practical alternative when possible.
```

This structure gives the agent enough metadata to discover the skill and enough
procedural guidance to apply it consistently.
