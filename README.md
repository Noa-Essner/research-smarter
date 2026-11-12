# Research Smarter

In 2024, the American Psychological Association said in
[an article](https://www.apa.org/topics/artificial-intelligence-machine-learning/ai-research-writing)
that, when it comes to research, "Ideally, AI tools will progress to the
point that they can enable researchers to focus on the more complex and
cognitively demanding elements of scholarship."

Research Smarter is a research assistant skill that works with the user to
refine their research topic, stress-test their arguments, and do the mental
work of engaging with the research process. The goal is for the skill to
develop the user's critical thinking skills as AI becomes more prevalent as
a research tool.

## How it works

A project moves through six phases. Each one ends with a short exit check
you answer in your own words. You can go back to an earlier phase at any
time, and you decide when to move on.

| Phase | What happens |
|---|---|
| 0. Intake | Claude learns about the assignment (type, length, deadline, source rules) and sets the research type |
| 1. Explore and choose a direction | A briefing on the topic plus an interactive 3D mind map of possible angles; you write a draft research question |
| 2. Pre-research stress test | A second, focused briefing, then Claude challenges your working position: counterarguments, assumptions, gaps in logic |
| 3. Plan the research | You write sub-questions, decide where to look, and name what would support or complicate your position |
| 4. Research | Claude searches and summarizes sources; you sort, evaluate, and reflect on them |
| 5. Ongoing stress testing (optional) | Bring one argument or source at a time to test it while you write |

## What makes it different

- **You do all the writing.** Claude won't write your research question,
  your thesis, a topic sentence, or even a suggested phrasing. If you ask, it
  will explain why and help you take the smallest next step yourself.
- **Facts are corrected; reasoning is questioned.** If you state something
  factually wrong, Claude tells you and gives the correct information with a
  source. If the issue is an interpretation or a leap in logic, it asks
  questions that lead you to find the problem yourself.
- **Honest pushback, not contrarianism.** Claude pushes back on weak or
  fallacious reasoning, and says so when an argument is genuinely strong.
- **No invented sources.** Every source is one Claude actually found and
  opened during the session, with a working link. If it can't verify
  something, it says so.
- **Works for any kind of research.** Argumentative essays, empirical
  studies, literature reviews, historical or interpretive work, and
  exploratory projects each get a lens suited to what's being tested.
- **Challenge scales with the assignment, not the person.** A short opinion
  piece gets lighter pushback than a thesis. Claude never asks your age,
  grade, school, or name.
- **Pick up where you left off.** At the end of a session Claude gives you a
  research log. Upload it next time and it continues from the exact step you
  stopped at.
- **AI disclosure.** At the end of the research phase, Claude encourages you
  to write a short note in your work describing how you used AI.

## Installing

**Claude app (claude.ai or desktop):** zip the `research-smarter/` folder
(or use a packaged `research-smarter.skill` file) and upload it in Claude's
settings under Skills. Skills need code execution to be turned on.

To build the package from this repo, leaving out the test cases:

```bash
zip -r research-smarter.skill research-smarter -x "research-smarter/evals/*" "*.DS_Store"
```

**Claude Code:** copy the folder into your skills directory.

```bash
cp -r research-smarter ~/.claude/skills/
```

## Using it

Say you want to research something, at any stage, for school or your own
curiosity. A topic alone is enough. For example:

- "I want to research coffee"
- "Help me research four-day school weeks for my AP Seminar project"
- "I'm starting research for my senior thesis and don't know where to begin"
- "Found a source for my research paper, can you help me look at it?"
- "Continue my research" (and attach your research log)

If you just want an answer, such as "what does research say about
intermittent fasting?", Claude answers normally instead.

Searching for sources needs web search turned on. Without it, Claude says
so and focuses on the thinking phases, pointing you to where to search.

## Repository layout

```
research-smarter/          the skill itself
├── SKILL.md               core principles, phase overview, every-turn rules
├── references/            one file per phase, plus sources, research types,
│                          question framework, and mind map instructions
├── templates/             research log and the 3D mind map page
└── evals/                 test cases with grading criteria
DESIGN.md                  the full design document, with an example walkthrough
SPEC.md                    testable requirements, acceptance criteria, known issues
prototypes/                standalone mind map demo and walkthrough page
```

Open `prototypes/walkthrough.html` in a browser to see a full example
project (Sam researching school phone bans), with the mind map embedded.

## Status

- The skill has ten test cases in `research-smarter/evals/`. In the latest
  run it passed all 48 checks in the seven newest cases, against 24 of 48
  without the skill; the first three cases passed all 20 of theirs. Each case
  has been run once so far. `SPEC.md` lists which requirements are tested and
  which aren't yet.
- The research question framework in
  `research-smarter/references/question-framework.md` is provisional and
  will be replaced with frameworks tracked as GitHub issues.
