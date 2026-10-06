# Contributing to Interview Dungeon

Thanks for wanting to help. This project is still in the design stage, so most of the
useful work right now isn't code. Here's what you can do, from most to least needed.

## 1. Share your interview experience

Paths are only as good as their data. Right now most of it comes from public candidate
reports, and the project labels it *Reported*. Real experiences make it reliable.

Open an issue with the **Interview report** template and tell us:

- The company, the role and the level (intern, new grad, junior...).
- The rounds, in order: online assessment, phone screen, technical interviews,
  behavioral, team match...
- For each round: the format (live coding, take-home, plain doc, IDE...), the
  length, and the **topics** (arrays, graphs, SQL, system design, STAR stories...).
- Whether you could run your code, and what they seemed to grade.
- When it happened (month and year), since processes change.

### Respect your NDA

Many companies ask candidates not to share interview questions. **Don't post exact
questions, problem statements or anything you agreed to keep confidential.** Formats,
lengths and topics are what the project needs, and those are usually fine to share.
If you're unsure, leave it out.

## 2. Propose a new dungeon (path)

Open a **New path** issue with:

- The role you're targeting, and why it would help others.
- What you know about its interview process, with sources: official careers pages,
  your own experience, candidate reports.
- Which skills it tests that the existing paths don't.

A path is designed in the same way as [Google SWE Intern](docs/paths/google-swe-intern.md):
zones, floors, weights and bosses. Every requirement gets a trust label:

| Label | Meaning |
|---|---|
| Official | The company says it (careers pages, job posting) |
| Reported | Candidates say it, consistently |
| Estimated | Our own judgment from the two above |

## 3. Play the prototype and give feedback

Play it at https://renilsonjr.github.io/Interview-Dungeon/prototype/ (or open
[`prototype/index.html`](prototype/index.html) locally), play through Floor III,
and open a **Feedback** issue. Useful feedback is specific: which screen, what you
expected, what happened, and whether you'd actually use it to study.

## 4. Write or translate learning pages

Each floor has learning pages with a fixed shape: when to use the pattern, the idea,
template code, a trace on real numbers, and common traps. Pages can be in English or
Brazilian Portuguese. **Code always stays in English.** Open an issue first, so two
people don't write the same page.

## 5. Code

There's no app code yet. The roadmap is in [`docs/roadmap.md`](docs/roadmap.md), and
issues labeled `good first issue` will appear once the stack is confirmed and the
build starts. Please open an issue before starting anything big.

## Rules for every contribution

- **Original content only.** Don't copy problems, statements or test cases from LeetCode,
  HackerRank or any other platform. Being *inspired by a pattern* is fine; copying text
  is not.
- **No Blizzard assets.** No Diablo names, logos, art, fonts or character names.
- **No confidential interview content** (see the NDA section above).
- **Be honest about sources.** Never present a guess as a fact. Use the trust labels.
- **Be kind.** Many people here are job hunting, which is stressful. Review the work,
  not the person.

Full details in [`docs/ip-rules.md`](docs/ip-rules.md).

## Pull requests

1. Fork the repository and create a branch from `main`.
2. Keep each pull request about one thing.
3. Explain what changed and why in the description.
4. Link the issue it closes, if there is one.
