# Progress

## Now
- **Phase:** first draft of the skill, private repo
- **Current step:** dry run complete (throwaway test project `~/claude/design-grill-test`, made-up "Pantry" app, ground + 3 reaction rounds + 1 gap-grill question + review). Compiled a 6-item friction list of what was unclear/missing/guessed in the skill files. Now grilling through the proposed fixes with Joseph one question at a time (per the new one-question-per-message habit — see vault `_system/CLAUDE-global.md`). Stopped mid-grill at Q1 of 7 (Q1: add explicit `DESIGN.md` output path to `SKILL.md` step 1.1) — Joseph had not yet answered when this session paused.
- **Model:** opusplan
- **Last updated:** 2026-09-25

## Next steps
- [x] Skill files: SKILL.md, ROUNDS.md, GAPS.md, BANNED-DEFAULTS.md, templates
- [x] README with credit to Matt Pocock's grilling skill; MIT LICENSE with his notice
- [x] Anonymized worked example (`examples/voice-archive.md`)
- [ ] Joseph reads the example and OKs his (anonymized) words going public
- [x] Dry run on a small made-up project (`~/claude/design-grill-test`, "Pantry") — friction list compiled, see below
- [ ] Finish grilling Joseph through the 7 proposed fixes (Q1 of 7 asked, unanswered) — resume one question at a time
- [ ] Apply the agreed fixes to `skills/design-grill/` (not yet touched — dry run only wrote to the throwaway test project)
- [ ] Delete `~/claude/design-grill-test` once the fixes are applied and confirmed (throwaway, not a repo, never push it)
- [ ] Decide: also package as a Claude Code plugin (marketplace install) or copy-folder install only
- [ ] Flip the GitHub repo to public

## Known issues
- Dry run only exercised Ground, 3 early reaction rounds (link-based), 1 gap-grill question, and the review — never reached the mock-switching mechanics (round 8+), the full gap scan, or the borrowing scan. Those are the most complex instructions in `ROUNDS.md`/`GAPS.md` and haven't been proven clear. Recommend a second, longer dry run before flipping the repo public (see grill Q6).
- Friction list from the dry run, pending the grill's resolution (see grill-log style summary below):
  1. `DESIGN.md`'s output path is never stated in `SKILL.md` (in grill, Q1).
  2. Real conflict: `BANNED-DEFAULTS.md` says copy the banned list into `DESIGN.md` "at the start of the grill"; `SKILL.md` step 3 treats it as filled in after all reaction rounds (in grill, Q2).
  3. `SKILL.md` step 1.2 (Ground confirmation) doesn't say whether it follows the same numbered/recommend/wait format as reaction rounds, or how to read "ask only for what the project can't tell you" (in grill, Q3).
  4. Numbering + A/B/C-labeled options together is untested — never hit a round with two simultaneous frontier questions (in grill, Q4; leaning: leave as a noted open question rather than guess a fix).
  5. `README.md`'s Install section doesn't warn that copying the skill mid-session won't make it invocable until a fresh session (in grill, Q5).
  6. Whether to run a second, longer dry run before going public, to cover what this one skipped (in grill, Q6).
  7. Whether "Claude can self-drive mechanical reaction rounds during a dry run" should become documented skill behavior, or stay a one-off accommodation (in grill, Q7; leaning: leave undocumented, real users won't want this).
