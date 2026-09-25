# Progress

## Now
- **Phase:** first draft of the skill, private repo
- **Current step:** grill on the dry-run friction list is done (all 7 questions answered) and the agreed fixes are applied to `skills/design-grill/` and `README.md`. Next up is a second, longer dry run before going public.
- **Model:** opusplan
- **Last updated:** 2026-09-25

## Next steps
- [x] Skill files: SKILL.md, ROUNDS.md, GAPS.md, BANNED-DEFAULTS.md, templates
- [x] README with credit to Matt Pocock's grilling skill; MIT LICENSE with his notice
- [x] Anonymized worked example (`examples/voice-archive.md`)
- [ ] Joseph reads the example and OKs his (anonymized) words going public
- [x] Dry run #1 on a small made-up project (`~/claude/design-grill-test`, "Pantry") — friction list compiled
- [x] Grill Joseph through the 7 proposed fixes — all answered, see resolutions below
- [x] Apply the agreed fixes to `skills/design-grill/` and `README.md`
- [ ] Run a second, longer dry run (new throwaway test project) that reaches mock-switching (round 8+), the full gap scan, and the borrowing scan — none of which dry run #1 exercised
- [ ] Delete `~/claude/design-grill-test` once the second dry run is done and confirmed (throwaway, not a repo, never push it)
- [ ] Decide: also package as a Claude Code plugin (marketplace install) or copy-folder install only
- [ ] Flip the GitHub repo to public

## Known issues
- None open. Resolutions from the fix grill (2026-09-25):
  1. `DESIGN.md` now has an explicit output path: `docs/design/DESIGN.md` (`SKILL.md` step 1.1).
  2. Banned list is copied into `DESIGN.md` during Ground (step 1), not at step 3; rounds narrow it in place. Fixed the wording conflict between `BANNED-DEFAULTS.md` and `SKILL.md` step 3.
  3. Ground confirmation (`SKILL.md` step 1.2) now explicitly uses the same numbered/recommend/wait grill format as reaction rounds, filtered to only the fields the project's own materials didn't already make clear.
  4. Numbering + A/B/C-labeled options together is still untested (never hit a round with two simultaneous frontier questions) — left as a noted open question in `SKILL.md` rather than guessing a fix.
  5. `README.md`'s Install section now warns that skills load at session start, so copying mid-session needs a fresh session before it's invocable.
  6. Decided to run a second, longer dry run before flipping the repo public — see Next steps.
  7. Decided self-driven mechanical reaction rounds (used to dry-run without a live user) stay an undocumented one-off testing accommodation, not documented skill behavior.
