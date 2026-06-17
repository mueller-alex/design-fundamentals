# Rule: .ix-head is for A/B toggles only

During L03 build, `.ix-head` was initially used on several sections as a decorative title
bar. The correct rule: `.ix-head` only appears on interactive blocks that have a genuine
Version A / Version B toggle (two states the learner flips between to compare).

**Why it matters:** using `.ix-head` as decoration adds visual chrome that implies a comparison
is available when there isn't one. The learner looks for a toggle that isn't there. Decorative
section titles belong in the prose before the `.ix` block, or as a plain `<h2>`/`<h3>`.

**When to use `.ix-head`:**
- The block has exactly two named states (e.g. "Version A" / "Version B", "Wrong" / "Right")
- Clicking the labels in `.ix-head` switches the active view inside `.ix-body`

**When not to use it:**
- The block has one state and is just titled (use a heading above the `.ix` instead)
- The block cycles through steps internally (use `.step-label` or in-widget controls)

See `lessons/0003-constraints-and-conceptual-models.html` §03 (date picker A/B) and §05
(trash / undo A/B) as correct examples. All other `.ix` blocks in that lesson have no `.ix-head`.
