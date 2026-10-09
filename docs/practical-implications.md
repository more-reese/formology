# Practical Implications

## For systems and process consulting

Formology reveals what standard process mapping doesn't: the *persistence of form across conformations*. In the purchase order case (Case 5), the same PO is a need, a commitment, an order, and a liability — one form traversing four registers. Standard process mapping sees four documents; formology sees one form resolved by four contexts.

**Practical use:** When mapping a process, identify what form persists across steps. The form is the thread; the steps are the conformations. The POSIWID gap (design intent vs. actual behavior) is where the process is alive — where to focus improvement. The stateless/stateful distinction (H6/H10) tells you which steps can be reversed (drafts, approvals before signing) and which can't (payments, shipments).

**What to drop:** The proformation/conformation terminology for clients. Use "the same thing seen from different angles" — the formology is in the analysis, not the vocabulary.

## For designing English-like modeling languages

The form/context distinction suggests a design principle: **separate the form (what the model says) from the context (what it means in a specific deployment).** A model that hardcodes its interpretation is a literal (it carries its own meaning). A model that carries a range and lets the deployment context select is a form — it is reusable across deployments.

**Practical use:** Design models as underspecified (carrying a range of potential determinations) and let deployment contexts resolve them. This is already how configuration systems work (a config is a form; an environment is a context). Formology's contribution is naming the pattern and connecting it to linguistics, cybernetics, and philosophy.

## For AI agents working across domains

The form/context framework is directly applicable to AI agent design:

1. **Skills as forms.** A skill (like the Hermes pattern-language skill) is a form — it carries a range of potential determinations (it can be applied to linguistics, business, music, law). The session context resolves it (selects which determination is active). This is formology applied to the skills system.

2. **Profiles as conformations.** Each profile is the same agent (form) resolved by a different context (the profile's config, memory, skills). This is the dossier metaphor: the dossier carries the form; the clearance level is the context.

3. **Underspecification as a design principle for agents.** An agent that is too specifically configured (it knows exactly what to do in one context) is a literal. An agent that is underspecified (it carries a range of potential behaviors and the session context selects) is a form — it generalizes. The design question is: how much should the agent carry (the range) vs. how much should the context supply (the selection)? Formology frames this as the form/context division of labor.

4. **The POSIWID gap for agents.** The designed purpose of an agent (proformation — what you intended it to do) vs. its actual behavior (conformation — what it does in practice) is the gap where agent improvement lives. Monitoring this gap is the S4 function — the agent's intelligence layer sensing the difference between intent and behavior and feeding it back.
