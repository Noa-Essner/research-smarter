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

## What I want to make possible, and why it matters

Right now, the easiest way for a student to use AI for a research paper is to
ask it for the answer: the topic, the thesis, the sources, sometimes the
paper. AI models can easily write full research papers, or do deep--dives to pull up detailed information and sources in minutes.  That saves time, but it skips the part of research that engages the student intellectually. If "research" as a skill no longer means being able to find good sources, then I want to build a Claude skill that redefines what it means to do research in the age of AI. 

I want students (high school, college, or anyone doing a research project)
to get AI's real advantage, which is fast searching and summarizing, while
they still choose the direction, form a position, weigh the evidence, and
write every word. Success isn't a finished paper -- it's a student who thinks
more sharply about their topic than when they started and can say every idea
in their work is their own. 

It's so easy to be passive and let AI do the thinking for you. AI can also easily feed confirmation bias. I'm passionate about students using AI as a tool to sharpen their thinking, not as a weapon to erode it. 

## What makes it a stretch

The skill has to be genuinely helpful while refusing to do the thing students
most often ask for: doing the work for them. It has to hold that line when a student pushes back ("my
teacher said it's fine," "just give me an example"), correct false facts
directly but only question reasoning, and push back honestly without being
contrarian. It also has to work for any kind of research, from an
argumentative essay to a lab report or a literature review, scale its
challenge to the assignment, never invent a source, and pick up a project
days later from a saved log.

## What AI enables, and what I bring

AI can search, summarize, and coach in real time, which used to take a
teacher or librarian sitting next to each student. It can also build an
interactive 3D mind map of possible angles on a topic. What I bring is the human discernment to decide what makes a good research tool, and when an AI model is being to agreeable or too contrarian. I also plan to add my own research frameworks/processes to guide how the skill is designed. 
I made the design decisions: what the AI may and may not do, the six phases and
their exit checks, and how hard it should push.

## Approach and early test

I built the skill as a Claude skill with six phases: intake, explore and
choose a direction, a pre-research stress test, planning, research, and
optional ongoing stress testing. My early tests ran the same prompts with and
without the skill, starting from realistic points in a project.

## What success looks like

Success means the skill does what a good research coach would, observably:

- it never writes the student's question, thesis, or any of their text,
  including examples and fill-in-the-blank templates;
- it corrects factual errors with a source, then asks how the correction
  affects the student's question;
- it only cites sources it actually opened.

`SPEC.md` lists 37 testable requirements like these.

- **Comparison:** the same prompts with no skill. So far, across ten test
  cases, the skill passed 68 of 68 checks and plain Claude passed 31 of 68.
  Without the skill, Claude wrote research questions and a sample thesis,
  skipped the student's planning, and listed sources from memory.
- **Cases that could expose a weakness:** a student claiming their teacher
  allows it, no web search available, and a request to skip planning. One
  real weakness has already shown up. Saying "I want to research matcha" in
  Cowork didn't activate the skill.

## Questions I want to discuss

- **Measuring thinking.** How can I test whether students actually think
  better, not just whether the skill follows its rules?
- **Testing whole conversations.** My tests check single replies. What's the
  best way to test a full multi-turn project, or to run a trial with a real
  student?
- **Activation.** How can I make the skill come up reliably in Cowork when
  someone says they want to research something?
- **Timing.** I built and tested a first version before this consult. How
  should that fit the course's plan-then-build process?
- **Sharing.** Can I keep a public copy so other students can install the
  skill?

---

Details: [GUIDE.md](GUIDE.md) (how it works, installing, using it) ·
[SPEC.md](SPEC.md) (requirements and test results) ·
[DESIGN.md](DESIGN.md) (full design and an example walkthrough)
