# BRAND.md

**Brand guidelines your coding agent can follow.**

`README.md` is for people. `AGENTS.md` is for agents that change the code.
`BRAND.md` states what a project stands for and against, who it is for and
how it works, in its owner's words. Agents read it before they write landing
pages, onboarding, emails and error messages.

Without it, an agent writes the same copy as every other landing page. With
it, the agent has the owner's words to keep to.

## What a BRAND.md looks like

```markdown
# BRAND.md

This file states this project's brand in its owner's words. Read it before
you write user-facing text. Keep to it. Do not change or add values; ask the
owner.

## What it stands for

Status: confirmed · Source: person

> Plain words. Forms that work on an old phone. Data that belongs to the
> charity.

## What it will not do

Status: confirmed · Source: person

> We will not sell or share sign-up data. We will not add tracking to forms.
```

Every entry says whether the owner confirmed it, and where it came from: the
owner (`person`), the owner's written guidelines (`guidelines`) or an agent
(`agent-inferred`). Agents may draft suggestions. Only the owner confirms.

- Full format: [SPEC.md](SPEC.md)
- Blank template: [templates/BRAND.md](templates/BRAND.md)
- Invented example: [examples/lanternform/BRAND.md](examples/lanternform/BRAND.md)

## Make one

**Option 1: let your agent interview you.** Install the skill below, then
ask your agent: "Make a BRAND.md for this project." It asks nine short
questions, one at a time, and writes the file. It never invents your values.

**Option 2: by hand.** Copy [templates/BRAND.md](templates/BRAND.md) to the
root of your repository and replace the help text with your own answers.

## Install the skill

**Claude Code**

```text
/plugin marketplace add robindarlington/brand-md
/plugin install brand-md@brand-md
```

**Other agents.** Copy [`skills/brand-md/SKILL.md`](skills/brand-md/SKILL.md)
into your agent's skills folder, or paste it into the agent's instructions.
The skill is plain Markdown. It needs no API key, account or network access.

## Use it

Once your repository has a `BRAND.md`, the skill tells your agent to read it
before it writes user-facing text. You can also add one line to your
`AGENTS.md`:

```markdown
Before you write user-facing text, read BRAND.md and keep to it.
```

## Rules the skill follows

- Values come from you or your written guidelines. The agent never invents
  them.
- Anything the agent works out by itself stays a suggestion until you
  confirm it.
- A new answer never silently replaces one you confirmed.
- Personal history is never required.
- Oppose patterns, not people.

## Status

Version 0.1 is a draft. Feedback and pull requests are welcome, especially
from people who use `BRAND.md` with their agents. See
[CHANGELOG.md](CHANGELOG.md).

`BRAND.md` comes from Brand Compass, a guided branding worksheet. The format
is open: any tool may read or write it.

## Licence

MIT. See [LICENSE](LICENSE).
