---
name: paper-self-review
description: Self-review checklist for a doctoral qualitative education-research proposal or thesis draft before sending it to a supervisor or submitting it. Audits research question alignment, theoretical framework coherence, literature review argument, qualitative methodology design, ethics, trustworthiness, reflexivity, APA 7 and British English conformance, overclaiming about generative AI, and overall supervisor-readiness. Use when the user asks to "self-review", "audit my proposal", "check before submission", or "is this ready to send?".
version: 0.2.0
---

# Paper Self-Review

A structured pre-submission audit for a doctoral qualitative education-research proposal or thesis chapter. The goal is to give the user an honest read of what is ready, what is not, and what is blocking the next milestone — before a supervisor, panel, or examiner sees the draft.

This skill checks the draft against itself and against the standards of qualitative doctoral writing. It does not search for sources (`literature-review`), does not verify citations (`citation-verification`), and does not simulate a supervisor's voice (`supervisor-review`).

## When to use

Trigger when the user asks to:
- "self-review my proposal" / "audit my draft"
- "check before I submit" / "check before confirmation"
- "is this draft ready to send to my supervisor?"
- "run a quality pass on the whole proposal"
- "check whether my claims hold together"

Use after the draft is substantively complete. Not the right tool for an early outline or a single paragraph.

## What this skill audits

Six audit areas, in order. For each, the output records what is working, what is missing, what is overclaimed, and what to do next.

### 1. Alignment across the spine of the proposal
The most common doctoral-panel critique is misalignment. Check:
- Does the problem statement match the research questions?
- Do the RQs map cleanly to the analytic moves in the methodology?
- Does the theoretical framework actually shape the analysis plan, or is it name-dropped?
- Does the significance claimed at the start match what the methods can deliver?
- Do the limitations match the design, or are they generic?

### 2. Research question quality
- Are RQs open, how/what questions appropriate to qualitative inquiry?
- Has any RQ slipped into hypothesis-testing or comparative-effect phrasing?
- Does each RQ do distinct analytic work?
- Is the scope tractable for one study?

### 3. Literature review coherence
- Is the review organised thematically, advancing an argument that motivates the RQs?
- Or is it chronological / paper-by-paper / topic-list?
- Does each subsection synthesise rather than summarise?
- Is AI-in-education literature read critically — distinguishing empirical findings from vendor advocacy?
- Are the Australian / ACT context and policy instruments (e.g. Australian Framework for Generative AI in Schools) grounded, or generic?
- Are there obvious gaps a panel will notice? Differentiation, inclusive education, TPACK/AI-TPACK, teacher decision-making, ethics of AI in schools — which of these are thin?

