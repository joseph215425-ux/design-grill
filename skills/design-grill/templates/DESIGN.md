# Design

The visual system for <product>. Written in a design grill (log: `docs/design/grill-log.md`). Every session that touches the UI reads this file. After approval, the tokens and rules are fixed: changing one is a design change the owner approves.

## 1. What this product is
- **Subject:** what it's made of (e.g. spoken conversations and the people in them; recipes and their ingredients).
- **Primary job:** what a typical visit does.
- **Audience:** who uses it, on what device, in what situation.
- **Consequence:** what that means for the look. Distinctive choices come from the subject, not from the product category.

## 2. The hero moment
The one screen that gets the most design effort and that every later page copies. Then the second priority.

## 3. Rules
One short list per area. Each rule states what to do, and cites the round it came from.
- **Color:** where colors live (tokens only), the roles, what the accent is for, what each color family means, contrast minimums, light/dark.
- **Type:** families and their jobs, the scale (named steps, no other sizes), emphasis (what italic and bold mean), case.
- **Shape and depth:** radius by role, what a shadow means, when something is a card.
- **Spacing and layout:** the spacing scale, phone layout, desktop layout.
- **Icons:** where icons are used, the set, the weight, the size per context.
- **Pictures:** what visuals exist and where they come from.
- **Motion:** what moves and why.
- **Copy:** button wording, errors, empty states.

## 4. Banned defaults
Starting from the skill's starter list, as adjusted in the rounds.

## 5. Tokens
### References and what was taken from each
| Source | Round | Taken |
|---|---|---|

### Palette
| Role | Light | Dark | Use |
|---|---|---|---|

### Typefaces
### Type scale
### Spacing scale
### Radius by role
### Shadow
### Icon set, weight, and sizes
### Page patterns
The hero screen and the other settled layouts, one short paragraph each.

## 6. "Would any other app make this choice?"
| Choice | Verdict |
|---|---|

### What makes this look like itself
Three sentences, naming things only this product has.

## 7. Checks
- **Self-critique checklist** to answer in writing before showing any new page (radius by role, shadows only on floating things, one obvious first thing to look at, nothing decorative, nothing banned, readable in every theme, tap targets at least 44 points, one thing removed).
- **Automated checks** the build should run (no color literals outside the token file, sizes from the scale only, contrast of every text/background pair, no external font URLs).

## Approved
<date>, on <device>.
