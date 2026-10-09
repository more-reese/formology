# Case Study: BUSINESS — Purchase order under v0.4.0 rules, with reader-as-context

*Fourth practice-level case. Run date: October 8, 2026. This is the case the collaborator review called "the fairest test" — it has the most structure and the most at stake. The reader-as-context rule (H9) is explicitly applied: the same PO is read differently by the requester, the approver, the AP clerk, and the auditor.*

---

## The case

A generic purchase order (PO-1234) for $4,500 of office supplies from Vendor Corp, moving through a mid-sized company:

1. **Request:** Employee needs supplies → creates PO-1234
2. **Approve:** Manager reviews → approves (under $5,000 threshold)
3. **Issue:** PO sent to Vendor Corp
4. **Fulfill:** Vendor ships supplies
5. **Receive:** Shipping dock confirms delivery
6. **Invoice:** Vendor sends invoice referencing PO-1234
7. **Match:** AP clerk matches PO + invoice + receiving record (three-way match)
8. **Pay:** AP issues payment

## Step 1: Take the process in its own language

Standard process mapping (BPMN, SIPOC) sees: a linear flow with eight steps, each transforming the PO's state. The PO is a document that moves through a workflow. Actors are assigned per step. Gates control transitions (approval threshold, three-way match). Exceptions are handled in a queue.

## Step 2: Render as forms and contexts, with readers

