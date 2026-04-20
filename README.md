# Bivalent Comments

A Claude skill for generating short comments that sit on the fence between sincere support and unmarked sarcasm — comments engineered so that supporters of the source material read them as validation, and detractors read them as ridicule, without the comment itself ever committing to either stance.

Install the `.skill` file into Claude, provide any article, transcript, headline, tweet, or video description, and the skill returns three candidate comments optimised for bilateral resonance.

## What is a bivalent comment?

A bivalent comment achieves four things simultaneously:

1. **Positive-dominant surface.** Read literally, the comment agrees with or amplifies the source claim. A supporter parses it as genuine support and engages positively.
2. **Unmarked sarcasm substrate.** A skeptic reads the same words and finds a sarcastic interpretation — but the sarcasm is supplied by the reader, never signalled by the writer. No `/s`, no eye-roll emoji, no tonal giveaway. Marking the sarcasm would collapse the mechanism and lose the supporter audience.
3. **Brevity.** Short comments stay on the fence because there isn't enough surface area to fall off it. Every additional word risks tipping toward one camp. Targets are typically under fifteen words.
4. **Plausible deniability in both directions.** Challenged by a supporter, the writer meant it sincerely. Challenged by a detractor, obviously they were being dry. Neither camp can prove which it was, because it is genuinely both.

### The anchoring example

A viral video claims: *"This house was built for $10 with dirt."*

A bivalent comment: *"Wow, you can't even buy two cups of coffee for $10."*

The phrase "two cups of coffee" does double duty — it is simultaneously a real price reference that makes the cheapness vivid and impressive, and a standard sarcastic trope for "this number is suspiciously low." The phrase works for both audiences and commits to neither.

## How the skill works

The skill operates in two passes:

**Pass 1 — Angle selection.** It reads the source material and identifies a single element with *structural bivalence available to it*: a suspiciously low or high number, a bold transformation claim, a superlative, an implausible timeframe, a before/after contrast. Elements without a bivalent hook are rejected and the skill keeps searching.

**Pass 2 — Three phrasings.** All three candidate comments engage the same angle via the same mechanism. They differ only in wording — one leans slightly warmer (easier sincere reading), one leans slightly drier (easier skeptical reading), one sits maximally in the middle. None crosses into marked sarcasm or pure sincerity.

The output is three numbered lines and nothing else — no explanation, no bivalence notes, no ranking. The operator picks.

## Example output

**Source:** *"Tech startup raises $200M Series A, valued at $3 billion, with no product launched yet."*

```
1. Three billion before shipping anything, investors really see the vision
2. Two hundred million on potential alone, what a time for founders
3. Valued at three billion pre-launch, the future is already here
```

Each engages the valuation-without-product gap. Each reads as "wow, belief in the team" to a supporter and as "classic bubble behaviour" to a skeptic. None of the three says either.

## Triggering

The skill triggers on any request for comments on articles, video transcripts, headlines, social posts, or any published content — including phrases like "bivalent comment", "fence-sitter comment", "doublespeak comment", "write a comment that both sides upvote", or "viral comment." It's particularly well-suited to pairing with a video-understanding model that hands it a description or transcript to work from.

## Installation

Download `bivalent-comments.skill` from the releases and install it via the Claude skills interface.

## 📚 Citation

### Academic Citation

If you use this codebase in your research or project, please cite:

```bibtex
@software{bivalent_comments_skill,
  title = {Bivalent Comments: A Claude skill for generating doublespeak comments with bilateral audience resonance},
  author = {[Drift Johnson]},
  year = {2025},
  url = {https://github.com/MushroomFleet/bivalent-comments-skill},
  version = {1.0.0}
}
```

### Donate:

[![Ko-Fi](https://cdn.ko-fi.com/cdn/kofi3.png?v=3)](https://ko-fi.com/driftjohnson)
