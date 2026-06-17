# Feedback: example devices must vary across sections — the quiz must not mirror the audit

Lesson 03 (Constraints & Conceptual Models) shipped a first draft where the §11 "retrieve it"
quiz reused the §09 audit's two gimmicks: a free-text field that accepts garbage (classified as a
"constraint" failure) and a button that does more than its label says (a "model" failure). One quiz
widget was the audit's bounded stepper duplicated as the "nothing wrong" case. The learner flagged the
examples as "quite bad, especially since they mirror the audit section," and asked for them to be
improved immensely.

**Why it matters:** repeating one or two UI archetypes across a lesson collapses the variety that makes
retrieval hard. If every "constraint" example is "free text eats bad input" and every "model" example is
"button does extra," the learner pattern-matches the *device*, not the *concept* — recognition, not
transfer. For an expert who reads fast, that is the difference between practice and filler. Distinct
devices force the reasoning to generalise.

**How to apply to every lesson from now on:**
- **Keep a device ledger.** List the concrete UI archetype each interactive widget uses (free-text
  field, bounded stepper, destructive button, two-field form, toolbar mode, date pickers, masked input,
  modal, and so on). No archetype should appear in two sections. The audit and the quiz especially must
  not share devices.
- **Cover the full taxonomy with different mechanisms.** For an N-way classification, demonstrate each
  class through a *different* failure mechanism. Constraints alone span: a missing logical constraint
  *between fields* (a budget that allows $120 against $100), an over-constraint that blocks a valid
  action (a paste-blocked, length-capped password), a semantic mismatch (a trash-can icon on an Export
  action), physical bounds. Reach past the one obvious gimmick.
- **Use edge cases that overturn the simple rule** (per [[0003-advanced-level-raise-difficulty]]):
  over-constraint where the fix is to *remove* a constraint; mode errors; optimistic feedback that lies
  about system state (a "Saved ✓" that never synced — a model mismatch, and a callback to a prior lesson).
- **Make the "nothing wrong" case an honest *working* instance of the mechanism, not inert text.** An
  auto-formatting card field that strips letters and groups digits is a far better distractor than a
  static label, because it actively manipulates input and tempts a false flag.
- A widget that is interactive but recycled is worse than no widget. Device variety is part of
  [[0005-ui-demonstrates-not-prose]], not separate from it.

See `lessons/0003-constraints-and-conceptual-models.html` §09 (audit) and §11 (retrieve it) as the
corrected template: six audit items and six quiz widgets, twelve distinct devices, zero overlap.
