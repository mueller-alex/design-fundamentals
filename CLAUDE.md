# Design Fundamentals — Authoring Rules

## Learner profile
Expert practitioner: 11 yrs visual design, 8 yrs UX, Digital Media & Design degree. Can produce good
interfaces by instinct. The gap is explicit vocabulary and reasoning — the *why* behind choices already
made correctly. Do not teach UI mechanics or visual craft. Teach the language and the thinking.

## Lesson design
- Lead with interactive wrong-way / right-way comparisons. The UI demonstrates the flaw; prose never
  telegraphs it. Neutral task prompts ("Make the screen brighter"), not descriptions of the bug.
- Default difficulty: edge cases and contested judgment calls, not recognition-level exercises.
  Multiple answers must be defensible; reasoning is what's graded, not the label.
- Never put give-away descriptions under graded answer options. Hints go in post-answer feedback only.
- Every lesson ends with a "Strengthen the muscle" section: explicit protocol → guided walk-through →
  real-world field mission. Save the protocol as a print-friendly reference card in /reference.
- Aim for 3–5+ screens of content, chunked into active widgets — length from doing, not reading.

## Prose voice
*(From learning-record 0006)*

**Avoid these patterns:**
- Reversal clichés: "X isn't Y — it's Z", "not X. Just Z", "it's not X, it's Y", "X, not just Y".
  State claims positively and directly.
- Punchy fragment endorsements: "that's the move", "the upgrade", "the muscle", "the senior move".
- Manufactured stakes: "how users lose data and trust", "win the critique", "you'll apply forever".
- Em-dash drama. Prefer periods and colons. One em-dash per paragraph at most.
- Intensifiers and self-praise: viscerally, sharp/sharper, crisp, genuinely, literally, exactly,
  precisely, "the whole point".
- Meta-commentary about the lesson itself: "here's the trap", "the goal of this section".

**Keep:**
- Real Norman/Nielsen quotes and citations — they earn the authority.
- Plain, confident statements that let examples carry the weight.
- Target voice: knowledgeable colleague at a whiteboard, not a landing page.

## Typography & CSS
- Fonts: **Gambarino** (`var(--serif)`) for headlines, **Switzer** (`var(--ui)`) for body and UI.
  Import via Fontshare: `https://api.fontshare.com/v2/css?f[]=switzer@...&f[]=gambarino@400`
- **No `text-transform: uppercase`** anywhere — labels, captions, kickers, table headers, section
  heads. Sentence case throughout.
- All shared styles live in `lessons/lesson.css`. Never inline styles that belong there.
- Dark page chrome, light UI example canvas — do not invert this.
