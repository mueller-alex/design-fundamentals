# Feedback: the UI must DEMONSTRATE the flaw; prose must never telegraph it

In Lesson 02 the learner found the diagnostic exercises too easy because the question text *described the
failure* ("a slider that dims as you drag right"), handing over the answer. He wants the rendered UI to be
rich and interactive enough that he has to **explore it and feel what's wrong** — the example should
*demonstrate* the problem, not merely illustrate a sentence that already states it.

**Why it matters:** Describing the flaw collapses the exercise into transcription — zero diagnosis, zero
desirable difficulty. For an expert, the whole value is *noticing*. The flaw must be discovered through
interaction, the way it would be in a real product.

**How to apply to every diagnostic exercise (clinics, audits, quizzes) from now on:**
- Make the widget genuinely **interactive and functional**, with a **neutral task** ("Make the screen
  brighter", "Turn off the second setting") — NOT a description of the bug.
- The question stem stays neutral: "What's wrong here, if anything?" — never name or hint the failure.
- The failure reveals itself through use (drag right → it dims; tap → nothing happens; click ▲ → it moves
  down; hit Reset → everything vanishes with no warning). Explanation goes in POST-answer feedback only.
- In audits, separate "explore the control" from "flag it" (e.g. a small flag button per element) so the
  user can actually operate the broken control before judging it.
- Include honest "nothing wrong" cases so the answer isn't always "it's broken."

This supersedes the earlier habit of verbose scenario captions. See [[0003-advanced-level-raise-difficulty]].
