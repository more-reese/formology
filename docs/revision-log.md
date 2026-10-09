# Revision Log

*Hypotheses: H1 (form is the invariant), H2 (form resolved by context), H3 (context is what form is not), H4 (three conditions for form-ness), H5 (recursion), H6 (resolution is reversible), H7 (form is unprovable). See `starting-core.md` for full definitions.*

*This log merges the first pass (Oct 7–8) and the collaborator review (Oct 8). Where the collaborator found more severe failures, the entry is marked [v0.4.0].*

---

## Collaborator review revisions (v0.4.0)

### H3: DROPPED as ontological claim (was "revised" in v0.3.0)

**What changed:** "Context is not form" is false. Every context formology names is itself a form by H4's own test — the key signature occupies a slot, stands in for something recoverable, and means what it means only under Western notation. Confirmed by 8+ independent tracks (Luhmann, functor categories, Tarski, PL environments, Saussurean value, Frege, Aristotle/Kant polarity, Madhyamaka, Alexander's kettle, Ashby's list, Rubin's reversal).

**What forced it:** The key-signature case (stress test) + eight independent formal/philosophical counterexamples.

**Tag:** [CONFIRMED — the most heavily over-determined change in the log]

### H6: DROPPED as stated (was "revised" in v0.3.0)

**What changed:** Withdrawing a context does not return the original proformation — it produces a new state carrying a trace. The erased key signature's accidentals still record the old key. Repeal a statute and accrued rights stand (UK Interpretation Act 1978 s.16). Beta-reduction replaces the redex. Closures keep their environment. Husserl's epoché yields a new noema. Quine's indeterminacy says there was never a unique original. Confirmed by all six tracks with 11 independent counterexamples.

**What forced it:** All six tracks, independently.

**Tag:** [CONFIRMED — the most uniformly supported failure in the report]

### H4: DROPPED as single test, replaced by two-kind split (was "demoted" in v0.3.0)

**What changed:** H4 fails formology's own paradigm cases — the note on the staff, "issue," and the morpheme all fail condition (b). The first pass said H4 was "too restrictive" but kept it as the pro-form test. The collaborator showed it fails even as a pro-form test (the note doesn't substitute; it *is* the pitch). Replaced by a two-kind split: placeholders (anaphoric (b)) and patterns (≥1 open parameter). Excludes anchors and limits.

**What forced it:** The seven-example table (6/7 fail (b) strictly) + the REGISTER case + model theory's free-variable/constant distinction.

**Tag:** [CONFIRMED — the deepest change in the report, deeper than v0.3.0 found]

---

## First pass revisions (v0.3.0, retained)

## 1. H1: Active → Passive

**What changed:** "Form is what stays the same when the instance changes" → "Form is what *can* stay the same — it carries the range of what it could be, and context selects from that range."

**What forced it:** The Aristotelian inversion (Aristotle's form = the active determinant; formology's form = the passive substrate) and the business case (the PO doesn't *do* anything; it *gets resolved*). H1 made form active; H2–H3 make form passive. The revision resolves the tension by making form the *carrier of the range* (passive but not empty).

**Tag:** [CONFIRMED — forced by Aristotle and the business case]

---

## 2. H2: "Undetermined" → "Underspecified"

**What changed:** "Form is complete but undetermined" → "Form is complete but underspecified — it carries a range of possible determinations."

**What forced it:** The register case (Case 1). "Issue" across registers is not blank before context — it carries a *range* of senses (problem, work item, legal point, personal objection). Context *selects* from the range, it doesn't *create* the meaning from nothing. Linguistics calls this underspecification.

**Tag:** [CONFIRMED — forced by the register case and linguistics]

---

## 3. H3: Added Level-Qualification

**What changed:** "Context is defined as what form is not" → "Context is what form is not *at that level*. At the next level up, the context is itself a form in its own context."

**What forced it:** H5 (recursion) + Aristotle. If a resolved form is itself a form at the next level, then the context at level N is a form at level N+1. "Context is not form" is true locally, false globally. The revision makes the level-dependence explicit.

**Tag:** [CONFIRMED — forced by H5 and the Aristotelian inversion]

---

## 4. H4: Demoted from Form-Test to Pro-Form Test

**What changed:** H4 was "the test for form-ness." It is now "the test for *pro-form-ness* — a specific kind of form." Form-ness is tested by H2 (does it get its meaning from a declared context?) and H1 (does it stay the same when the instance changes?). H4 tests for a *subset*: forms that substitute.

**What forced it:** The music case (notes don't substitute — they *are* the pitch), the law case (statutes don't substitute – they *are* the rule), and the business case (POs don't substitute – they *are* the order). All three satisfy H2 (form resolved by context) but fail H4 (no substitution). H4 was too restrictive as the form-ness test — it excluded clearly form-like things. Additionally, H4's three conditions are the textbook linguistic definition of a pro-form (Lyons 1977, Levinson 1983), making H4 a rename, not a novel claim.

**Tag:** [CONFIRMED — forced by the music, law, and business cases. The deepest change in the report.]

---

## 5. H5: "No Ground Level" Qualified

**What changed:** "There is no ground level" → "For forms, there is no ground level — but the recursion bottoms out at non-forms: things that directly refer (rigid designators, proper names, mathematical constants)."

**What forced it:** The non-form case (Case 3). Proper names (Kripke's rigid designators) fail the form test because they don't substitute — they directly refer. They are not "forms in a trivial context"; they are a different kind of reference (causal-historical, not descriptive). If non-forms exist, the recursion has a floor.

**Tag:** [CONFIRMED — forced by the non-form case and Kripke's rigid designation]

---

## 6. H6: Added Stateless/Stateful Distinction

**What changed:** "Resolution can be reversed by withdrawing the context" → "Resolution can be reversed by withdrawing the context, *when resolution is stateless*. When resolution is *stateful* (it causes irreversible effects), the context can be withdrawn but the effects persist."

**What forced it:** The business case. A paid PO cannot be "unresolved" — the payment has happened. Removing the AP context doesn't un-pay the invoice. Context withdrawal only works for stateless resolution (variables, notes, lazy evaluation). Stateful resolution (payments, shipments, decisions) is irreversible.

**Tag:** [CONFIRMED — forced by the business case]

---

## 7. H7: No Change

**What happened:** H7 was tested against the self-referentiality objection. The counterargument (circularity) was found to be the standard foundational move (Spencer-Brown, Peirce, set theory axioms). H7 survived unchanged.

**Tag:** [CONFIRMED — survived. Spencer-Brown and Peirce confirm foundational self-referentiality is expected, not defective.]
