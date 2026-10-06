# Roadmap

One phase at a time. The first version is deliberately small: **Floor III (Arrays)
working for real, for one player.** Everything else comes after.

## Proposed stack (not confirmed yet)

| Part | Proposal |
|---|---|
| Frontend | React + TypeScript + Vite |
| Backend | Python + FastAPI |
| Database | PostgreSQL, with Docker for local development |
| Running code | Pyodide (Python in the browser via WebAssembly) |
| AI | Anthropic API (Claude), to generate problems and judge text checks |
| Speech to text | The browser's Web Speech API in v1 |
| CI | GitHub Actions |
| Deploy | Frontend on Vercel, API on Render, database on Neon |

Known limit of Pyodide: hidden tests live in the browser, so a curious player could
peek. That's fine for personal use. Before opening to other people, bosses move to the
server (phase 10).

## Phases

| Phase | What | Done when |
|---|---|---|
| 0. Groundwork | Name check, license, IP rules, API keys with a spending limit | License added and IP rules written |
| 1. Repo foundation | Folders (`apps/web`, `apps/api`, `content/`, `tools/`, `docs/`), Docker, linting, tests, CI | The first pull request shows green checks |
| 2. Data model | ERD, migrations, seed with the Google path, readiness calculation with tests | Tests pass with the values in the design |
| 3. Content pipeline (Floor III) | Problem format, generator, validator, approval tool, learning pages and quizzes | Floor III pool approved: 5+ step problems, 20+ boss problems |
| 4. API | Heroes, dungeons, attempts, progress and every rule of play | Tests cover each rule |
| 5. Frontend | Prototype screens in React, the dev scroll, code running in the browser | A correct solution wins, a wrong one shows the failing input |
| 6. Version 1 | Floor III end to end, played for two weeks, then adjusted | Floor III is worth recommending to a friend |
| 7. Text checks and voice | Rules plus AI judge, speech to text, follow-up questions | Floor XVII works |
| 8. The rest of Google | Content for every floor, the final boss | Google path playable start to finish |
| 9. Deploy | Staging, automatic deploys, production with backups and spending alerts | Stable public URL |
| 10. Opening up | Accounts, server-side bosses, privacy policy and terms, then new paths | Safe for other people's data |
