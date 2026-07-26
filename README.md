# ruler-before-result

**A calibration protocol for AI-assisted research.**

Seven failure modes, a verification ledger, and a closure hierarchy for claims that depend on AI assistance — built on the premise that language models should be treated like any other instrument that drifts: fast, useful, and in need of a ruler you trust more than the device itself.

[**Read the field guide →**](./verification-methodology-v2.html)

---

## What this is

AI language models are increasingly used across research workflows — literature review, citation gathering, drafting, cross-checking claims. They are fast, cheap, and genuinely useful. They also fail in specific, recurring patterns that a casual read-through won't catch: fabricated citations that look real, real citations attached to the wrong claim, correlated confidence across multiple models, confident answers to leading questions, and systems that quietly resolve their own flagged errors.

This guide names seven of those failure modes and gives each one a concrete, checkable protocol — not a call for skepticism in the abstract, but a specific thing to do differently.

## Contents

- `verification-methodology-v2.html` — the field guide itself
- `verification-methodology.md` — plain-text source draft

## The seven failure modes

| # | Failure mode | The fix |
|---|---|---|
| 00 | Source laundering | Trace claims to their evidentiary root, not their most recent citation |
| 01 | Citation hallucination | Two-step DOI-gate: resolve the source, then match the exact quoted claim to its location in it |
| 02 | Correlated instrument agreement | Weight agreement by independence, not by headcount |
| 03 | The closed-loop trap | A flag can only be closed by something higher in the closure hierarchy than what raised it |
| 04 | False precision | Tag every claim's epistemic strength, separate from whether it's cited |
| 05 | Silent computational error | Test AI-generated code against known synthetic output before trusting it on real data |
| 06 | Leading the witness | Run high-stakes claims twice — once for, once against |

## Disclosure

This guide was produced through a multi-system review process: an initial draft, independent adversarial review passes from separate AI systems, and a synthesis pass that weighed convergent feedback against single-source suggestions before revision. Consistent with the disclosure principle in Failure Mode 00 of this guide itself — correlated agreement across reviewers counts as one signal, not several — that process is disclosed here rather than treated as incidental.

Disclosed by function: drafting, adversarial review (multiple independent systems), synthesis and revision, and structural/accessibility review were all AI-assisted. Editorial judgment on what to keep, cut, and prioritize was human.

## License

CC0 — no rights reserved. Free to reuse, adapt, or redistribute without attribution.
