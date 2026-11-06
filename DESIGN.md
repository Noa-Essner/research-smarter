# Research Smarter — Design

## Motivation

In 2024, the American Psychological Association said in [an article](https://www.apa.org/topics/artificial-intelligence-machine-learning/ai-research-writing) that, when it comes to research, "Ideally, AI tools will progress to the point that they can enable researchers to focus on the more complex and cognitively demanding elements of scholarship."

Research Smarter is a research assistant skill that works with the user to refine their research topic, stress-test their arguments, and do the mental work of engaging with the research process. The goal is for the skill to develop the user's critical thinking skills as AI becomes more prevalent as a research tool.

## Guiding Principles

- **The user does the thinking.** The skill is a tool for getting the user to
  do the critical thinking themselves. When it offers options (angles,
  framings, avenues to explore), the user chooses and must justify the choice.
  The skill never offers conclusions.
- **The user does all the writing.** The skill never writes anything for the
  user's work: not the research question, not a thesis, not a paragraph. All
  of it has to come from the user. The skill's own output (briefings, source
  summaries, questions) is there to inform the user, not to be copied into
  their work.
- **Facts are corrected; reasoning is questioned.** When the user gets a fact
  wrong, the skill tells them directly and shows the correct information. When
  the issue is conceptual (reasoning, interpretation, assumptions), the skill
  doesn't say the user is wrong. It asks probing questions that lead the user
  to examine their own thinking.
- **Honest pushback, not contrarianism.** The skill is neither a cheerleader
  nor a contrarian. It pushes back on points that are poorly reasoned,
  unsupported, or rely on logical fallacies. When an argument is well
  supported, it says so and names what makes it strong, then moves on to probe
  the next weakest point.
- **Verify what the AI says.** At the start of the session, the skill reminds
  the user that AI models can sometimes hallucinate and encourages them to do
  their own research and fact-check what the model produces. After that, it
  flags accuracy where it matters, next to specific claims and citations.

## Research Types

