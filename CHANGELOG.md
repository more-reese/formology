# Formology — Development Log

*Reverse chronological. Most recent changes at the top. The story of how formology is developing.*

---

## v0.4.0 — October 8, 2026 — The Collaborator Review

**What happened:** A collaborating formologist conducted a substantially more rigorous review across ~20 fields, organized into six research tracks (philosophy, linguistics/PL, formal, cybernetics, stress test, applied). The review found failures the first pass missed and identified prior art the first pass overlooked.

**The headline:** "Formology survives as a method, not a theory." None of H1–H7 survives unchanged. Two hypotheses fail outright (H3, H6). The honest verdict is "a patchwork of renames with one or two additions."

**What fell:**

- **H3 fell** as an ontological claim. "Context is not form" is false — every context formology names (key signature, environment, statute) is itself a form by H4's own test. The key signature occupies a slot, stands in for something recoverable, and means what it means only under Western notation. Confirmed by 8+ independent tracks. Survives only as role naming: "context" names a role in a resolution, not a kind.
- **H6 fell** as stated. Withdrawing a context does not return the original proformation — it produces a new state carrying a trace. Erase a key signature and the accidentals still record the old key. Repeal a statute and accrued rights stand (UK Interpretation Act 1978 s.16). Confirmed by all six tracks with 11 independent counterexamples.
- **H4 fell** as a single conjunctive test. It fails formology's own paradigm cases: the note on the staff, "issue," and the morpheme all fail condition (b) ("stands in for something recoverable"). The pointing demonstrative "that," which has the least invariant content, passes all three. Replaced by a two-kind split: **placeholders** (anaphoric (b): pronouns, blank fields) and **patterns** (≥1 open parameter: types, open terms, "issue"). Excludes **anchors** (proper names, one-time keys, brute facts) and **limits** (the unmarked state).

**What changed:**

