---
name: project-planning-docs
version: 1.0.0
description: Scopes a software or game development project through a short interactive Q&A and then drafts a full suite of pre-planning documents (vision/concept, PRD or GDD, technical design, project plan, user stories, art bible, test plan, risk register). Use this skill whenever the user wants to plan, scope, or kick off a software OR game project, asks "what documents do I need" for a dev project, mentions a PRD, GDD, game design document, product requirements, project pre-planning, or wants help briefing a development team. Trigger even if the user only describes an app/game idea and asks how to get started — they likely need this planning workflow.
---

# Project Planning Docs

This skill turns a fuzzy project idea into a complete, ready-to-share set of pre-planning documents. It works for both **software** projects (apps, web tools, SaaS, internal tools, APIs) and **game development** projects.

The flow is always: **(1) figure out the project type → (2) run a short interactive intake → (3) draft the full document suite → (4) present the files and offer a Word export.**

The user of this skill is often non-technical or semi-technical (e.g. a marketer, founder, or producer scoping work to brief a dev team). Explain choices in plain language and avoid unexplained jargon.

---

## Step 1 — Determine the project type

If the conversation hasn't already made it obvious, ask which track to use with a single tappable question via the interactive-question tool (`ask_user_input_v0`):

> "Is this a software project or a game?"
> Options: `Software (app / web / platform)` · `Game`

Once known, pick the matching document suite:
- **Software** → read `references/software-suite.md`
- **Game** → read `references/game-suite.md`

Read the relevant reference file now — it defines exactly which documents to produce and the section structure for each. Do not draft from memory; the reference files are authoritative for structure.

## Step 2 — Run the interactive intake

Gather what's needed to draft the documents for real (not generic filler). Combine two input styles:

1. **One free-text ask in the chat** for things that can't be multiple-choice:
   > "In a few sentences, tell me: what is this project, who's it for, and what's the single most important thing it needs to do?"

2. **Tappable questions** (`ask_user_input_v0`) for the structured choices. Ask in rounds of up to 3 questions. Use the question sets in the relevant reference file. The common ones (both tracks) are: target platform, team size, timeline horizon, and development methodology.

Keep it tight — aim for the free-text ask plus 1–2 rounds of tappable questions, not an interrogation. If the user says "just assume sensible defaults," stop asking and proceed, stating the assumptions you made.

**Methodology helper:** if the user picks "Not sure" for methodology, default to Agile/Scrum for most projects and briefly say why (iterative, good when requirements will evolve), reserving Waterfall for fixed-scope, fixed-deadline work.

## Step 3 — Draft the full document suite

Produce **every document** listed in the relevant reference file, each as its own Markdown (`.md`) file saved to `/mnt/user-data/outputs/`. Use clear filenames like `01-vision-concept.md`, `02-prd.md`, etc., numbered in the order a team would create them.

Drafting rules:
- Fill documents with **specific, plausible content** derived from the intake answers — real feature names, real user types, a real-looking milestone schedule. The point of "fully drafted" is that the user can edit rather than start from scratch.
- Where a detail genuinely wasn't provided, insert a clearly marked placeholder like `[TODO: confirm budget]` rather than inventing something risky (e.g. exact costs, legal commitments).
- Things that are inherently visual (wireframes, concept art, UI mockups) can't be drawn as text — describe what's needed and add a placeholder note pointing to where they'll go.
- Keep each document scannable: short intro, then clear headings. Follow the section structure in the reference file.
- Carry the same project name, audience, and scope consistently across all documents.

## Step 4 — Present and offer Word export

Use the `present_files` tool to show all the drafted files, leading with the vision/concept document. Give a one-line summary of what's in the set.

Then offer, in one short line, to convert any or all of them into Word (`.docx`) documents for sharing with stakeholders. Only do the conversion if the user says yes — if they do, follow the `docx` skill.

---

## Output format reminder

ALWAYS produce real saved files (not just inline text) for the documents, since the whole value is a deliverable the user can hand off. The numbered `.md` files in `/mnt/user-data/outputs/` are the deliverable; the chat is just narration around them.
