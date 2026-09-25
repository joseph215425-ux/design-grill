# design-grill

A Claude Code skill for people who know good design when they see it but can't say what they want.

Instead of asking you for a mood board or a list of adjectives, Claude shows you a few live web pages or mocks per round, each option different in one way, and you just react: "I like B, A feels like a chore, I don't know why." Claude turns each reaction into a concrete design choice, logs your words and what it took from them, and keeps going until every part of the look is decided. The result is a `DESIGN.md` you've approved on your own phone, ready to build from.

## How it works

1. **Ground.** Claude reads your project and writes down what the product is made of, who uses it on what device, and which screen matters most (the *hero moment*). You confirm.
2. **Reaction rounds.** One dimension per round, broad to narrow: overall feel, what pulls you in, title font, reading font, color, color strength, pictures, density, the hero screen, then a whole page. Early rounds use real web pages; once the question is about *your* product, Claude switches to a single HTML mock it updates every round.
3. **Draft the spec.** Every rule and token cites the round it came from.
4. **Gap grill.** Claude hunts for anything the draft decided by default (dark mode, navigation, a fifth category color, empty states...) and asks about only those.
5. **"Would any other app make this choice?"** Every choice is checked for genericness. Generic ones are either kept deliberately or replaced with something that comes from your product's subject.
6. **Approve** on the device you'll actually use.

Everything is logged to `docs/design/grill-log.md` after every round, so a cleared context or a new session loses nothing.

See [examples/voice-archive.md](examples/voice-archive.md) for excerpts from a real 24-round grill.

## Install

Copy the `skills/design-grill` folder into one of:
- `~/.claude/skills/` to use it in every project, or
- `<your project>/.claude/skills/` for one project.

Then, in Claude Code, say "design grill" or type `/design-grill`.

## What's in the skill

| File | What it is |
|---|---|
| `SKILL.md` | The six steps and when each is done. |
| `ROUNDS.md` | Dimension order, how to pick links, when to switch to a mock, how to read common reactions ("it looks like AI", "good enough for now"). |
| `GAPS.md` | What to scan the draft for in the gap grill. |
| `BANNED-DEFAULTS.md` | A starter list of looks that signal nobody decided. |
| `templates/` | The `DESIGN.md` and log skeletons. |

## Credits

The round-by-round questioning is adapted from Matt Pocock's [grilling skill](https://github.com/mattpocock/skills) ("grill me"): map the decisions as a tree, ask every question whose prerequisites are settled, give a recommendation for each, then wait. design-grill specializes it for visual design, adds the reaction-and-translate loop, mocks, the gap grill, and the genericness review, and runs without needing his skill installed. Used under the MIT License; his notice is included in [LICENSE](LICENSE).

The process was worked out while designing a personal voice-notes app with Claude Code.

## License

MIT. See [LICENSE](LICENSE).