The skill works for any kind of research. The phases stay the same; what
changes is the central thing being tested (the user's "working position") and
the lens the skill uses to challenge it in Phases 2 and 5. Phase 0 identifies
the type.

| Research type | Working position | What Phases 2 and 5 challenge |
|---|---|---|
| Argumentative essay | Thesis | Counterarguments, logical fallacies |
| Empirical study | Hypothesis | Other explanations, confounding factors, whether it can be disproved, sample size and method |
| Literature review | How the review organizes the field | What's left out, which voices dominate, whether the gaps are real |
| Historical or interpretive | Interpretation | Other readings, bias in the sources, anachronism |
| Exploratory, no position yet | The question itself | Assumptions built into the question, scope, whether it can be answered |

New types can be added as new rows.

## Moving Between Phases

- **Progress marker.** Each response opens with a short header showing where
  the user is, for example "Phase 2 of 5: pre-research stress test."
- **Exit checks.** Each phase ends with a quick check the user completes in
  their own words, for example "State your research question in one sentence"
  (Phase 1) or "Name the strongest counterargument and your response to it"
  (Phase 2). The skill can recommend staying longer, but the user decides when
  to move on.
- **Going back.** The user can return to an earlier phase at any time. If
  findings undercut the research question, the skill suggests going back and
  treats that as a normal part of research.
- **Skipping ahead.** A user who arrives with a research question can start at
  Phase 2, but the skill first checks the question against the research
  question framework.
- **"Just give me the answer."** The skill holds the line firmly but kindly. It
  briefly explains why, then offers the smallest next step (for example, "Just
  tell me which of these two angles interests you more"). It can speed up the
  process, such as by moving to Phase 4 sooner, but it never writes the user's
  content.

## Phase 0: Intake

Before any research begins, the skill gathers context:

- the type of assignment or project, its length, and its deadline
- the type of research (see Research Types)
- the discipline or subject area
- any required source types and the citation style
- what the user already knows about the topic

The skill never asks for the user's age, grade, or school. It uses the
assignment details to set how challenging to be (see Tone and challenge
level).

**Outcome:** The skill has the context it needs to tailor the rest of the
process to the user.

## Phase 1: Explore and choose a direction

1. **Preliminary briefing.** The skill does some preliminary research on the
   topic and gives a quick briefing.
2. **Patterns.** It identifies patterns across existing texts and literature.
3. **Mind map.** It presents an interactive mind map of possible avenues the
   user could explore (see Output formats). The user explores, chooses a direction, and justifies why.
4. **Refining questions.** Once the user chooses a direction, the skill follows
   up with refining questions, guided by a framework for what makes a good
   research question:
   - It flags topics that are oversaturated, or angles that don't add anything
     new.
   - It suggests alternate angles to consider. The user picks among them (or
     rejects them) and explains their reasoning.

**Outcome:** The user has written a draft research question.

## Phase 2: Second briefing and pre-research stress test

1. **Targeted research.** The skill does more research on the angle the user
   picked and gives a second briefing.
2. **Back-and-forth.** The user says, based on this research, where they want
   to go and what they want their arguments to be. This stage tests the user's
   reasoning before they've gathered evidence. The skill:
   - shows what the other side might argue
   - questions the user toward logical fallacies in their arguments
   - pushes back on and helps refine the user's thinking
   - challenges assumptions and asks questions unprompted

**Outcome:** The user has a final research question and a working position,
and can name the strongest counterarguments to it.

## Phase 3: Plan the research

1. **Sub-questions.** The skill prompts the user to break their research
   question into smaller sub-questions.
2. **Where to look.** For each sub-question, the user decides where the answer
   might be found: what kinds of catalogs or platforms, possible keywords, and
   who might hold the expertise.
3. **Critical thinking moment.** The user considers what kinds of research
   could support their argument and what kinds could counter or complicate it.

The first two steps help guide the skill's research. The main purpose of this
phase, especially the last step, is to prepare the user to know what they're looking for, what's useful, and what they want to do with the research the skill will conduct in Phase 4, so the user can parse that information more strategically and take ownership of the research.

**Outcome:** The user has a research plan: sub-questions, where to look for
each, and what evidence would support or complicate their position.

## Phase 4: Research

The skill does the research and delivers:

- the relevant sources it compiled
- a summary of what it found and what it didn't find
- additional questions or fine-tuning
- suggested avenues to explore, including things the user should look into
  more on their own

The user then works with the results:

- **Sorting.** The user matches sources to the sub-questions they serve and
  judges which ones support their position and which complicate it.
- **Evaluating sources.** The user assesses the credibility of a few sources
  themselves (author, venue, methods, date, possible bias) before the skill
  shares its own assessment.
- **Reflecting.** The user compares what they found with what they expected in
  Phase 3. What's missing? What would make this research stronger? What types
  of findings might weaken it?

To close the research process, the skill encourages the user to include a
disclosure in their work describing how they used AI in the research process,
and lets them know Phase 5 is available whenever they want it.

**Outcome:** The user has a curated, annotated set of sources, mapped to their
sub-questions.

## Phase 5: Ongoing stress testing (optional)

Phase 5 isn't a required step. Once the research question is refined and the
research is done, it's a resource the user can return to whenever they want,
to keep engaging deeply with their research as they continue working.

The user doesn't need to bring in all their research. They bring in whatever
they want tested, one piece at a time, such as:

- an argument or claim they're making
- a source they're relying on
- a line of reasoning they're unsure about

The skill then stress-tests it:

- **Credibility.** For a source, the skill first asks the user for their own
  assessment (author, venue, methods, date, possible bias), then shares its
  own. It checks that the source exists and says so if it can't verify it.
- **Logical fallacies.** It questions the user toward any fallacies in their
  reasoning.
- **Evidence and perspectives.** Where Phase 2 tested the user's reasoning
  before the evidence, this phase tests their arguments against the evidence
  and against other perspectives, using the lens for their research type. For
  example: "This source seems to contradict your claim. How do you account for
  that?"
- **Critical thinking.** It asks probing questions that push the user to
  strengthen their own thinking.

**Outcome:** Whatever the user brings in has been stress-tested, and the user
leaves with questions to keep strengthening their work.

## Logistics

### Format

Research Smarter is a Claude Skill, built mainly for Claude.ai so students
don't need a terminal. Claude loads each phase's file only when the user
reaches that phase.

```
research-smarter/
  SKILL.md                  # overview, principles, phase flow
  references/
    phase-0-intake.md … phase-5-post-research.md
    research-types.md
    question-framework.md
  templates/
    research-log.md
    mind-map.html
```

### Activation

The skill runs only when the user asks for help with a research project using
the keyword "research," for example "help me research X" or "continue my
research." It does not run for casual or factual questions that happen to
mention research, such as "what does research say about coffee?" Those get a
normal answer.

### Saving and resuming

At the end of each session, the skill produces an up-to-date research log for
the user to save. The log records:

- the current phase and step, and which exit checks the user has passed
- the intake answers
- the user's research question and working position, in their own words
- sub-questions and the research plan
- sources found so far
- arguments and sources the user has stress-tested in Phase 5
- key decisions and changes of direction, and why
- what the user was in the middle of when the session ended

When the user uploads a log in a new session, the skill reads it, gives a
short recap, and asks the user to restate their current question and position
in their own words before picking up exactly where they left off.

### Sources and citations

- The skill never cites from memory. Every source must be one it actually
  found during the session, with a working link or DOI.
- It says clearly when a source couldn't be verified.
- For paywalled sources, it says it can't read the full text and works from
  the abstract. It points the user to their library or a librarian, or to a
  free open-access version if one exists.
- Web search is the baseline tool. Scholarly databases (such as OpenAlex or
  Semantic Scholar) can be added where the environment allows.

### Output formats

- **Briefings:** about 300–500 words, with sections for key debates, major
  voices, patterns, and open questions.
- **Mind map:** an interactive 3D map, built as a Claude.ai artifact.
  - The research topic sits at the center. Each branch is a possible angle,
    with smaller branches for sub-angles.
  - The user can rotate, zoom, and click through the map.
  - Clicking a branch opens a panel with a short description, a few key
    sources, how crowded the angle is, and questions to consider. The panel
    never offers conclusions.
  - Colors show saturation: warm for crowded angles, cool for under-explored
    ones.
  - The user chooses a branch and justifies the choice in the chat.
  - The skill includes a ready-made template (`templates/mind-map.html`), and
    Claude fills in only the data for each topic, so the map looks and works
    the same every time.
  - In Claude Code, the same template becomes a file the user opens in their
    browser. Where artifacts aren't available, the skill falls back to an
    indented text tree.
  - A working prototype with demo data is in `prototypes/mind-map.html`.

### Pacing

- One or two questions per turn, never a long list.
- Short turns in the back-and-forth phases. Longer responses are for
  briefings.

### Tone and challenge level

- **One tone for everyone.** The default tone is challenging but encouraging,
  and it stays the same for every user.
- **Challenge level follows the assignment.** The skill never asks for the
  user's age, grade, or school. Instead, it sets how hard to push based on the
  assignment details from intake: the type of research, its length, the
  source requirements, and the discipline. For example, a short opinion piece
  gets lighter pushback than a long empirical study or a thesis.

### Privacy

Many users may be minors. The skill asks only for what intake needs and never
for names, ages, grades, schools, or other personal details.

### Test cases

Scenarios the skill must handle correctly:

- The user asks the skill to write their thesis.
- The user states a false fact.
- The user makes a genuinely strong argument. Does the skill acknowledge it?
- The user wants to skip straight to Phase 4.
- A citation can't be verified.
- The user uploads a research log and resumes mid-phase.
- The user returns days later with a single source to stress-test in Phase 5.

## Example Walkthrough

This walkthrough follows one student, Sam, through every phase. The exchanges
are shortened to show how the skill behaves, not every turn of the
conversation. The sources described are placeholders, not real citations.

### Starting the skill

> **Sam:** I need to research social media and teen mental health for my
> sociology class.

The keyword "research" and a research project activate the skill. It opens
with a short reminder that AI can make mistakes and that Sam should fact-check
what it produces.

### Phase 0: Intake

The skill asks a few questions, one or two at a time. Sam explains that it's
an 8-page argumentative essay for a sociology class, due in
four weeks, requiring at least five peer-reviewed sources in APA style. Sam
has read a few news articles but nothing academic.

**Exit check:** the skill confirms it has the context it needs, and the
research type is set to argumentative essay, so the working position will be
a thesis. Because it's an 8-page paper requiring peer-reviewed sources, the skill
sets a fairly demanding challenge level, without ever asking Sam's age or
school.

### Phase 1: Explore and choose a direction

The skill gives a short briefing: this is a heavily studied topic, most
research asks whether social media harms teens, and the public debate is
heated. It points out patterns, such as many studies relying on teens'
estimates of their own screen time.

It then opens the interactive mind map. Sam rotates it and clicks through the
branches. The main "does social media cause depression?" branch is red,
meaning crowded. "School phone bans" is green, meaning moderately explored,
and its narrower branches are cooler still.

> **Sam:** I want to do school phone bans. My school just started one.
>
> **Skill:** What makes that more than a personal connection? Why might phone
> bans be worth researching right now?
>
> **Sam:** Because lots of schools are trying them, but there isn't much
> research yet on whether they work.

The skill flags that "Do phone bans work?" is too broad to answer in 8 pages,
and asks what "work" would mean. Sam settles on social life, rather than
grades, because that branch was less explored.

**Exit check:** Sam states the draft question in one sentence, in their own
words: "How have school-day phone bans changed how high school students
interact with each other in person?"

### Phase 2: Pre-research stress test

The skill researches phone bans and social life more deeply and gives a second
briefing. Sam starts forming a position.

> **Sam:** Phone bans started after COVID, when everyone realized how addicted
> kids were.
>
> **Skill:** That part isn't accurate. France passed a law restricting phones
> in primary and middle schools in 2018, before the pandemic. How might a
> longer history of bans be useful to your project?

That's a factual error, so the skill corrects it directly. When Sam makes a
conceptual claim, the skill asks questions instead:

> **Sam:** Bans obviously improve social life. At my school, people talk at
> lunch now.
>
> **Skill:** What else might have changed at your school at the same time? And
> how would you know whether what you're seeing at one school is true at
> others?

Later, Sam points out that some studies look at the same schools before and
after a ban. The skill acknowledges that this is a strong point and explains
why, then moves on to a weaker one: whether "talking more at lunch" is the
same thing as better social life.

**Exit check:** Sam writes a working thesis and names the strongest
counterargument: bans may just move social conflict to after school instead of
reducing it.

### Phase 3: Plan the research

> **Sam:** Can you just write my sub-questions? I'm short on time.
>
> **Skill:** I can't write them for you, because they need to come from your
> thinking. But let's make it quick: what's one thing you'd need to know
> before you could answer your main question?

Sam writes three sub-questions, then decides for each where to look: education
research databases, school district reports, and interviews or surveys of
students. Sam also lists what would support the thesis (before-and-after
studies showing more in-person interaction) and what would complicate it
(evidence that conflict moved online after school).

**Exit check:** Sam has a research plan, with sub-questions, where to look,
and what would support or complicate the thesis.

### Phase 4: Research

The skill searches and delivers the sources it found, with working links, a
summary of what it found and didn't find (for example, almost no long-term
studies yet), and suggestions for what Sam should look into further,
including asking a librarian about two paywalled journals.

Sam then sorts the sources by sub-question, evaluates the credibility of two
of them before seeing the skill's assessment, and reflects: what's missing,
what would make the research stronger, and what types of findings might
weaken it.

To close, the skill encourages Sam to include a disclosure describing how AI
was used in the research process, and mentions that Phase 5 is available
whenever Sam wants it. Sam saves the research log.

### Phase 5: Ongoing stress testing (optional)

A week later, while writing, Sam uploads the research log and one new source:
a news article reporting a school district survey.

> **Skill:** Welcome back. Last time you finished your research plan and
> sorted your sources. Before we start, can you restate your thesis in your
> own words?

Sam restates it. The skill asks for Sam's own read of the article's
credibility first, then shares its own: the article reports a survey but
doesn't say how many students responded or how they were chosen. It asks how
much weight Sam's argument should place on it, and what Sam would need to
find to rely on it.

Sam leaves with a stronger sense of which evidence can carry the argument, and
with every word of the essay still Sam's own.
