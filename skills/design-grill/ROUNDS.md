# Running the reaction rounds

## Dimension order

Broad to narrow, so each round builds on settled ground. Skip any that don't apply; split any the user has a lot to say about.

1. **Overall feel:** what kind of object this is (a book, a tool, a feed, a magazine).
2. **Pull:** what makes someone want to keep tapping (people, polish, big headlines, images).
3. **Title type:** the face with personality, for headings.
4. **Reading type:** the face for long text. Often the same round as 3 when one family will do.
5. **Color:** the base (page, text, greys), then the accent, then any color families that carry meaning.
6. **Color strength:** pastel vs soft vs vivid, shown in a mock with the product's own content.
7. **Pictures:** what visuals exist, and where they come from.
8. **Density:** big cards vs compact rows, per list.
9. **The hero moment:** the screen named in step 1, in two or three layouts.
10. **Secondary screens:** the next most important pages.
11. **Pairing on a whole page:** the chosen faces and colors on one complete hero screen, with a switch for any still-provisional pick.

## Picking links

- Links go to specific public pages that load without a login: one article, one font specimen, one changelog. A home page shows too many ideas at once.
- The options in a round differ on the round's dimension and as little else as possible. Label each by what it stands for ("A. book/magazine, B. scholar's archive, C. precise tool"), so a reaction to it is a reaction to that idea.
- Mix in an option you wouldn't recommend. Rejections teach as much as picks.
- For fonts, link each font's specimen page and ask the user to type or paste a real sentence from the product into it, at the size it will be used.
- Expect the user to be on a phone. Pick pages that hold up there.
- When a round needs no visuals (a yes/no on an idea, a rule), ask questions only.

## Switching to a mock

Links stop helping once the question is how *this* product looks, usually by the color-strength round. From then on, build one self-contained HTML mock and keep updating it:

- One page, one stable URL or file path for the whole grill, with a version number in the page and in the log (v1, v2...). Use a hosted page if the harness can publish one; otherwise a local HTML file the user opens.
- Made-up content shaped like the real thing (realistic names, lengths, numbers), never the user's private data.
- Options side by side, or behind a small switch, labeled to match the round's question.
- Newest section at the top; remove options once they're decided so the page stays readable.
- Check it at phone width yourself before sending. When the user reports a mock behaving oddly, fix it if the behavior is part of the design question; otherwise say it's a mock limitation.
- Commit the mock's source next to the log so it survives the session.

## Reading reactions

| The user says | Do this |
|---|---|
| "I don't love any of them, but B is closest" | Take B's direction, then run a narrower round inside it. |
| "B is good enough for now" | Take B as provisional and name where it gets judged again (the specimen page, the real hero screen). |
| "I want images" but images are costly or would look fake | Find what can be drawn from the product's own data, and mock several kinds. |
| "It looks like AI" | That's a real signal about generic, generated looks. Find which element triggers it (a big number on a tint, a gradient, a stock-art feel), then retry that element in a different form. |
| A feature idea that isn't about looks | Log it as parked, with the user's words, and return to the round. It becomes a product decision elsewhere. |
| A pick that breaks the banned list | Ask what the user likes about it. If it carries real information (a tappable tag above a title), narrow the ban to the decorative version; otherwise, keep the ban and find another way to give them what they liked. |
| A size, spacing, or behavior complaint on the mock ("text feels too big") | Fix it in the mock, name the new values, and re-check at phone width. |
| A new idea the user brings up themselves | Treat it as a candidate, not a decision: mock it, then confirm. |

After each round, check whether anything the user said reopens an earlier pick. If it does, say so and settle it next round rather than silently overwriting it.