Under v0.4.0 rules, the PO is a **form** — a pattern with at least one parameter left open. The open parameters include: what kind of thing the PO *is* (a need, a commitment, an order, a liability, evidence), and who is reading it (the reader's role determines the reading).

The **readers** are the contexts (H9). Four readers, four glossaries, four readings of the same form:

### Reader 1: The Requester (Employee)

**Glossary:** Need, requisition, budget, "my order"
**Reading:** The PO is a *need* — "I need these supplies." The PO is the expression of a requirement. The requester sees the PO from the inside: they know what they need and why. The PO is their voice in the procurement system.
**What the PO is for them:** A requisition — a request to spend company money for a legitimate business purpose.

### Reader 2: The Approver (Manager)

**Glossary:** Budget, approval threshold, authority, "should we spend this?"
**Reading:** The PO is a *commitment* — "if I approve this, we're committing $4,500 from the office supplies budget." The approver sees the PO as a decision: should this be approved? The threshold ($5,000) is part of their glossary — the PO is under it, so it's a routine approval.
**What the PO is for them:** A budget commitment — a request to authorize spending that will count against their budget.

### Reader 3: The AP Clerk (Accounts Payable)

**Glossary:** Invoice, three-way match, ledger, "does this agree?"
**Reading:** The PO is a *liability* and a *matching reference* — "we owe Vendor Corp $4,500, and I need to match the PO, the invoice, and the receiving record." The AP clerk sees the PO as a record to be matched. The three-way match is their glossary's primary test: does the PO agree with the invoice and the receiving record?
**What the PO is for them:** A liability — a financial obligation, and a matching reference for the three-way match.

### Reader 4: The Auditor (Internal or External)

**Glossary:** Control, evidence, compliance, segregation of duties, "was this done correctly?"
**Reading:** The PO is *evidence* — "this document shows that the procurement process was followed." The auditor sees the PO as a record that proves the process worked. Was it approved by someone with authority? Was the three-way match performed? Was there segregation of duties between the requester and the approver?
**What the PO is for them:** Evidence — a record that demonstrates compliance with internal controls.

## Step 3: Compare at the level where the readers become comparable

The four readers are comparable at the level of "what is the PO *to this reader*?" This is the open parameter (H4' pattern). The word changes with the reader:

| Reader | What the PO is | Glossary | Form or anchor? |
|---|---|---|---|
| Requester | A need ("my order") | Requisition, budget | Pattern (conformation) |
| Approver | A commitment ("should we spend this?") | Budget, threshold, authority | Pattern (conformation) |
| AP Clerk | A liability + matching reference ("does this agree?") | Invoice, ledger, three-way match | Pattern (conformation) |
| Auditor | Evidence ("was this done correctly?") | Control, compliance, segregation of duties | Pattern (conformation) |

All four readers are conformations of one form (the PO). The form is a pattern: "what the PO is" is the open parameter, and the reader's role supplies the reading. No reader is an anchor — each has a glossary that supplies a determinate reading.

### The invariant

What stays the same across all four readings? What is the form that persists?

The invariant is: **a record of an intended transaction.** In all four readings, the PO is a record of a transaction that someone intended to happen. The requester records their intent to buy. The approver records their intent to commit budget. The AP clerk records the intent to pay. The auditor records that the intent was followed through correctly.

Does this invariant do work?

- **Requester:** Yes — "a record of an intended transaction" tells the requester that their need has been formalized. Without the PO, the need is informal; with it, it's a record.
- **Approver:** Yes — the record tells the approver what they're committing to. The record is the commitment.
- **AP Clerk:** Yes — the record is what they match against. Without the record, there's nothing to match the invoice to.
- **Auditor:** Yes — the record is the evidence. Without the record, there's nothing to audit.

**The invariant holds in all four readings and does work.** No invariance failure.

### The reader-as-context (H9)

The key finding: **BPMN has lanes for who acts (requester creates, approver approves, AP pays). Formology adds lanes for who reads the same artifact differently.** The same PO-1234 is:
- "My order" to the requester
- "A budget commitment" to the approver
- "A liability + matching reference" to the AP clerk
- "Evidence of compliance" to the auditor

These are four conformations of one form, resolved by four different reader-contexts. The form persists ("a record of an intended transaction"); the conformations change with the reader.

This is what the collaborator review identified as formology's actual addition over standard process mapping: **a place for readers.** BPMN tracks the flow of the PO through the process. Formology tracks the readings of the PO by different readers. Both are real; they are complementary.

## Step 4: Bring the finding back into each reader's terms

### Requester

"The PO is my order — I created it because I need supplies. But the same document means different things to different people. My manager sees it as a budget commitment. AP sees it as something to match against an invoice. The auditor sees it as evidence that the process worked. It's the same PO number, the same line items, the same amount — but the meaning changes with who's reading it. That's what formology calls the reader-as-context."

### Approver

"When I approve a PO, I see it as a budget commitment — am I authorizing $4,500 of office supplies spending? But the same PO is a need to the person who requested it, a liability to the AP clerk who has to pay it, and evidence to the auditor who checks the process. The PO doesn't change — the reader changes. My role as approver gives me a glossary (budget, threshold, authority) and that glossary determines what the PO is for me. That's the formology reading."

### AP Clerk

"I do the three-way match — PO, invoice, receiving record. If they all agree, I pay. But the PO I'm matching is not the same PO the requester created — not in meaning. The requester sees a need. The approver sees a commitment. I see a liability and a matching reference. The auditor sees evidence. Same document, four meanings, four readers. Formology calls that the reader-as-context: the reader's role determines what the form means. My glossary is invoices and ledgers; that's what I bring to the PO."

### Auditor

"I check whether the process was followed. The PO is evidence — was it approved by someone with authority? Was the three-way match done? Was there segregation of duties? But the same PO is a need to the requester, a commitment to the approver, a liability to AP. The document doesn't change; the reader does. Formology gives that a name: the reader is a context. BPMN tracks who acts on the PO. Formology tracks who reads it and what it means to them. That's the addition — not a new process, but a new lane for readers."

## Step 5: Hunt for disconfirmations

### 1. Register rejection: Do competent users reject the rendering?

**Requester:** Would an employee reject the claim that the PO is "a record of an intended transaction" and that it means different things to different readers? Unlikely — employees already know that the PO they create goes to different people who use it differently. Acceptable.

**Approver:** Would a manager reject it? They already know that what they see as a "budget commitment" is a "need" to the requester. The rendering is recognizable. Acceptable.

**AP Clerk:** Would an AP clerk reject the claim that the PO is "a liability + matching reference" in their register? No — that's exactly what they do. The claim that it's also "a need" to the requester and "evidence" to the auditor is also recognizable. Acceptable.

**Auditor:** Would an auditor reject the claim that the PO is "evidence" in their register? No — that's exactly what auditors call it. The claim that it's different things to different readers is standard audit thinking (the same document has different significance depending on the control objective). Acceptable.

**No register rejection found.** All four readers accept the rendering.

### 2. Nesting failure: Is a declared nesting shown not to nest?

The nesting: the PO as "a record of an intended transaction" is one instance of the higher-level form "records that are read differently by different roles." Is this nesting real?

"Records that are read differently by different roles" is a real class — medical records (doctor reads differently from patient, insurer, researcher), legal documents (lawyer reads differently from client, judge, opposing counsel), financial statements (CFO reads differently from auditor, investor, regulator). The PO is one instance of this class. The nesting holds.

But: is "records that are read differently by different roles" just "documents"? No — it is the class of records where the *same record carries different meanings depending on the reader's role*. Not all documents do this — a memo has one meaning (it says what it says). A PO does this: it is a need, a commitment, a liability, and evidence depending on who reads it. The nesting holds at the level of "role-dependent records," not "documents."

**No nesting failure found.**

### 3. Invariance failure: Does an agreed instance lack the claimed invariant?

The claimed invariant: "a record of an intended transaction."

- Requester: ✅ The PO records their intent to buy.
- Approver: ✅ The PO records their intent to commit budget.
- AP Clerk: ✅ The PO records the intent to pay (and is matched against the invoice and receiving record to confirm the intent was fulfilled).
- Auditor: ✅ The PO records that the intent was followed through correctly (it is evidence of the intended transaction being executed properly).

The invariant holds in all four readings. No invariance failure.

But: is the invariant too thin? "A record of an intended transaction" could describe almost any document in a business process. Is it vacuous?

No — it is doing work: it is distinguishing the PO from the invoice (which is a record of an *actual* transaction, not an *intended* one) and from the receiving record (which is a record of an *actual* delivery). The PO is the record of *intent* — what was supposed to happen. The invoice and receiving record are records of *what happened*. The invariant distinguishes intent from actuality, which is exactly the PO's role in the three-way match.

**No invariance failure found.** The invariant holds in all four readings and does real work (distinguishing intent from actuality).

## Verdict

**The case survives. No disconfirmation found. Fourth [CONFIRMED] tag.**

Key findings:

1. **The reader-as-context (H9) is formology's actual addition over process mapping.** BPMN has lanes for who acts. Formology adds lanes for who reads. The same PO is four things to four readers: a need, a commitment, a liability, and evidence. The form persists ("a record of an intended transaction"); the reader's role determines the conformation. This is not a new process — it is a new dimension of the same process.

2. **The invariant "a record of an intended transaction" does real work.** It distinguishes the PO (intent) from the invoice (actuality) and the receiving record (actuality). The three-way match is a test of whether intent and actuality agree — three conformations of one form (PO, invoice, receiving record) must agree on the invariant (amount, items, vendor). The collaborator review identified this as "what the three-way match is for."

3. **The four readers all have glossaries.** Unlike the "issue" case (where the everyday reader had no glossary) and like the "case" case (where all four readers had glossaries), all four PO readers have professional glossaries. The form is strong — no boundary case.

4. **The form is a pattern, not a placeholder.** "What the PO is" (need, commitment, liability, evidence) is the open parameter. The word "PO" does not stand in for a recoverable antecedent in the way a pronoun does — it is a document with a number. But it has at least one parameter open (what it means to the reader), which makes it a pattern under H4'. This is a weaker form than "case" (which was both placeholder and pattern) but a real form.

5. **The POSIWID gap is visible.** The *designed purpose* of the PO (proformation — what the process was designed to do: control spending, ensure approval, track fulfillment) vs. the *actual behavior* (conformation — what the process does in practice: rubber-stamp approvals under threshold, rush orders that bypass the process, invoices that don't match POs). The gap is where the process is alive — where the auditor's register (H9) detects the difference between intent and actuality.

## Cross-case comparison

| Property | "issue" | "case" | "charge" | PO |
|---|---|---|---|---|
| Registers tested | 4 | 4 | 4 (+ 2 everyday sub-uses) | 4 readers |
| Conformations | 3 | 4 | 5 (1 weak) | 4 |
| Boundary case | Yes (everyday) | No | Yes (emotion, weak) | No |
| Placeholder (H4b) | No (donkey anaphora) | Yes | Yes | No (pattern only) |
| Pattern (H4') | Yes | Yes | Yes | Yes |
| Invariant | "demands attention" | "a unit of situation" | "a transfer to a target" | "a record of an intended transaction" |
| Invariant does work? | 3/4 | 4/4 | 5/6 | 4/4 |
| Disconfirmation found? | No | No | No | No |

**Across four cases: zero disconfirmations.** The v0.4.0 rules survive all four practice-level tests. The framework correctly:
- Identifies boundary cases (everyday "issue," emotional "charge") as proformations or weak conformations
- Holds the form across all conformations
- Distinguishes placeholders from patterns
- Applies the reader-as-context rule to identify what standard process mapping misses
- Earns [CONFIRMED] tags in practice, not by consistency

## What the PO case adds to the practice

1. **The reader-as-context is the addition.** The collaborator review said "formology adds a place for readers" — the PO case confirms this in practice. BPMN has lanes for actors; formology adds lanes for readers. This is not a new process; it is a new dimension.

2. **The three-way match is a form-agreement test.** Three conformations of one form (PO, invoice, receiving record) must agree on the invariant (amount, items, vendor). Disagreement means at least one context resolved it differently. Formology names what the match is *for*: testing whether three conformations agree.

3. **The POSIWID gap is the auditor's register.** The gap between the PO as designed (proformation — what it was intended to be) and the PO as executed (conformation — what it actually became) is where the auditor operates. The auditor's register is the one that detects the gap — which is H7's "disconfirmation in practice."

4. **About half of what formology adds is already standard practice.** The collaborator review noted this: "anyone who runs work-as-imagined/work-as-done interviews and role-based requirements gathering already has most of points one and four." The honest summary: formology gives a one-page vocabulary that ties together standard practices (Hollnagel's WAI/WAD, role-based requirements, the three-way match) and a reason they belong together. It does not give a new method.
