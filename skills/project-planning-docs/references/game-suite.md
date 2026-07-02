# Game Project — Document Suite

Produce all of the following, each as its own numbered `.md` file. Ordered the way a studio would create them (pitch → design → tech → look → schedule → verify).

## Intake questions (tappable, game track)

Ask these via `ask_user_input_v0` (rounds of ≤3), alongside the free-text project description.

**Round 1**
1. Genre — `Action / Adventure` · `RPG` · `Puzzle / Casual` · `Strategy / Sim` · `Other (free text)`
2. Platform — `PC` · `Console` · `Mobile` · `Web` · `Cross-platform`
3. Player mode — `Single-player` · `Multiplayer` · `Both`

**Round 2**
1. Art style — `2D / Pixel` · `2D / Stylized` · `3D / Stylized` · `3D / Realistic`
2. Monetization — `Premium (one-time)` · `Free-to-play` · `Subscription` · `Ad-supported` · `Not sure`
3. Team size — `Solo` · `Small (2–5)` · `Medium (6–15)` · `Studio (15+)`

Also ask timeline horizon and methodology (same options as the software track) if not already known.

---

## The documents

### 01 — Game Concept / Pitch Document
The hook. Sections: Elevator pitch (1–2 sentences), Genre & platform, Target audience, Core fantasy / what makes it fun, Unique selling points, Comparable titles ("it's like X meets Y"), Monetization model at a glance.

### 02 — Game Design Document (GDD)
The heart of the project — a living doc. Sections: Overview, Core gameplay loop, Mechanics & systems (movement, combat, progression, etc.), Game world / setting, Story & characters, Level / content structure, Player progression & economy, Controls / UX, Win/lose conditions, Audio direction (high level). This is the longest document — be thorough but organized.

### 03 — Technical Design Document
For engineers. Sections: Target engine & rationale (e.g. Unity, Unreal, Godot — recommend based on team size and art style if not specified), Platform/performance targets, Core systems architecture, Save system & data, Networking (only if multiplayer), Third-party tools & middleware, Key technical risks. Mark deep specifics to confirm as `[TODO]`.

### 04 — Art Bible / Style Guide
The visual and audio direction. Sections: Visual pillars / mood, Color palette & lighting direction, Character & environment style, UI/HUD style, Animation direction, Audio & music direction, Reference notes. Since art can't be drawn as text, describe the direction precisely and add `[TODO: mood board / concept art]` placeholders.

### 05 — Project Plan / Roadmap
Sections: Milestones tuned to game dev — include a **Vertical Slice** milestone (one small fully-polished slice that proves the concept) plus Prototype, Alpha, Beta, Launch. Phase breakdown with rough durations, Team & roles, Dependencies, Key dates. Present as a table.

### 06 — Test / QA Plan
Sections: Testing approach (functional, playtesting, balance, compatibility across devices), What gets tested, Playtest cadence & how feedback is captured, Bug triage & severity levels, Release/cert criteria (note console certification if relevant).

### 07 — Risk Register
A table: Risk · Likelihood · Impact · Mitigation · Owner. Populate with realistic game-dev risks (scope creep / feature bloat, fun-factor not landing in playtests, art pipeline bottlenecks, platform certification delays, monetization underperforming).

---

## Note on the MVP equivalent
Games don't ship an MVP the way software does — the equivalent is the **vertical slice**. Make sure the concept doc and roadmap both reference it as the first proof-of-concept target.
