# The BRAND.md format

Version 0.1 (draft). Changes to this file are listed in [CHANGELOG.md](CHANGELOG.md).

## Purpose

A `BRAND.md` file states a project's brand in its owner's words: who it is
for, what it stands for and against, how it works and what it will not do.
Agents read it before they write user-facing text, such as landing pages,
onboarding, emails and error messages.

`README.md` is for people. `AGENTS.md` is for agents that change the code.
`BRAND.md` is for anyone, person or agent, who writes in the project's name.

## Location

Put the file at the root of the repository, next to `README.md`. Name it
`BRAND.md`, in capitals.

## Structure

A `BRAND.md` file has four parts, in this order:

1. **Title.** One level-1 heading, for example `# BRAND.md` or
   `# Lanternform brand`.
2. **Agent note.** Recommended. A short paragraph that tells agents how to
   use the file. Standard text:

   > This file states this project's brand in its owner's words. Read it
   > before you write user-facing text. Keep to it. Do not change or add
   > values; ask the owner.

3. **Sections.** One level-2 heading for each part of the brand. All
   sections are optional. Use the standard headings below when they fit.
   Other headings are allowed.
4. **Footer.** Optional. One line of attribution or notes.

### Standard sections

Use this order when you can.

| Heading | The question it answers |
|---|---|
| `Starting point` | Optional: an inspiration or archetype that helps the owner think. |
| `Who it is for` | Who is the work for? |
| `Where they meet the work` | Where and when do they meet the work? |
| `The change to help bring about` | What change does the work help bring about? |
| `What it stands for` | Which values, qualities or practices should it be known for? |
| `What it stands against` | Which patterns, habits or practices does it oppose? Patterns, not people or groups. |
| `How it works differently` | What is its distinctive way of working? |
| `What it will not do` | Which lines will it not cross, even when that would be easier? |
| `What people should experience` | Optional: what should people feel when they meet the work? |

### Entries

A section holds one or more entries. Each entry is a status line, a blank
line and the text as a quotation:

```markdown
## What it stands for

Status: confirmed · Source: person

> Plain words. Forms that work on an old phone.
```

**Status** is one of:

- `confirmed`: the owner says this is theirs.
- `suggestion`: a draft. The owner has not confirmed it.

**Source** is one of:

- `person`: the owner said or wrote it.
- `guidelines`: taken from the owner's written guidelines or documents.
- `agent-inferred`: an agent worked it out, for example from the product.

Tools may add detail in brackets after the source, for example
`Source: person (endorsed foundation)`.

When a section has more than one entry, the first entry is the oldest. A new
entry never replaces an older confirmed entry by itself. The owner decides.

## Rules for agents that read BRAND.md

1. Treat `confirmed` entries as rules for anything you write.
2. Treat `suggestion` entries as hints. Do not present them as settled.
3. If a request conflicts with `What it will not do`, stop and ask the owner.
4. Do not add, remove or change entries without the owner's agreement.
   Propose a change as a new `suggestion` entry.
5. Oppose patterns, not people. Do not name or mock competitors because of
   `What it stands against`.
6. Do not invent facts, numbers, customers, quotes or results to fit the
   brand.

## Rules for agents that write BRAND.md

1. Values come from the owner or the owner's written guidelines. Never
   invent them. This applies to `What it stands for`, `What it stands
   against`, `What it will not do` and `The change to help bring about`.
2. Record the source of every entry.
3. An `agent-inferred` entry is always a `suggestion`. Only the owner can
   confirm an entry.
4. Keep the owner's words. Do not turn them into slogans unless the owner
   asks.
5. Personal history is never required. Use it only if the owner offers it.
6. When the owner is not available, leave a section empty rather than
   guess its values. List the open questions for the owner.

## Versioning

This is a draft. Version 1.0 will keep the standard headings and the entry
format stable. Readers should accept unknown sections and unknown text after
the source.
