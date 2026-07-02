# Project Planning Docs — Self-Check Quiz

A short quiz to verify the skill behaves correctly. Each question lists the expected answer.

---

**1. A user says: "I have an idea for a mobile fitness app but I don't know where to start." Should this skill trigger?**

> **Yes.** The skill triggers even when the user only describes an app/game idea and asks how to get started — that's the planning workflow they need.

---

**2. What is the very first thing the skill must establish?**

> The **project type**: software or game. If it isn't already obvious from the conversation, ask with a single tappable question before doing anything else.

---

**3. Where is the authoritative structure for each document defined?**

> In the **reference files** — `references/software-suite.md` or `references/game-suite.md`. Documents must be drafted from the reference structure, not from memory.

---

**4. How should the intake be conducted?**

> One **free-text** question (what/who/most-important-thing) plus **1–2 rounds of up to 3 tappable questions**. Keep it tight — not an interrogation.

---

**5. The user says "just assume sensible defaults." What should happen?**

> Stop asking questions and proceed to drafting, **explicitly stating the assumptions** that were made.

---

**6. A required detail (e.g. budget) wasn't provided. What goes in the document?**

> A clearly marked placeholder such as `[TODO: confirm budget]` — never an invented figure, date, or legal commitment.

---

**7. The user picks "Not sure" for methodology. What's the default?**

> **Agile/Scrum** for most projects (iterative, good when requirements evolve), with a brief reason. Reserve Waterfall for fixed-scope, fixed-deadline work.

---

**8. What is the actual deliverable of this skill?**

> Real **saved `.md` files** (numbered `01-…`, `02-…`) in `/mnt/user-data/outputs/` — one per document in the suite. The chat is just narration around them.

---

**9. How are wireframes and concept art handled?**

> They can't be drawn as text, so **describe** what's needed and leave a placeholder pointing to where the visual will live (e.g. Figma).

---

**10. What's the game-development equivalent of a software MVP, and where must it appear?**

> The **vertical slice** — one small, fully-polished slice that proves the concept. Both the concept doc and the roadmap must reference it as the first proof-of-concept target.
