# claude-skills

A collection of **skills** for [Claude](https://claude.ai) — self-contained instruction packs that teach Claude how to carry out a specific, repeatable job well.

A skill is just a folder with a `SKILL.md` file (the instructions) plus any supporting reference files. When the skill is available to Claude, Claude reads it and follows it whenever your request matches what the skill is for. You don't call it manually — it triggers on the kind of task it was built for.

## What's in here

| Skill | What it does |
|-------|--------------|
| [`project-planning-docs`](#project-planning-docs) | Turns a rough project idea into a full set of pre-planning documents for a software **or** game project. |

Skills are stored as zip archives in the repo root (e.g. `project-planning-docs.zip`) so they're easy to download and drop into Claude.

## project-planning-docs

Give Claude a fuzzy idea for an app or a game, and this skill walks you through a short Q&A, then drafts a complete, ready-to-share set of planning documents you can hand to a development team.

It's built for non-technical and semi-technical people (founders, marketers, producers) scoping work — so it explains choices in plain language instead of jargon.

**How it works:**

1. **Figures out the project type** — software (app / web / SaaS / internal tool / API) or a game.
2. **Runs a short interactive intake** — a few tappable questions plus one free-text description, so the documents are specific to *your* project rather than generic filler.
3. **Drafts the full document suite** — each as its own numbered Markdown file.
4. **Presents the files** and offers to export them to Word (`.docx`) for sharing with stakeholders.

**Documents it produces:**

*Software track:* Vision/Concept · Product Requirements (PRD) · Technical Design/Architecture · Project Plan/Roadmap · User Stories/Backlog · Test/QA Plan · Risk Register

*Game track:* Game Concept/Pitch · Game Design Document (GDD) · Technical Design · Art Bible/Style Guide · Project Plan/Roadmap · Test/QA Plan · Risk Register

**What's inside the package:**

```
project-planning-docs/
├── SKILL.md                       # the instructions Claude follows
└── references/
    ├── software-suite.md          # document structure for software projects
    └── game-suite.md              # document structure for game projects
```

## Using a skill

1. Download the skill's `.zip` from this repo.
2. Add it to Claude wherever skills are supported (for example, upload it in the Claude app, or place the unzipped folder in your Claude Code skills directory).
3. Just describe your task in plain English — Claude picks up the skill automatically when your request matches what it's for. For `project-planning-docs`, that's anything like *"help me plan my app idea"* or *"what documents do I need to brief a dev team?"*

## License

No license file is included, so all rights are reserved by default. Add a `LICENSE` file if you intend to let others reuse this.