- **H1** has a free parameter: which changes count as "the same thing changing" is itself the form. The Ship of Theseus makes it concrete. Depends on H2, not ground-floor.
- **H2** lost four qualifiers: "complete" (Hart's open texture), "undetermined" (Carnap's intension is a complete function), "declared" (registers are recognized, not declared; Kaplan's context is a parameter), "one bit" (the pivot chord is doubly determined).
- **H5** keeps recursion, gains "no top" (Tarski, Girard), loses "no ground level" (Frege, Aristotle, Kant, PL literals all have grounds). Disjointness of proformation/conformation holds per record, not per thing.
- **H7** survives as a chosen posit (Fichte's Setzen, Spencer-Brown's injunction) but treatise 12.2's self-confirmation is circular and 7.5 as written absorbs counter-evidence. Add disconfirmation clause: register rejection, nesting failure, invariance failure.

**New prior art the first pass missed:**

- **Model theory (Tarski/Carnap):** interpretation of an open formula by a structure — does H2 cleaner than formology. Carnap's intension/extension dissolves the disjointness-vs-recursion problem by type.
- **Kaplan's character/content:** structurally identical to H2 with a complete function. Context is a parameter, not a declaration. Content is a rigid designator, not re-resolvable.
- **PL theory open terms:** unbound variable = proformation, environment = context. Thunks separate having a context from being resolved — formology fuses these.
- **Alexander's kettle:** form/context with a movable boundary. "Widen the frame and the kettle becomes part of the context, while the stove perhaps is form." Breaks H3-as-absolute.
- **Eigenform (von Foerster):** objects as fixed points of an observer's repeated operation. Form is *produced* by the operation, not read from a pre-existing invariant.
- **Hart's penumbra:** core/penumbra as the clearest statement that a form is fixed but underspecified. In the penumbra, the judge's act adds content.
- **Hollnagel's WAI/WAD:** work-as-imagined vs. work-as-done — the actual source of the POSIWID gap, with four varieties (imagined, prescribed, disclosed, done), not two.
- **Madhyamaka (Nagarjuna):** dependent origination = H4(c) as a universal. "Emptiness of emptiness" = H5+H7 with more care than the treatise.
- **Canalisation:** a form built so context barely matters — reverses the arrow of H3.

**The "two jobs" problem (H10, new):** The word "form" does two opposite jobs in every deep field. The invariant (Peirce's type, Aristotle's form) and the undetermined thing a context determines (Peirce's token-before-language, Aristotle's matter) are different items. Formology merges them in one word, which is the source of the disjointness-vs-recursion problem and the form/proformation collapse suspicion.

**Recommended next step:** Adopt the ending core v0.4.0. Replace the two disjoint classes in the ontology with one relation `resolvedBy(form, context)`. Derive "level" as chain length. Run the "issue" register case under the rewritten rules, hunting for a practice-level disconfirmation. If none appears, that is the first [CONFIRMED] tag earned in practice rather than by consistency.

---

## v0.3.0 — October 8, 2026 — The Research Pass

**What happened:** A full research pass was conducted against ~20 fields of prior art, with 5 shared cases run through every deep-tier field and all 7 hypotheses stress-tested. The pass was driven by a structured research brief from a collaborating formologist.

**The big change: H4 was demoted.**

H4 — the three conditions for form-ness (structural slot, substitution, anaphoric interpretation) — was the foundation of formology's claim to novelty. The survey showed it is the textbook definition of a linguistic pro-form (Lyons 1977, Levinson 1983). It does not define form; it defines pro-forms, which are a *subset* of forms. Form is broader: things that carry a range of potential determinations and get their meaning from a declared context (H2), whether or not they substitute for something.

This is the deepest change in the report. It means formology's core is not the three conditions (those are linguistics) but the *form/context distinction applied beyond linguistics* — to business, cybernetics, law, music, and any system where something gets its meaning from a declared context.

**Other revisions:**

- **H1:** "Form is what stays the same" → "Form is what *can* stay the same — it carries the range, context selects." Active → passive. Forced by the Aristotelian inversion: Aristotle's form is the determinant; formology's form is the substrate.
- **H2:** "Undetermined" → "underspecified." Form before context carries a *range* of determinations, not nothing. Forced by the register case ("issue" across CEO, developer, lawyer, everyday speech).
- **H3:** Level-qualified. "Context is what form is not" holds locally but not globally — at the next level up, the context is itself a form.
- **H5:** "No ground level" → "no ground level *for forms* — but recursion bottoms out at non-forms (rigid designators, proper names)." Forced by the non-form case.
- **H6:** Reversibility qualified — stateless resolution is reversible; stateful resolution (payments, shipments) is not. Forced by the business case.
- **H7:** Survived unchanged. The self-referentiality ("form cannot be proven since proof requires form") is the standard foundational move, confirmed by Spencer-Brown and Peirce.

**New hypotheses:**

- **H8:** Form carries a range of potential determinations. Context selects; it does not create. This is underspecification, not emptiness. The most novel claim in the framework.
- **H9:** The recursion bottoms out at non-forms: things that directly refer (rigid designators) rather than substitute. The ground level exists.
- **H10:** Resolution is either stateless (reversible) or stateful (irreversible — effects persist after context withdrawal).

**Key prior-art findings:**

| Formology claim | Verdict | Closest prior art |
|---|---|---|
| H1 (form = invariant) | Rename | Peirce type/token; Gentner relational structure |
| H4 (three conditions) | Rename of pro-form definition | Lyons, *Semantics* (1977) |
| Proformation/conformation | Rename of anaphora resolution states | Halliday & Hasan (1976) |
| H3 (context = not-form) | Rename | Beer, *Diagnosing the System* (1985) |
| The fork | Rename | Gentner's mapping limit (1983) |
| H8 (underspecification as state) | **Novel** | — (Frege has it as failure; linguistics as ambiguity) |

**The single most important prior-art match:** Spencer-Brown's *Laws of Form* (1969). The mark is the closest existing primitive — distinction + indication + operation in one. Formology diverges by separating form from context and adding the underspecification state.

**Recommended next step:** Integrate with linguistics rather than parallel to it. The novel contribution (underspecification as a legitimate state) is best developed in dialogue with computational linguistics. The proformation/conformation terminology should be presented as a generalization of anaphora resolution, not as a new field.

---

## v0.2.0 — September 16, 2026 — Formology Named, Morphology Stress-Tested

**What happened:** The framework was named "Formology" and rooted in form as the atomic unit (previously "pro-form" was the atom). The productive morphology was expanded to two axes: suffix (grammatical function) and prefix (resolution state). The pro/con prefix system was stress-tested against VSM and found to work cleanly with the root "form" but predicted to break on other roots (e.g., "struct").

**Key developments:**

- Atomic unit shifted from "pro-form" to "form." Proformation (pre-context) and conformation (post-context) became resolution states, not the atom itself.
- VSM mapping fully worked through: S5 = form (invariant), S4 = proformation (latent edge), S3 = formalize (resolution management), S2 = formal (anti-oscillatory grammar), S1 = conformation (operations), environment = conform (verb, the shaping force).
- Morphology mapped as a coordinate system: prefix = direction (where in the system), suffix = orientation (what kind of attention).
- The POSIWID gap characterized: design intent = proformation, actual behavior = conformation, the gap is the condition of viability (where S4 operates).
- Caveat noted: the pro/con prefix system works with "form" but does not generalize to all roots. Left as an open question.

**Artifacts:** Skill updated to v0.2.0. Vault updated in Obsidian (35 files, ~2,165 lines). OWL ontology scaffolded in Protégé.

---

## v0.1.0 — September 1, 2026 — Pattern Language Origin

**What happened:** Formology emerged from a morpheme-by-morpheme re-translation of Stafford Beer's Viable System Model vocabulary. The initial framing was a "shared operating language built on pro-forms" — patterns whose meaning is resolved by context, carried by a productive morphology.

**Origin:** The re-translation produced the insight that VSM's vocabulary (transduce, environment, system, operations, intelligence, policy) could be decomposed into morphemes that each carry structural roles. "Transduce" = trans (boundary) + duct (channel). The boundary and the channel are forms — structural roles that persist across the specific words that fill them.

**Initial principles:**
- The atomic unit is the pro-form (later revised to form in v0.2.0).
- Productive morphology: state (noun) → property (adjective) → action (verb).
- Form is invariant; conformation is variable; context determines resolution.
- "At high enough levels of abstraction, all forms are the same."
- The development process is self-describing: emerge → formalize → express → feedback → refine.

**Proven artifacts as case studies:** substrate (coordination language), vsm-translator (bidirectional translation), TMCO Revenue System (ASU/AUV, typed state machine), Decrypt articles (bidirectional translation), dreamward C0 (formal proof).

**Note:** This version was the starting point. Many of its claims were revised or demoted in v0.3.0.
