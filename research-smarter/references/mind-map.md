# Building the mind map (Phase 1)

The mind map lets the user explore possible angles on their topic visually:
the topic sits at the center, each branch is an angle, and smaller branches
are narrower sub-angles. Colors show how crowded each angle is, from cool blue
(under-explored) to warm red (crowded).

The map's job is to help the user explore, not to steer them. Descriptions are
neutral, and each branch offers questions to consider, never conclusions or a
recommended choice.

## How to build it

Use the ready-made template in `templates/mind-map.html`. Don't redesign it:
the template handles the 3D view, rotation, zoom, colors, and the side panel,
so the map looks and works the same every time. You only supply the data.

1. Read `templates/mind-map.html`.
2. Replace the single token `__MIND_MAP_DATA__` with a JSON object in the
   format below. Change nothing else.
3. Present it:
   - **Claude.ai:** create an HTML artifact with the filled-in template.
   - **Claude Code or another environment with files:** save it as
     `mind-map.html` in the user's working folder and tell them to open it in
     their browser.
   - **No artifacts or files:** fall back to an indented text tree (see below).
4. Ask the user to explore it, then tell you which direction they want to take
   and why.

## Data format

```json
{
  "topic": "Social media and teen mental health",
  "overview": "Two or three neutral sentences describing the landscape.",
  "branches": [
    {
      "label": "School phone bans",
      "saturation": 0.4,
      "description": "One or two neutral sentences about this angle.",
      "sources": ["Short description of a kind of source or a real source you found"],
      "questions": ["A question for the user to consider"],
      "children": [
        {
          "label": "Bullying and social life",
          "saturation": 0.3,
          "description": "One sentence.",
          "questions": ["A question to consider"]
        }
      ]
    }
  ]
}
```

- **branches:** 4 to 6 angles, each with 2 or 3 children. More gets cluttered.
- **label:** short (under about 45 characters), written as a topic, not as a
  research question. Never phrase the user's question for them.
- **saturation:** a number from 0 (barely studied) to 1 (heavily studied),
  based on what your preliminary research found. Spread values honestly; don't
  bunch everything in the middle.
- **sources:** only sources you actually found (with the rules in
  `sources.md`), or general descriptions of kinds of sources ("early
  evaluations of school phone policies"). Never invent a specific citation.
- **questions:** open questions that make the user think, not hints toward a
  particular answer.
- Escape quotes properly; the result must be valid JSON.

## Text-tree fallback

```
Social media and teen mental health
├── Does social media cause teen depression? [crowded]
│   ├── Correlation vs. causation [crowded]
│   └── How big is the effect? [crowded]
├── School phone bans [moderately explored]
│   ├── Bullying and social life [under-explored]
│   └── How bans are enforced [under-explored]
└── ...
```

Below the tree, give each top-level angle its one-sentence description and
one question to consider.
