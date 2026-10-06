# Path 1: Google SWE Intern

*Not affiliated with Google.* Built from public candidate reports and Google's
published hiring attributes. Every requirement has a trust label.

## The real process

| Stage | What happens | Trust |
|---|---|---|
| Application | Resume plus basic info. Must be enrolled in a BS/MS. Applications usually open around August to September | Official |
| Online assessment | 60 to 90 min, 1 to 2 coding problems (easy to medium), plus a work-style questionnaire. A referral may skip it | Reported |
| Technical interviews | Two rounds, 45 to 60 min each. One problem per round, then improve it. Plain shared doc, no autocomplete | Reported |
| Team match | Calls with host managers. Resume-based and behavioral questions | Reported |
| What's graded | General cognitive ability, role-related knowledge, leadership, "Googleyness" | Official (published around 2014–2015) |

No system design for interns.

## Zones and floors

| Zone | Floors | Weight |
|---|---|---|
| The cathedral (gates) | I Application and resume · II Coding foundations | 15% |
| The catacombs (DSA basics) | III Arrays and strings · IV Hash maps · V Two pointers and sliding window · VI Stacks and queues · VII Linked lists · VIII Binary search | 22.5% |
| The caves (DSA advanced) | IX Recursion and backtracking · X Trees · XI Heaps · XII Graphs · XIII Intervals · XIV Dynamic programming | 22.5% |
| The abyss (the interview) | XV Technical communication · XVI Online assessment · XVII Team match · XVIII The full loop | 40% |

All weights are **Estimated**. Each DSA floor is worth 3.75%. Prerequisites: Trees needs
Recursion; Heaps and Graphs need Trees; Dynamic programming needs Recursion.

## What each floor contains

### I. Application and resume
Write a draft → checklist pass → rewrite → **Boss:** the resume passes every item, and
you explain your main project out loud for 5 minutes without notes.

**Resume checklist**
- Eligibility (Official): enrolled in a BS/MS in CS or a related field; expected
  graduation date visible; experience in at least one general-purpose language; data
  structures or algorithms shown in coursework or projects.
- Content: bullets follow the "accomplished X, as measured by Y, by doing Z" idea; each
  project names its stack and what *you* did; only real, verifiable numbers; at least one
  project with a full cycle (idea, build, test, published or used); GitHub link with
  readable READMEs.
- Format (Reported): one page; PDF; simple single-column layout; consistent dates; no
  photo, age or full address.
- Honesty: you can talk for 5 minutes about every line; no bullet claims more than happened.

### II. Coding foundations
Learn (the Python you'll use in interviews) → Recall (8 snippets from memory) → Big-O
quiz (6 snippets) → Easy ×2 → Trace (find a bug without running the code) →
**Boss:** 3 unseen easy problems in 30 minutes, with the correct complexity for each.

### III to XIV. Data structures and algorithms
Every DSA floor follows the same run:

1. **Learn:** the pattern, when to use it, template code, common traps.
2. **Recognize:** a quiz. Five problem statements, and you name the pattern for each.
3. **Easy ×2**, running code allowed.
4. **Medium ×3**, running code allowed.
5. **Explain:** a text check on one medium you solved (approach, why it works, complexity).
6. **Boss:** one unseen medium, 45 minutes, no running code. Write your approach before
   coding. To win: hidden tests pass, the complexity is correct, and the approach came first.

Boss problems come from a separate pool that never appears in the steps.

### XV. Technical communication
Learn (6 behaviors, with good and bad transcripts) → Clarify (ask 3+ questions about a
vague problem) → Brute force first → Narrated easy → Narrated medium ×2 → Self-debug →
**Boss:** an unseen medium, narrated, no running code.

The 6 behaviors: ask clarifying questions before coding; say the brute force first;
think out loud; test by walking through an example; find your own bugs; state the final
complexity.

### XVI. Online assessment
Learn → Constraints quiz → Timed easy (30 min) → Timed medium (45 min) → Edge case hunt →
Questionnaire (learning page only, never trained or graded) → **Boss:** 2 unseen
problems in 90 minutes, sample tests can be run, both must pass 100% of hidden tests.

### XVII. Team match
Learn → Tell me about yourself → 4 STAR stories (ambiguity, collaboration or conflict,
learning something fast, stepping up) → Project deep dive → Questions for the host →
**Boss:** a mock host call with 4 random questions worded differently from the steps.
After each story, the AI asks 2 follow-up questions based on what you said.

**Checklists**
- *Tell me about yourself:* 180 to 250 words; present, then past, then why this role;
  one concrete project by name; ends with why this company and this internship.
- *Each STAR story:* situation in 1 or 2 sentences; your own task; specific actions
  written with "I", not "we"; a concrete result; one sentence on what you learned; 150 to
  300 words; tagged with the trait it proves.
- *Project deep dive:* one sentence a non-engineer understands; your part separated from
  the team's; one technical decision and why; one problem and how you solved it; what
  you'd change today.
- *Questions for the host:* at least 2, specific to the team, none a quick search answers.

### XVIII. The full loop
Two 45-minute interviews back to back, each an unseen medium in a plain doc, graded on
the code and on the 6 behaviors. Open at any time, with a warning listing what isn't
cleared yet.

## Sources

- Google careers, "How we hire" (to be confirmed by hand; the pages load with JavaScript).
- World Economic Forum (2015) and Business Insider on the attributes Google grades.
- Candidate guides and reports: Aced (formerly Exponent) Google intern guide, Glassdoor
  Google internship reviews.

Have you interviewed for this role? Open an **Interview report** issue to correct or
confirm anything here.
