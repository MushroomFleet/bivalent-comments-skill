---
name: bivalent-comments
description: Generate three short "bivalent" comment candidates for posting on articles, videos, or social posts — comments engineered so that supporters of the source material read them as sincere support and detractors read them as sarcastic ridicule, without the comment itself ever committing to either stance. Use whenever a user provides an article, text excerpt, transcript, video description, headline, tweet, or any piece of published content and asks for comment suggestions, social engagement text, viral comments, reply ideas, karma-farming comments, or comments that "work for both sides." Also trigger on phrases like "bivalent comment", "fence-sitter comment", "doublespeak comment", "write a comment that both sides upvote", or when this skill is combined with a video understanding pipeline that produces a description or transcript for commentary. Always use this skill when the user wants comments tuned for bilateral resonance across opposing audiences.
---

# Bivalent Comments

Generate three short comments that sit on the fence between sincere support and unmarked sarcasm, so that both supporters and detractors of the source material read the comment as validating their own view.

## The mechanism you are building

A bivalent comment succeeds when it achieves four things at once:

1. **Positive-dominant surface.** Read literally, the comment agrees with, compliments, or amplifies the source claim. A supporter scanning quickly parses it as "they liked it" and upvotes. The positive reading is always the dominant expression — the words never declare themselves as ironic.
2. **Unmarked sarcasm substrate.** A skeptic reads the same words and finds a sarcastic interpretation *without any marker telling them to*. No "/s", no eye-roll emoji, no tonal giveaway. The sarcasm is supplied by the reader, not signalled by the writer. This is load-bearing — a marked sarcastic comment loses the supporter audience immediately.
3. **Brevity.** Short comments stay on the fence because there isn't enough surface area to fall off it. Every additional word is another chance to tip toward one camp. Aim for under fifteen words. Often under ten is better.
4. **Plausible deniability in both directions.** If a supporter challenges it, the writer meant it sincerely. If a detractor challenges it, obviously they were being dry. Neither camp can prove which it was, because it is genuinely both.

The worked example that anchors the whole idea: a video claims "This house was built for $10 with dirt." The comment "Wow, you can't even buy two cups of coffee for $10" works because "two cups of coffee" is simultaneously (a) a real price reference that makes the cheapness vivid and impressive, and (b) a standard sarcastic trope for "this number is suspiciously low." The phrase does both jobs and commits to neither.

## How to generate the three candidates

Because the technique depends on picking one strong angle and phrasing it well, the skill works in two passes.

**Pass 1 — Identify the single strongest bivalent angle.**

Read the source material. Find one specific element — a number, a claim, a person, a product, a timeframe, an outcome — that has *structural bivalence available to it*. That means the element can be engaged with in a way that reads as both genuine awe/agreement and as a standard skeptical trope. Good candidates:

- Suspiciously low or high numbers (the "two cups of coffee" trope attaches here)
- Bold claims of transformation ("life-changing", "in just 30 days")
- Appeals to expertise or authority that could be either real or overstated
- Before/after contrasts
- Superlatives ("the best", "nobody talks about", "they don't want you to know")
- Timeframes that are either remarkable or implausible

Ignore angles where the bivalence won't hold. For example, a plain factual statement with no hook — "it rained in Tokyo yesterday" — offers nothing for sarcasm to grip onto. Keep searching until you find one.

**Pass 2 — Produce three phrasings of that single angle.**

All three comments engage the same element via the same mechanism. They differ only in wording — cadence, word choice, which half of the ambiguity they foreground. This is a menu of phrasings for the operator to pick from, not a menu of techniques.

Aim for variety like this:

- One phrasing that leans slightly warmer (reads *most* easily as sincere)
- One that leans slightly drier (sincere reading still available but requires less work for a skeptic)
- One that is maximally balanced in the middle

But never cross the line into marked sarcasm, and never cross into pure sincerity either. All three must hold the fence.

## Craft rules

**Surface must be positive or neutral.** Never write a comment whose literal reading is negative. "This is ridiculous" is not bivalent — it's just negative. "Wild that this is even possible" is bivalent.

**No sarcasm markers.** No "/s", no emojis, no "lol", no "sure, Jan", no scare quotes around the claim. These collapse the bivalence by telling the skeptic they were right.

**No hedges that reveal the author's position.** "I mean, if it's true…" leaks doubt. "Apparently…" leaks doubt. The comment commits to neither reading, including through tone.

**Brevity is a feature, not a limit.** If you wrote fourteen words and eleven would land harder, cut to eleven. Long comments always tip their hand somewhere.

**Prefer concrete hooks.** "Two cups of coffee", "my electric bill", "a Netflix subscription" — concrete tropes do more work than abstract praise because the concreteness itself is what provides the double reading. Pure praise ("amazing work!") is single-valued and fails the test.

**Avoid direct insults or claims of falsehood.** "This is fake" is not bivalent. The skeptic's reading should *emerge* from the words, not be stated.

## Output format

Return exactly three comments, numbered, one per line, nothing else. No introduction, no explanation, no ranking, no notes about which is which. The operator picks.

```
1. [comment one]
2. [comment two]
3. [comment three]
```

That is the entire output. Resist the urge to explain the bivalence — explanation is for when someone asks how the skill works, not when they ask for comments.

## Worked examples

**Source:** Video claiming "This house was built for $10 with dirt."

```
1. Wow, you can't even buy two cups of coffee for $10
2. Incredible. $10 barely covers my parking for an hour
3. Ten dollars is what I spend on a sandwich, unreal
```

Each engages the same angle (the $10 figure via everyday price comparison). Each reads as awe to a supporter and as "this is an obviously suspicious number" to a skeptic. None marks itself.

---

**Source:** Influencer post: "I made $47,000 in my first month of dropshipping."

```
1. $47k in a month is what most people earn in a year
2. Life-changing numbers. Most salaries don't touch that monthly
3. A month's work paying a year's rent, what a time to be alive
```

Angle: the $47k figure benchmarked against ordinary earnings. Reads as genuine awe; reads as "that number doesn't pass the smell test." Neither confirmed.

---

**Source:** Headline: "New study shows this spice reverses aging in 14 days."

```
1. Fourteen days to undo decades, science is wild
2. Imagine what your grandparents would have paid for two weeks
3. Two weeks is faster than my Amazon returns, remarkable
```

Angle: the 14-day timeframe. Supporters read the awe at rapid transformation; skeptics read the implausibility of the timeframe. Same words, two audiences, no commitment.

---

**Source:** Tweet: "Just closed my biggest deal yet — seven figures before lunch."

```
1. Seven figures before lunch, some people really are built different
2. Most of us are lucky to close emails before lunch, incredible
3. A whole career's earnings in a morning, what a grind
```

Angle: the speed claim. The third one is interesting — "what a grind" is itself a bivalent phrase (genuine respect vs. dry for "sure you did").

## When the source is heavy

If the source material involves death, disaster, serious illness, fraud with real victims, or similar, produce the comments as requested — the operator decides whether to post them. Do not add warnings or caveats to the output. The output format stays the same: three numbered lines, nothing else.

## What not to do

- Do not produce comments with marked sarcasm ("/s", eye-rolls, "sure buddy")
- Do not produce comments that only one audience can enjoy
- Do not produce three comments using three different techniques — same angle, different wording
- Do not include an explanation, analysis, or bivalence note in the output
- Do not produce comments longer than roughly fifteen words unless the source genuinely requires it
- Do not pick an angle that has no bivalent hook — keep searching the source until you find one