### 4. Qualitative methodology design
- Is the paradigm named (interpretivism / constructivism) and consistent with the methodology?
- Is the methodological choice (descriptive phenomenology / interpretive phenomenology / reflexive thematic analysis) justified against the alternatives the candidate considered, not just declared?
- Is sampling logic explicit and the sample size methodologically defensible (not quantitatively defended)?
- Is the interview design described enough to evaluate (number of questions, probes, duration, mode, pilot)?
- Is ethics substantive — beyond "HREC approval obtained"? Are data management, withdrawal, sensitive content, and student privacy each addressed?
- Are trustworthiness criteria named with concrete actions (credibility, dependability, confirmability, transferability — or Braun & Clarke's quality criteria for reflexive TA)?
- Is reflexivity positioned as analytic resource, not a one-off statement?
- Do the limitations match the design? (E.g. do not flag "small sample" if the chosen methodology calls for small samples — flag what the small sample means for the kind of claim licensed.)

### 5. Claim audit — overclaiming, especially about generative AI
For each major claim in the draft, check whether evidence licenses the strength of the wording.

Use this shape:
```md
## Claim Audit

- **Claim:** <verbatim wording from the draft>
- **Location:** <section, page/paragraph>
- **Evidence anchored:** <source or "none">
- **Verdict:** keep | weaken | revise | remove
- **Overclaim risk:** none | low | medium | high
- **Suggested wording:** <a tighter alternative if needed>
```

Flag particularly:
- Promotional or transformative language about AI ("revolutionise", "transform", "unprecedented", "harness", "unlock").
- Quantitative framings inside a qualitative design ("AI improves outcomes", "leads to better differentiation").
- Agentic framings ("AI personalises learning") where the real actor is the teacher mediating the tool.
- Generalisation claims ("teachers find that...") from a study designed to surface specific lived experience.

### 6. Surface conformance
Lower priority than the five above, but flag for tidy-up:
- British English throughout (no `organize`, `analyze`, `behavior`, etc.).
- APA 7 in-text format (`Author, Year`; `et al.` from three authors; page numbers for direct quotes).
- Reference list ordering and italics conventions.
- No orphan bullet lists in body sections (lists belong to methods or appendices).
- No section opens with "In today's rapidly evolving..." or similar.
- Acronyms defined on first use.

## Audit workflow

### Step 1. Inventory the draft
Confirm what is present: which sections exist, approximate length of each, where the user has flagged a section as "not yet drafted" vs "ready for review".

### Step 2. Alignment pass
Read introduction → RQs → methodology → expected analysis as a chain. Report mismatches before reading any other section in depth.

### Step 3. Section-by-section pass
For each section, produce:
- One-line summary of what the section is doing.
- Three things that are working.
- Up to five issues, prioritised, each with a concrete next step.
- Any claim-audit entries that arose in this section.

### Step 4. Cross-section pass
Catch issues that only appear when sections are read together:
- Same construct, different names across sections (e.g. "differentiation" vs "differentiated instruction" vs "personalisation").
- Same source used in two sections with subtly different claims.
- Significance promised in the introduction but not delivered by the methodology.
- Theoretical framework cited only in one chapter.

### Step 5. Final verdict

Use one of four buckets, with a short justification:

- **Ready to send.** No blockers. Minor surface items only.
- **Ready after surface fixes.** Substantively sound; needs APA 7, British English, or formatting clean-up before sending.
- **Needs targeted revision before sending.** One or two substantive issues identified; specific next steps will close them within a week or so.
- **Not yet ready.** Alignment, methodology, or claim issues that need supervisor input or structural rework.

The verdict is honest. If the draft is not ready, say so plainly. If it is ready, say that too — empty hedging wastes the user's time.

## Output format

```md
# Self-Review: <draft name>

## Verdict
<one of the four buckets, with 2–3 sentences of justification>

## Alignment across the spine
<what holds together, what does not>

## Section-by-section
### <section name>
- One-line summary
- Working: ...
- Issues (prioritised):
  1. **Issue.** What it is. **Why it matters.** **Next step.**
  ...

## Claim audit
<table or list using the claim-audit shape above>

## Surface conformance
<short list — British English, APA 7, list misuse, etc.>

## Top three next steps
1. ...
2. ...
3. ...
```

## Sensitivity to this project

- Watch for **overclaiming about generative AI**. Flag it explicitly, with the verbatim wording.
- Watch for **slipping into quantitative framings** inside a qualitative design. Flag it.
- Check that **differentiation** is treated as teacher decision-making, not as something AI does.
- Check that **diverse learners** are characterised with care, not flattened into one category.
- Check that **ethics** is substantive throughout the design, not relegated to a paragraph.

## What this skill does not do

- Does not verify whether cited sources exist or say what is claimed → use `citation-verification`.
- Does not rewrite prose → use `qualitative-academic-writing`.
- Does not strip generic AI patterns → use `writing-anti-ai` (often runs after this audit).
- Does not simulate supervisor voice → use `supervisor-review` for that.
- Does not run statistical analysis or quantify findings.

## Quality bar before delivering the audit

- [ ] All six audit areas covered (alignment, RQs, lit review, methodology, claim audit, surface).
- [ ] Verdict bucket is named and justified.
- [ ] Each issue has a concrete next step, not just a critique.
- [ ] No invented citations or fabricated quotes from the draft.
- [ ] No vague "consider tightening" feedback without naming what to tighten.
- [ ] Tone is honest — not flattering, not harsh.
- [ ] Length matches the draft — a short proposal does not need a 20-page audit.
