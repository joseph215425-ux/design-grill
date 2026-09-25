# Worked example: a voice-notes archive

Excerpts from a real design grill (24 reaction rounds, 3 gap grills, then the review), lightly trimmed and anonymized. The product: a private, phone-first app that turns recorded conversations, classes, and voice memos into notes, and builds a profile of each person the owner talks to. The owner is not a designer. They knew what they liked when they saw it and couldn't have written any of this down beforehand.

## Round 1: overall feel
Links (contrast: what kind of object the app feels like):
- A. Book/magazine: https://craigmod.com/essays/
- B. Scholar's archive: https://gwern.net/
- C. Precise tool: https://docs.stripe.com/

Recommended: A, a calm book for rereading.

The owner's words:
> It doesn't really entice me to tap anything. [B is] too bare bones. When I open my app I want it to feel nice. I want to feel enticed to read the different things. Almost like social media in a way. I don't want the app to feel like a chore to use. The best of these three is C, but even then it's not perfect.

Taken:
- **Inviting over austere.** Closer to a feed than a document. Overruled the recommendation.
- **Not bare bones.** Pages need visible structure and things that look tappable.
- **C is closest:** clear hierarchy, obvious links. Not the target on its own.

## Round 2: where the pull comes from
Links: A. people and their takes (Letterboxd), B. polish (Linear changelog), C. big bold headlines (Apple Newsroom).

The owner's words (trimmed):
> Some sort of picture would be nice, but I don't want my app to feel like AI. I like the big bold titles of Apple's newsroom, and the name at the top that you can tap to go back up. The date in smaller text in a slightly different color, and above the headline a tag of sorts. I'm leaning towards a light app.

Taken:
- **Light-first.**
- **From C:** big confident headlines, a sticky top bar that scrolls to top, the date small and grey, a small tag above the headline.
- **Wants images, but nothing AI-generated.** Open question: where visuals come from.
- **Conflicts with the banned list:** a label above the headline. Settled in round 3: allowed when it's real, tappable data.

## Round 5: title typeface, narrowed
After round 4's "I don't love any of them, but A", three fonts inside A's direction: Plus Jakarta Sans, Instrument Sans, Geist.

> My favorite is B. Really what I'm basing it on is readability. Can we pick B and keep going, and change it later if I don't like it?

Taken:
- **Instrument Sans, provisional.** The owner's test for fonts is readability. Judged again on a whole page in round 22, where it stuck.

## Round 8: color strength, via a mock
From here on, one HTML mock at a fixed URL, updated each round. v1 showed a white page, a blue accent, the chosen fonts, and three strengths of speaker color: pastel, soft but bright, vivid.

> I really like this. I want to go with B. I'd like some black at the top like Apple's newsroom, and the bar stuck at the top to be transparent. The recording picture is nice, it almost looks like an instrument, but I'd like other images as well.

Taken:
- **Soft but bright** for speaker colors.
- **Black, see-through sticky bar.** Blur allowed here only, because the bar really floats.
- **The "who spoke when" picture works.** Pictures drawn from the recording's own data answer round 2's "no AI images."

## Round 11: picture types
Mock v3 showed six picture types drawn from each note: who spoke when, a quote card, a voice shape, topic bubbles, a key figure, a moments line.

> I like all of them except the dollar amount. It looks like AI.

Taken:
- **A big bold number on a tinted card reads as generated.** The idea stays; the form goes. After six tries it landed as the quote where the number was said, with the number underlined in the speaker's color.

## Gap grill 2
The draft spec left the dark palette, status colors, and icon weight as defaults. Mock v20 showed each.

> Dark mode reads well. Status colors look better in dark than light. The three icon weights looked identical.

Settled: the dark palette as shown; light mode gets two shades per status color (bright for dots, dark only for text); icons compared again at a bigger size, and Regular picked.

## The review: "would any other notes app make this choice?"
| Choice | Verdict |
|---|---|
| White page, near-black text, cool greys, blue links | Generic, kept on purpose (round 2). |
| Speaker colors across transcript, faces, quotes, tags | Ours. Only makes sense in an app built on who said what. |
| Note pictures drawn from the recording | Ours. Replaces the stock hero image most apps default to. |
| Action items list | Generic, changed: each item shows who owns it in their speaker color and opens the recording at the moment it was said. |
| Search results | Generic, changed: under each result, the matching spoken line (borrowed from Apple Podcasts' transcript search). |

What makes it look like itself: every picture is drawn from the recording itself, so nothing looks like stock or AI art. Each person keeps one color across the transcript, their face, and their quotes, so you follow people by color. The page reads like a book (serif text, upright quotes, italic and bold with a job) under a bold sans and a black see-through bar.
