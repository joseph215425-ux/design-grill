# Progress

## Now
- **Phase:** v0.1 published, repo public
- **Current step:** all checklist items done — repo public, install copy-folder only, throwaway test folders confirmed gone. Nothing blocking.
- **Model:** opusplan
- **Last updated:** 2026-09-25

## Next steps
- [x] Skill files: SKILL.md, ROUNDS.md, GAPS.md, BANNED-DEFAULTS.md, templates
- [x] README with credit to Matt Pocock's grilling skill; MIT LICENSE with his notice
- [x] Anonymized worked example (`examples/voice-archive.md`)
- [x] Joseph reads the example and OKs his (anonymized) words going public
- [x] Dry run #1 on a small made-up project (`~/claude/design-grill-test`, "Pantry") — friction list compiled
- [x] Grill Joseph through dry run #1's 7 proposed fixes — all answered, applied
- [x] Dry run #2 on a new throwaway project (`~/claude/design-grill-test-2`, "Fieldmark") — self-driven, reached mock-switching, three gap-grill passes, and the borrowing scan; friction list compiled
- [x] Grill Joseph through dry run #2's 5 proposed fixes — all answered, see resolutions below
- [x] Apply the agreed fixes to `skills/design-grill/`
- [x] Delete `~/claude/design-grill-test` and `~/claude/design-grill-test-2` — already gone, nothing to delete
- [x] Decide: also package as a Claude Code plugin (marketplace install) or copy-folder install only — decided copy-folder only, no plugin manifest
- [x] Flip the GitHub repo to public — confirmed public via GitHub API 2026-09-25

## Known issues
- None open. Resolutions from dry run #1's fix grill (2026-09-25):
  1. `DESIGN.md` now has an explicit output path: `docs/design/DESIGN.md` (`SKILL.md` step 1.1).
  2. Banned list is copied into `DESIGN.md` during Ground (step 1), not at step 3; rounds narrow it in place. Fixed the wording conflict between `BANNED-DEFAULTS.md` and `SKILL.md` step 3.
  3. Ground confirmation (`SKILL.md` step 1.2) now explicitly uses the same numbered/recommend/wait grill format as reaction rounds, filtered to only the fields the project's own materials didn't already make clear.
  4. Numbering + A/B/C-labeled options together was untested at the time — resolved in dry run #2, see below.
  5. `README.md`'s Install section now warns that skills load at session start, so copying mid-session needs a fresh session before it's invocable.
  6. Decided to run a second, longer dry run before flipping the repo public — done, see below.
  7. Decided self-driven mechanical reaction rounds (used to dry-run without a live user) stay an undocumented one-off testing accommodation, not documented skill behavior.
- Resolutions from dry run #2's fix grill (2026-09-25):
  1. Numbering + A/B/C-labeled options together, tested in gap grill 1 and reads clearly — `SKILL.md`'s "untested" note replaced with a line stating the pattern.
  2. Two gap-scan passes each missed real gaps by scanning GAPS.md's uncovered-cases list for an overall impression rather than line by line — `GAPS.md` now says to check every line.
  3. A mock's own scaffolding (its version label) violated the banned-defaults list and nothing in the reaction rounds was positioned to catch it — `ROUNDS.md` now says to keep scaffolding in plain browser-default styling, out of the design system.
  4. Confirmed, not a defect: Approve still can't be dry-run without a real approver on a real device.
  5. An unresolved "Generic, changed" row in the borrowing scan now explicitly blocks Approve — `SKILL.md` step 5 says to loop back rather than move on.
