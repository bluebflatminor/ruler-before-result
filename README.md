Here is the merged README — your base, with the toolkit additions woven in:
ruler-before-result
A calibration protocol for AI-assisted research.
Seven failure modes, a verification ledger, and a closure hierarchy for claims that depend on AI assistance — built on the premise that language models should be treated like any other instrument that drifts: fast, useful, and in need of a ruler you trust more than the device itself.
Read the field guide → ./verification-methodology-v2.html
Open the interactive toolkit → ./index.html (no build step; runs in any browser)
----
What this is
AI language models are increasingly used across research workflows — literature review, citation gathering, drafting, cross-checking claims. They are fast, cheap, and genuinely useful. They also fail in specific, recurring patterns that a casual read-through won't catch: fabricated citations that look real, real citations attached to the wrong claim, correlated confidence across multiple models, confident answers to leading questions, and systems that quietly resolve their own flagged errors.
This guide names seven of those failure modes and gives each one a concrete, checkable protocol — not a call for skepticism in the abstract, but a specific thing to do differently.
The toolkit edition adds what the static guide leaves out: triage rules (not every claim needs full DOI resolution), time estimates per step, interactive checklists, a live verification ledger you can edit in-place, and one-click export to Markdown or CSV.
Contents
File	Purpose
`verification-methodology-v2.html`	The original field guide (static, scrollable)
`verification-methodology.md`	Plain-text source draft
`index.html`	The interactive toolkit — triage, checklists, ledger, and export
Core principle
No orphan claims. Every assertion is tied to a verified source, a reproducible derivation, or is explicitly labeled as conjecture.
The seven failure modes
#	Failure mode	The fix
00	Source laundering	Trace claims to their evidentiary root, not their most recent citation
01	Citation hallucination	Two-step DOI-gate: resolve the source, then match the exact quoted claim to its location in it
02	Correlated instrument agreement	Weight agreement by independence, not by headcount
03	The closed-loop trap	A flag can only be closed by something higher in the closure hierarchy than what raised it
04	False precision	Tag every claim's epistemic strength, separate from whether it's cited
05	Silent computational error	Test AI-generated code against known synthetic output before trusting it on real data
06	Leading the witness	Run high-stakes claims twice — once for, once against
Using the toolkit
1.  Triage Calculator — Classify each claim as P0 (design-critical), P1 (supporting), or P2 (background). This sets your verification depth, time budget, and required closure authority.
2.  Failure Modes — Run the relevant interactive checklists. Each item has an estimated time cost. Check boxes off as you complete them.
3.  Verification Ledger — Log every claim, its source, exact location, method, status, and strength. Add rows as you go; edit in-place.
4.  Export — Dump the ledger as Markdown or CSV for your paper's supplementary materials.
Triage levels
Level	Role	Time budget	Closure authority
P0 — Design-critical	Central to a design decision; used in calculations; if wrong, the conclusion fails	45–90 min	Human domain expert or primary source only
P1 — Supporting	Background, motivation, related-work comparisons	15–30 min	Primary source or reproducible computation
P2 — Background	General field knowledge, well-established facts	5–10 min	Independent retrieval system acceptable
Closure hierarchy
An AI-raised flag can only be closed by something higher in this chain. AI-only closure stays Provisional, never final.
AI-raised flag → Primary source → Reproducible computation → Human expert → Independent retrieval system
Copying on iOS
iPhone auto-corrects triple dashes (---) to an em dash when pasting into standard text fields. If you are copying protocol text or ledger exports from this repo on an iPhone and the dashes collapse:
•  Go to Settings → General → Keyboard → Smart Punctuation and turn it OFF, then copy-paste again; or
•  Copy from fenced code blocks rather than plain paragraph text — iOS is less likely to smart-punctuate text copied from <code> regions.
Disclosure
This guide was produced through a multi-system review process: an initial draft, independent adversarial review passes from separate AI systems, and a synthesis pass that weighed convergent feedback against single-source suggestions before revision. Consistent with the disclosure principle in Failure Mode 00 of this guide itself — correlated agreement across reviewers counts as one signal, not several — that process is disclosed here rather than treated as incidental.
Disclosed by function: drafting, adversarial review (multiple independent systems), synthesis and revision, and structural/accessibility review were all AI-assisted. Editorial judgment on what to keep, cut, and prioritize was human.
License
CC0 — no rights reserved. Free to reuse, adapt, or redistribute without attribution.
