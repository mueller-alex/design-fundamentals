# Teaching Notes

## Learner profile
- 11 yrs visual design, 8 yrs UX-focused. Degree in Digital Media & Design.
- Expert *executor*; the gap is *design thinking* — the reasoning and vocabulary behind choices.
- Self-describes as "going with the flow," relying on empathy without explicit process.

## Stated preferences
- Wants **interactive wrong-way / right-way** comparisons in every lesson.
- Wants lessons **modelled on canonical experts** (Norman's *Design of Everyday Things*, interaction-design principles).
- Product designer — keep examples in **digital product UI**, not only physical-object examples.

## Teaching approach
- Skip beginner UI mechanics. Lead with the *concept and its reasoning*, then drill via retrieval.
- Anchor heavily to Norman's vocabulary; build a glossary and keep it consistent across lessons.
- Each lesson: one tight concept, a live wrong/right demo, a retrieval quiz, a primary source.
- Quiz answers kept equal length (word + char count) to avoid format-based cueing.

## DEPTH & LENGTH PREFERENCE (2026-06-16, important)
- **Reads very fast.** A 1.5-screen lesson does NOT sink in. Wants substantially MORE content per lesson.
- **Wants applied problem-solving**, not just explanation: "Here's a problem — how would you solve it
  knowing this fundamental?" Present broken interfaces / scenarios and have him diagnose + fix.
- Wants MORE interactive examples per lesson (multiple, not one).
- Resolution: longer lessons are fine BUT keep working memory safe by making the length *active* —
  break it into many short apply/retrieve widgets (diagnose-this, build-this, classify-this) rather
  than long passive prose. Length should come from doing, not reading.

## SHOW, DON'T DESCRIBE (2026-06-16, important)
- "Basically every example would be improved by showing the respective UI rather than just describing it."
- Every scenario in a lesson should RENDER the interface in HTML/CSS, not describe it in prose. Mockups,
  thumbnails, live mini-UIs. He's a product designer — visuals are the native medium.
- Interactive auditing of rendered screens (click elements to flag) lands well as a hard exercise.
- CRITICAL (learning-record 0005): the UI must DEMONSTRATE the flaw through interaction; never describe/
  telegraph the failure in the question text. Neutral task + neutral stem ("What's wrong, if anything?");
  the flaw is felt by using the widget; explanation only in post-answer feedback. Include honest cases.
- Provide a real textarea wherever the answer is open-ended (capstone), even if not auto-graded; autosave it.
- NO restating labels above a UI example. The lead PARAGRAPH frames each example (what it is, "as shipped",
  the task) without telegraphing the flaw — don't add an `.ix-head` that just names the topic. Reserve the
  `.ix-head` bar only for genuine controls (e.g. an A/B `.toggle`). No decorative dot in heads.

## CONSOLIDATION SECTION (2026-06-16, important)
- Wants every lesson to END with a "strengthen the muscle" exercise that makes the reasoning CONSCIOUS
  and deliberate, not instinctive. Three-part template now in use (see learning-record 0004):
  (A) explicit numbered protocol + a print-friendly reference card, (B) gated step-by-step guided
  walk-through with interleaved/mirror cases (must commit each step before the next unlocks),
  (C) real-world field mission logged in an autosaved form, brought back to chat for critique.
- The interactive "audit a rendered screen" format (§08) is the gold-standard hard exercise — reuse it.

## STYLING (2026-06-16)
- Shared stylesheet: `lessons/lesson.css`. Every lesson links it (`<link rel="stylesheet" href="lesson.css">`)
  and uses NO inline `<style>` block — edit the CSS once, all lessons update. New lessons must reuse the
  existing class names (.ix, .stage, .screen, .opts, .fb, .audwrap, .proto, .gstep, .fm, etc.).
- Fonts: **Instrument Serif** for headings (h1/h2/.lede/source h3), **Geist** for body/UI (var(--ui)).
  Loaded via @import in lesson.css.
- **Dark "page" chrome, light UI examples.** Page = dark (--bg). Rendered product UIs stay light: keep them
  inside `.stage` (light canvas) using example components (.screen/.card/.stat/.qcard/.cooktop/etc.), which
  carry literal light colors. Lesson chrome (options, feedback, inputs, matrix) uses dark tokens.
- Tokens: --brand (#7a4f2a, filled buttons, white text — works on both) vs --accent (light tan, accent
  TEXT/links/borders on dark). Status: --right/--wrong/--warn + dark *-bg tints. Don't use --accent as a
  fill or --brand as body text.
- Reference cards in /reference are intentionally LIGHT (print-friendly per skill) — leave them light.

## PROSE VOICE (2026-06-16, important — see learning-record 0006)
- Strip AI-prose tropes. No fragment endorsements ("that's the move," "the muscle," "lesson landed").
  No "X isn't Y — it's Z" reversals. No manufactured stakes. Minimal em-dashes (≤1/paragraph). Drop
  intensifiers (viscerally, sharp, crisp, genuinely, literally). Less meta-commentary about the lesson.
- Target voice: a knowledgeable colleague at a whiteboard, not a landing page. Let examples carry weight.
- Keep real Norman/Nielsen quotes and citations.

## Open questions to revisit
- Does the user want to join a community now, or work solo for a while? (Asked implicitly via RESOURCES; confirm.)
- After Norman's foundations, where next — interaction/microinteractions, or heuristics (Nielsen)?
