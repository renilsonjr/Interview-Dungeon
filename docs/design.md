# Design

Everything decided so far. The first path is in
[`paths/google-swe-intern.md`](paths/google-swe-intern.md).

## Core model

- **Shared skill tree.** Every skill (arrays, STAR stories, SQL modeling...) exists
  once. You study it once.
- **Dungeons are weights on that tree.** A dungeon (path) says how much each skill
  matters for that interview. One cleared challenge moves every dungeon that uses
  that skill, each by a different amount.
- **Trust labels** on every requirement: Official, Reported, Estimated.
- **Proof.** Clearing a floor in the game is the proof that you know that skill, as of
  that date. Notes and outside evidence don't count as proof.
- **No decay.** A cleared floor keeps its full value. The record shows the date it was
  cleared, and the player judges how fresh it is.

## Structure of a dungeon

| Piece | What it is |
|---|---|
| Zone | A group of floors (4 per dungeon) |
| Floor | One playable unit: a skill or an interview stage |
| Run | The steps inside a floor |
| Boss | Closes a floor. Copies the real interview format |
| Final boss | The full interview loop. Adds 0% and confirms the 100% |

**Free order.** Every floor is open from the start. Only real prerequisites seal a
boss (for example, Trees needs Recursion). You can still practice on a sealed floor.

## Challenge types

| Type | Used for |
|---|---|
| Code | Problems in a plain editor, no autocomplete |
| Quiz | Pattern recognition, Big-O, constraints |
| Text check | Resume, "tell me about yourself", STAR stories. You write or speak, and a checklist shows what's missing |
| Narration | Code plus a spoken or typed transcript of your thinking |
| Timed mock | Online assessments and the full loop |

## Rules of play

- **Running code** is allowed in normal steps and blocked in bosses. Exception: online
  assessment bosses, because real OAs allow running sample tests.
- **Boss submissions** are unlimited within the time limit. The first fully correct one
  wins. The number of submissions is kept in the history.
- **After submitting** you always see which hidden tests failed and the input that
  broke your code.
- **Losing a boss** sends you to one extra practice problem before the rematch. You
  still earn XP for the attempt.
- **Weights inside a run:** the boss is worth 4 times a normal step (starting value).
- **XP and level** measure effort and only go up. **Readiness** measures how close you
  are to one dungeon. They're never mixed.
- **Attributes are earned, never allocated.** There are no points to spend on level up.
- **The final boss** is open at any time, always with a warning listing what isn't
  cleared. A path is sealed only when every floor is cleared **and** the final boss is
  beaten. Early attempts are logged as practice runs.
- **Quizzes:** wrong answers come back at the end. The step clears when every question
  has been answered correctly once.
- **Voice or text** for narration and stories. A boss beaten by voice gets a "spoken" mark.

## Content

- Problems are generated with AI, inspired by each floor's pattern, with original wording.
- Pipeline: **generate** (with a reference solution and tests) → **automatic check**
  (a separate brute-force solution must agree on the tests and on random inputs, or the
  problem is discarded) → **human approval** → official pool.
- In-game **"this problem is unfair"** button: the problem leaves the pool, and a loss to
  it doesn't count.
- Text checks have two layers: **simple rules** for what can be counted (length, "I" vs
  "we", a concrete result) and an **AI judge** for quality. The AI only reviews drafts
  that pass the rules. Truthfulness isn't checked; honesty is the player's responsibility.
- **Language:** learning pages in English or Brazilian Portuguese. Code, challenges,
  quizzes, bosses and text checks in English, the language you're graded in.

## Screens

Game screens look like Diablo 1. Work screens are clean and readable, with a thin dark
bar on top (back, floor, timer, mini orbs) as the bridge between the two. Every screen
has a Back button.

| Game style | Clean style |
|---|---|
| Title | Learning page |
| Hero selection, with "New hero" | Quiz |
| Class (cosmetic only) and name | Code challenge |
| Dungeon selection (several can be active) | Text check |
| Character: two orbs, red for the current dungeon's readiness, blue for XP, plus a list of every active dungeon | Narration |
| The descent: the full map of one dungeon | Timed mock |
| Boss intro, victory, defeat, final warning, level up | |

- **Classes** (Warrior, Sorcerer, Rogue, Barbarian...) only change how the hero looks.
- **Uncharted dungeons** (researched but not designed yet) appear without a percentage.
- **Bosses** have generic names for now ("The Arrays guardian").

## The dev scroll

The game is also a dev diary.

- A **general scroll** on the Character screen: free text for what you learned, or
  anything extra, inside or outside the game.
- **Notes for each zone and each floor** in the descent (Steps and Notes tabs). The
  map marks the ones that have notes.
- Notes belong to their dungeon, are plain text, show the date of the last edit, and
  **never change XP, readiness or proof**.
- Light parchment with dark ink, like the books in Diablo.

## Open questions

- Tech stack (proposed in the [roadmap](roadmap.md), not confirmed).
- Content pipeline details: generator prompts, validator, pool sizes.
- Which checklist items are rules and which are judged by AI.
- Confirming the Google data against official sources.
- Path 2: Ramp SWE Intern (researched, not designed).
- Classes as career tracks (SWE, data, AI/ML).
- Logging real interviews to correct the estimated weights.
- Original boss names and art.
