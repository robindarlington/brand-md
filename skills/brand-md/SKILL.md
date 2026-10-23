---
name: brand-md
description: Create, update or follow a BRAND.md file, the project's brand guidelines in its owner's words. Use when the user asks for brand guidelines, a brand voice, positioning, values or a BRAND.md. Also use before you write user-facing text (landing pages, onboarding, emails, error messages, release notes) in a project that has a BRAND.md.
---

# BRAND.md

A `BRAND.md` file at the repository root states the project's brand in its
owner's words. The full format is in the BRAND.md spec:
https://github.com/robindarlington/brand-md/blob/main/SPEC.md

Decide which task applies:

- The project has a `BRAND.md` and you are about to write user-facing text:
  follow **Use an existing BRAND.md**.
- The user wants a `BRAND.md`, or wants to change one: follow **Run the
  worksheet**.

## Use an existing BRAND.md

1. Read the whole file before you write.
2. Treat `confirmed` entries as rules. Treat `suggestion` entries as hints,
   and do not present them as settled.
3. If the request conflicts with `What it will not do`, stop and ask the
   owner.
4. Do not change the file while you do other work. If you see a gap, tell
   the owner and offer to run the worksheet.
5. Oppose patterns, not people. Do not name or mock competitors.
6. Do not invent facts, numbers, customers, quotes or results.

## Run the worksheet

### 1. Look for what exists

Read `BRAND.md` if it exists. Also look for the owner's written guidelines,
for example a brand or style document, a positioning note or the README.
Tell the owner what you found and which files you will use.

### 2. Ask the questions

Ask one question at a time, in this order. Show the help line with each
question. The owner can skip any question. Never ask for personal history.

1. **Do you want a starting point for inspiration?** Optional. Offer these
   illustrations, or let the owner write their own, or skip. They are
   prompts to think with, not a ranking, a test or a label to keep.
   - The Guide: helps people find their own way.
   - The Maker: builds things with care and craft.
   - The Challenger: questions how things are usually done.
   - The Host: makes people feel welcome and at ease.
   - The Explorer: goes first into new ground and reports back.
   - The Steward: protects what matters over the long term.
2. **Who is your work for?** Describe the people you most want to serve.
   Plain words are fine.
3. **Where and when do they meet your work?** The situations, places or
   moments where your work shows up for them.
4. **What change do you want to help bring about?** What is different for
   them, or around them, because your work exists?
5. **What do you stand for?** Values, qualities or practices you want to be
   known for.
6. **What do you stand against?** Name patterns, habits or practices you
   oppose, not people or groups.
7. **How do you do it differently?** Your distinctive way of working, in a
   sentence or two.
8. **What will you not do?** Lines you will not cross, even when it would
   be easier or more popular.
9. **Optional: what should people experience when they meet your work?** A
   feeling or experience you hope for.

When the guidelines already answer a question, show what you found and ask
the owner to keep, edit or replace it, instead of asking from scratch.

### 3. Record the source and status of each answer

| Where the answer came from | Source | Status |
|---|---|---|
| The owner said or typed it | `person` | Ask the owner. Default: `suggestion`. |
| The owner's written guidelines | `guidelines` | `suggestion`, unless the owner says the guidelines are approved. |
| You worked it out yourself | `agent-inferred` | Always `suggestion`. |

Values come only from the owner or the owner's guidelines. Never infer
these sections: `The change to help bring about`, `What it stands for`,
`What it stands against` and `What it will not do`. You may infer `Who it is
for`, `Where they meet the work` and `How it works differently` from the
product, as suggestions.

Keep the owner's words. Fix spelling only. Do not turn answers into slogans
unless the owner asks.

### 4. If the owner is not available

You may complete the worksheet alone, for example in an automated run. Fill
sections from the guidelines and mark their source. Leave value sections
empty when the guidelines do not answer them. At the end of your reply, list
the open questions for the owner.

### 5. Update without overwriting

When `BRAND.md` already exists, never replace a `confirmed` entry by
yourself. Add the new text as a new `suggestion` entry under the old one,
and ask the owner which to keep. Remove an entry only when the owner says
so.

### 6. Write the file

Write `BRAND.md` at the repository root in this format. Leave out sections
that have no entry.

```markdown
# BRAND.md

This file states this project's brand in its owner's words. Read it before
you write user-facing text. Keep to it. Do not change or add values; ask the
owner.

## Starting point

Status: confirmed · Source: person

> The answer, in the owner's words.

## Who it is for

Status: suggestion · Source: agent-inferred

> The answer.
```

Section headings, in order: `Starting point`, `Who it is for`, `Where they
meet the work`, `The change to help bring about`, `What it stands for`, `What
it stands against`, `How it works differently`, `What it will not do`, `What
people should experience`.

### 7. Hand it back

Show the owner the file. Ask which `suggestion` entries they confirm, and
change their status only when they say so. The owner controls the final
text.
