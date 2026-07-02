# Project Planning Docs

## Overview

**Project Planning Docs** turns a fuzzy project idea into a complete, ready-to-share set of pre-planning documents. Describe an app or a game in a sentence or two, answer a short round of questions, and the skill drafts the full suite of documents a team would need to start building — vision, requirements, technical design, roadmap, backlog, test plan, and risk register.

It's built for the person doing the scoping — often a founder, marketer, or producer who is briefing a development team — so it explains its choices in plain language instead of engineering jargon.

## Core Capabilities

- **Two project tracks** — a tailored document suite for **software** projects (apps, web tools, SaaS, internal tools, APIs) and a separate one for **game** projects.
- **Guided intake** — a mix of one free-text question and a few tappable multiple-choice questions, so the output reflects *your* project instead of generic filler.
- **Fully drafted documents** — each document arrives with specific, plausible content you can edit, not empty templates. Genuine unknowns are flagged as `[TODO]` rather than invented.
- **Consistent across the set** — the same project name, audience, and scope carry through every document.
- **Shareable output** — documents are saved as real Markdown files and can be exported to Word (`.docx`) for stakeholders.

## Use Cases

- **Kicking off a new app or SaaS product** and needing a PRD, roadmap, and backlog to brief engineers.
- **Pitching a game** and needing a concept doc, GDD, and art bible for a studio or collaborators.
- **Answering "what documents do I even need?"** for a development project.
- **Turning a rough idea into a hand-off package** so a dev team can estimate and start work.
- **Scoping a project as a non-engineer** and wanting the planning done in plain English.

## Key Methods

The skill always follows the same four-step flow:

1. **Determine the project type** — software or game.
2. **Run a short interactive intake** — one free-text description plus 1–2 rounds of tappable questions (platform, team size, timeline, methodology, and track-specific choices).
3. **Draft the full document suite** — every document in the matching track, each as its own numbered `.md` file.
4. **Present the files and offer a Word export** — leading with the vision/concept doc.

### Software document suite

Vision/Concept · Product Requirements (PRD) · Technical Design/Architecture · Project Plan/Roadmap · User Stories/Backlog · Test/QA Plan · Risk Register

### Game document suite

Game Concept/Pitch · Game Design Document (GDD) · Technical Design · Art Bible/Style Guide · Project Plan/Roadmap · Test/QA Plan · Risk Register

## Best Practices

**Do:**
- Give a real one- or two-sentence description of the project at the intake step — the more specific the input, the more useful the drafts.
- Treat the output as a strong first draft to edit, not a final deliverable.
- Fill in every `[TODO]` placeholder before sharing with stakeholders — especially budgets, dates, and legal commitments.

**Don't:**
- Rely on the drafted schedule, costs, or risks as fact — they're plausible starting points, not commitments.
- Skip the intake and expect tailored documents — generic input produces generic output.

## Files

```
project-planning-docs/
├── SKILL.md                       # the instructions the model follows
├── README.md                      # this file
├── QUICK_REFERENCE.md             # one-page cheat sheet
├── references/
│   ├── software-suite.md          # document structure for software projects
│   └── game-suite.md              # document structure for game projects
└── tests/
    └── quiz.md                    # self-check quiz for the skill's behavior
```

## Links

- [SKILL.md](SKILL.md) — the authoritative skill instructions
- [QUICK_REFERENCE.md](QUICK_REFERENCE.md) — condensed reference
- [Software suite structure](references/software-suite.md)
- [Game suite structure](references/game-suite.md)
