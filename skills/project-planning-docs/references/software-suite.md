# Software Project — Document Suite

Produce all of the following, each as its own numbered `.md` file. They're ordered the way a team would naturally create them (why → what → how → when → verify).

## Intake questions (tappable, software track)

Ask these via `ask_user_input_v0` (rounds of ≤3), alongside the free-text project description.

**Round 1**
1. Product type — `Web app` · `Mobile app` · `SaaS platform` · `Internal tool` · `API / backend`
2. Target platform — `Web` · `Mobile (iOS/Android)` · `Desktop` · `Cross-platform`
3. Team size — `Solo` · `Small (2–5)` · `Medium (6–15)` · `Large (15+)`

**Round 2**
1. Timeline horizon — `Under 3 months` · `3–6 months` · `6–12 months` · `12+ months`
2. Development methodology — `Agile / Scrum` · `Kanban` · `Waterfall` · `Not sure`
3. Build approach — `MVP first, then expand` · `Full build` · `Not sure`

---

## The documents

### 01 — Vision / Concept Document
The highest-level "what and why." Sections: Overview (one paragraph), Problem statement, Target users, Proposed solution, Key goals & success metrics, Why now / why us, Out of scope.

### 02 — Product Requirements Document (PRD)
What the product must do, not how. Sections: Summary, Objectives & success metrics, User personas, Functional requirements (numbered, grouped by feature area), Non-functional requirements (performance, security, accessibility), Assumptions & constraints, In scope vs. out of scope, Open questions.

### 03 — Technical Design / Architecture Document
The how, for engineers. Sections: Overview, Proposed tech stack (with brief rationale), System architecture (describe components and how they connect; include a simple text/ASCII or described diagram), Data model / key entities, External integrations & APIs, Security & privacy considerations, Scalability notes, Key technical risks. Mark deep technical specifics the team must confirm as `[TODO]`.

### 04 — Project Plan / Roadmap
Timeline meets reality. Sections: Milestones (with a plausible phased schedule based on the timeline horizon — e.g. Discovery, MVP, Beta, Launch), Phase breakdown with rough durations, Team & roles, Dependencies, Key dates. Present the schedule as a table.

### 05 — User Stories / Backlog
Features from the user's perspective. Produce a prioritized list in the form: "As a [user], I want [goal] so that [benefit]," grouped by epic/feature area, with a simple priority tag (Must / Should / Could). Aim for a starter backlog of 15–25 stories covering the core gameplan.

### 06 — Test / QA Plan
How you'll verify it works. Sections: Testing approach (unit, integration, manual, UAT), What gets tested, Test environments, Entry/exit criteria for release, Bug triage & severity levels.

### 07 — Risk Register
What could go wrong and the backup plan. A table with columns: Risk · Likelihood · Impact · Mitigation · Owner. Populate with realistic risks for this project type (e.g. scope creep, key-person dependency, integration delays, adoption risk).

---

## Note on visuals
Wireframes and UI mockups belong with the PRD but can't be drawn as text. In the PRD, add a "Wireframes" section with a placeholder describing the key screens to be sketched and where the visuals will live (e.g. Figma).
