---
name: design-grill
description: Draw a visual design out of someone who can react to designs but can't name what they want, through rounds of live links and mocks, ending in an approved DESIGN.md. Use when deciding how an app or site should look, or when the user says "design grill".
---

# Design grill

Most people can't say what they want a product to look like, but anyone can react to one in front of them. This skill runs that split: the user **reacts**, you **translate**. Naming what to borrow, why it works, and what it means as a rule is your job, never theirs. "I don't know why, I just like it" is a complete answer.

The output is a design spec (`DESIGN.md`) and a round log. The skill stops at an approved spec; writing tokens and components comes after.

Keep one question style throughout, the **grill**: work in rounds, ask everything whose prerequisites are settled (the **frontier**), number each question, give your recommended answer, then wait. A pick that depends on another open question waits for a later round. When a question has a few discrete options and the harness has a multiple-choice tool, use it; links and mocks the user has to open go in plain chat text, since some choice UIs hide the text above them.

Open question, untested: how numbered questions (1, 2...) combine with a round's own lettered options (A, B, C) when two frontier questions land in the same round — no dry run has hit this yet.

## 1. Ground

1. Create `docs/design/DESIGN.md` from [templates/DESIGN.md](templates/DESIGN.md). Read the project (README, docs, code, any existing design notes). Draft section 1: **subject** (what the product is made of), **primary job** (what a typical visit does), **audience** (who, on what device), **consequence** (what that means for the look). Then name the **hero moment**: the one screen that gets the most design effort and that every later page copies. Copy the starter list from [BANNED-DEFAULTS.md](BANNED-DEFAULTS.md) into section 4 (Banned defaults) — the rounds narrow it from here.
2. Confirm with the user, in the same numbered/recommend/wait grill format as reaction rounds, but only for the fields the project's own materials didn't already make clear: state what's already settled from the read, and ask only the gaps.
3. Create the log at `docs/design/grill-log.md` from [templates/grill-log.md](templates/grill-log.md).

Done when the user has confirmed section 1 and the hero moment, and the log exists.

## 2. Reaction rounds

Each round tests one **dimension** (overall feel, type, color, density...). [ROUNDS.md](ROUNDS.md) has the dimension order, how to pick links, when to switch from links to a mock, and how to read common reactions. Read it before round 1.

Each round:
1. Show 2 to 4 options, labeled A, B, C, that differ on that one dimension, each with a short label for what it stands for. Say what you'd pick and why in one line.
2. Wait for the reaction. Take it as given; don't argue taste.
3. Translate it into **Taken** bullets: concrete candidate choices, one specific thing per source, never "make it like site X." When the user overrules your recommendation, say so in the bullet. When a reaction collides with the banned list ([BANNED-DEFAULTS.md](BANNED-DEFAULTS.md)), flag it for a later round.
4. Append the round to the log: what was shown, the user's words close to verbatim, and the Taken bullets. Do this before asking the next round, so a context reset loses nothing.
5. Open the next round by restating the Taken bullets in a line or two; the user corrects anything you misread.

Done when every dimension in ROUNDS.md that applies to this project has a pick, and the hero moment has been seen whole in a mock. A pick the user calls "good enough for now" counts: mark it provisional and name where it gets judged again.

## 3. Draft the spec

Fill the rest of `DESIGN.md` from the template: rules, tokens, and page patterns (the banned list is already in place from Ground, narrowed by whatever the rounds changed). Every token and rule gets a reason that points at a round ("round 7: white page, one blue accent"). A value you can't tie to a round or to section 1 is a **gap**; mark it and keep going.

Done when every section of the template is filled or marked as a gap.

## 4. Gap grill

Scan the draft for gaps using [GAPS.md](GAPS.md): values with no reason, cases no round covered, two picks that contradict each other, a pick that breaks a rule. Grill the user on those only; settled ground stays settled. Show visual gaps in the mock. Log each pass as "Gap grill N" and update the draft.

Done when a fresh scan finds no gaps.

## 5. "Would any other app make this choice?"

For every choice in the draft, ask whether any other product in the same category would make it too. Record a table in `DESIGN.md` with one verdict per choice:
- **Ours:** only makes sense for this product's subject.
- **Generic, kept on purpose:** another app could pick it too, and the user did so deliberately (cite the round).
- **Generic, changed:** propose a replacement that comes from this product's subject, and get the user's OK.

Also look at 3 to 5 well-known products in the category for one specific thing each worth borrowing, and say which you'd take.

Then write "What makes this look like itself" in three sentences. If they read as if they could describe any app in the category, the review isn't done.

Done when every choice has a verdict, every "changed" row is approved, and the three sentences name things only this product has.

## 6. Approve

The user checks the final mock on the device they'll actually use (usually a phone), in every theme the spec defines. Record the approval date in `DESIGN.md` and in the log. Close by listing what the spec hands off to the build: the token file, a specimen page, the hero screen, and the automated checks in the spec.
