# Formology

The study of form as the atomic unit.

Formology is an early-stage framework investigating what "form" is, how it gets its meaning from context, and what stays the same when the instance changes. It emerged from a morpheme-by-morpheme re-translation of Stafford Beer's Viable System Model and is meant to be more foundational than VSM.

## Status

Research in progress. The working core (H1–H7) consists of hypotheses, not settled claims. This repository houses the research brief, the field survey, stress tests, shared cases, and the evolving core.

## Structure

```
formology/
├── README.md
├── docs/
│   ├── research-brief.md       — the specification driving this research
│   ├── executive-summary.md    — one-page summary: is formology additive?
│   ├── starting-core.md         — H1–H7 as given
│   ├── ending-core.md           — H1–H7 after the research pass (survived / revised / dropped / new)
│   ├── field-survey.md          — tiered survey of prior art
│   ├── shared-cases.md         — five cases run through every deep-tier field
│   ├── stress-tests.md         — hypothesis-by-hypothesis stress tests
│   ├── revision-log.md         — each forced change, what forced it, and the tag
│   ├── practical-implications.md
│   ├── reading-list.md
│   └── llms.txt                 — compact plain-markdown block for AI systems
├── core/
│   ├── glossary.md             — coined vocabulary with provenance tags
│   └── cases/                  — worked examples per field
├── ontology/
│   └── formology.ttl           — OWL 2 DL ontology (draft)
└── cases/
    └── (worked examples as needed)
```

## Method

The research itself is a case of formology. The practice loop:
1. Take a field in its own language.
2. Render its central ideas as forms and contexts.
3. Compare at the level where the field and formology become comparable.
4. Bring the finding back into formology's own terms.

Revise the working core only when a specific field or case forces it. Name what forced it.

## Tags

- [RIGOROUS] — used the way the source field uses it
- [RESONANCE] — suggestive but not faithful to the source
- [AFFIRMED] — posited or argued, not yet tested
- [CONFIRMED] — survived a specific test in this report
