---
name: qualitative-academic-writing
description: Draft and revise qualitative academic prose for education research — proposals, theses, and journal articles. Use when the user asks to write or improve background/context, literature review, methodology, findings, discussion, or conclusion sections in a qualitative study. Default to British English and APA 7. Two-stage process — section outline first, then flowing paragraphs. Never invents citations and avoids overclaiming the benefits of generative AI.
allowed-tools: Read Write Edit Bash
license: MIT license
---

# Qualitative Academic Writing

## Overview

Drafting and revising scholarly prose for a qualitative education-research study. The target outputs are research proposals, doctoral theses, and qualitative journal articles — not biomedical IMRAD papers. The style is interpretive and reflexive, the citation system is APA 7, and the spelling is British English.

This skill is the writing companion to:
- `literature-review` — for searching and synthesising sources
- `citation-verification` — for confirming references before any claim
- `qualitative-findings-analysis` — for coding, themes, and quote selection
- `research-methodology-skill` — for paradigm, design, and methods wording
- `supervisor-review` — for honest pre-supervision feedback

## When to use

Trigger this skill when the user asks to:
- draft or rewrite a section of a research proposal or thesis (background, context, problem statement, significance, literature review, theoretical framework, methodology, findings, discussion, conclusion)
- tighten or "humanise" qualitative prose without changing its meaning
- shift writing into British English and APA 7
- check whether a paragraph overclaims, particularly about generative AI in education
- structure a section before writing it (outline-first workflow)

Do **not** use this skill for:
- finding sources → use `literature-review`
- verifying that a citation exists and says what the draft claims → use `citation-verification`
- coding interview data or building themes → use `qualitative-findings-analysis`
- formal reviewer/examiner response letters → use `review-response`

## Non-negotiables

1. **Never fabricate citations.** If a claim needs a source and the source is not in the user's library or supplied evidence, mark it `[citation needed]` and stop — do not invent an author, year, journal, or DOI. Defer verification to `citation-verification`.
2. **Do not overclaim about generative AI.** Avoid promotional language ("revolutionise", "transform", "unprecedented"). Frame AI uses as emerging, contested, and context-dependent. Pair affordances with constraints and ethical considerations.
3. **Preserve the researcher's voice.** Keep hedged, exploratory phrasing intact. Do not flatten reflexive first-person passages into impersonal generalisations unless the user asks.
4. **British English.** `organisation`, `behaviour`, `centre`, `analyse`, `recognise`, `programme` (in the educational sense), single quotes for first-level quotation in body text where the user's style allows.
5. **APA 7 throughout.** Author–date in-text citations (`Smith, 2024`; narrative `Smith (2024) argues...`). Use `et al.` from the first citation when there are three or more authors. Page numbers for direct quotes. Reference list entries follow APA 7 ordering and italics conventions.
6. **No promotional summaries.** Do not end sections with vague "in conclusion, this work demonstrates the potential of..." flourishes.

## Two-stage writing process

Always work in two passes. Bullet-point scaffolding belongs to stage one only — the deliverable is full prose.

### Stage 1 — Section outline with evidence anchors

Before drafting, build an outline that lists, for each paragraph:
- the claim or move the paragraph makes
- the evidence anchor (author–year, participant quote ID, document, or `[citation needed]`)
- the connection to the research question(s) it serves
- any tension or counter-evidence to acknowledge

Example (Literature Review subsection on differentiation):
```
Para 1 — Define differentiated instruction as a teacher decision-making practice,
         not a fixed method (Tomlinson, 2014; Scarparolo & Porta, 2025).
         Frame for AU secondary context.
Para 2 — Tension: rhetorical commitment vs. uneven enactment in AU schools
         (Porta, 2022; [citation needed for ACT-specific data]).
Para 3 — Connect to RQ1 by foregrounding the teacher as decision-maker rather
         than the technology as agent.
```

The outline is for planning. Do not deliver it as the final section.

### Stage 2 — Flowing paragraphs

Convert each outline point into connected sentences. Each paragraph should:
- open with a topic sentence that states the move
- develop with evidence and example
- close by linking forward, not by summarising what was just said
- integrate citations inside sentences rather than parking them at the end as a list
- use transitions that signal logical relations ("however", "by contrast", "building on this") rather than empty connectives ("furthermore", "moreover" used decoratively)

Vary sentence length. Use the first person ("I") where the user's methodology warrants reflexive positioning. Avoid passive voice as a default; use it only where the actor is genuinely unknown or unimportant.

## Section-by-section guidance for qualitative education research

### Background and context
Locate the study in time, place, and policy. For Australian education research, name the jurisdiction (ACT, sector — public/Catholic/independent), the relevant policy instrument (e.g. the Australian Framework for Generative AI in Schools), and the population (secondary teachers, year levels). Avoid generic openings about "the rapid rise of AI".

### Problem statement and significance
State what is missing in current understanding, not just what is happening in the world. Significance for a qualitative study lies in the insight gained from teachers' lived practice, not in generalisability claims. Make the gap small enough to plausibly close in one study.

### Literature review
Organise thematically, not chronologically. Synthesise — do not summarise paper-by-paper. Each subsection should advance an argument that motivates the research questions. Surface tensions and gaps. Treat AI-in-education literature critically: distinguish empirical findings from vendor advocacy.

### Theoretical framework
State which framework is doing analytical work (e.g. TPACK, AI-TPACK, sociocultural theory of teacher decision-making, ecological theory, UDL). Explain *how* it will be used in analysis — as a sensitising lens, a coding frame, or an interpretive scaffold — not just that it is "guiding" the study.

### Research questions
Phrase as open, how/what questions appropriate to qualitative inquiry. Avoid yes/no or comparative-effect phrasing. Each RQ should map to an analytic move; if it does not, it belongs in the discussion, not as an RQ.

### Methodology
Defer detailed wording to `research-methodology-skill`. In a written section, the order is usually: paradigm → methodology (e.g. interpretive phenomenology) → participants and sampling → data generation (semi-structured interviews) → analysis approach (e.g. reflexive thematic analysis) → ethics → trustworthiness → reflexivity → limitations. Each subsection should justify its choice in relation to the RQs, not list options.

### Findings (for completed studies)
Lead with themes, not participants. Anchor each theme in 2–4 representative quotes with pseudonyms. Quote selection should privilege illustrative power over coverage. Use participant voice generously but always interpret — do not let quotes "speak for themselves".

### Discussion
Move from theme to claim to literature to so-what. Read findings back against the theoretical framework. Acknowledge what cannot be said from this evidence (qualitative findings are not effect sizes). Surface ethical considerations the data raised that were not anticipated.

### Conclusion
Restate what the study has and has not shown. Implications for practice, policy, and further research. Avoid ending on inflated claims about AI's promise.

## Style rules

- **Citations.** Inside sentences. `Scarparolo and Porta (2025) argue that...` or `(Scarparolo & Porta, 2025)`. Three or more authors: `Bower et al. (2025)`. Group of same-parenthetical citations: alphabetical, semicolon-separated.
- **Quotations.** Direct quotes ≤40 words: in-text with single quotes (British style) and page number. Longer: indented block, no quote marks, page number after final punctuation.
- **Lists.** Use prose. Numbered or bulleted lists belong only in methods (inclusion criteria, interview protocol summary) or appendices. Never in introduction, findings narrative, or discussion.
- **Tense.** Past tense for what participants said and what prior studies reported (`Smith (2023) found...`). Present tense for established theoretical claims and for descriptions of the present study's argument.
- **Hedging.** Use modal hedges (`may`, `appears to`, `suggests`) wherever a claim exceeds the evidence. Strong claims require strong evidence; qualitative evidence rarely warrants `proves`, `demonstrates`, or `shows that all teachers`.
- **AI vocabulary to avoid.** Reject "leverage", "delve into", "navigate the landscape", "in today's rapidly evolving", "revolutionise", "transform", "unlock potential", "unprecedented", "robust", "seamless", "harness". When found, replace with specific verbs that name the action.
- **Negative parallelism cliché to avoid.** "It is not just X, it is Y" — name what is happening directly instead.

## Working with generative AI as a topic

This skill is often used to write *about* generative AI in education. Apply extra care:
- Frame teacher use of AI as a decision, not an inevitability.
- Pair every claim about an affordance with the matching constraint or ethical consideration the literature has flagged.
- Distinguish what the technology *does* from what teachers *do with it*. Avoid agentic phrasing ("AI personalises learning") where the actor is actually the teacher mediating the tool.
- Treat policy documents (e.g. AU Framework, school-level guidance) as primary sources, not background colour.

## Quick QA checklist before delivering a section

- [ ] Every empirical claim has a citation or `[citation needed]` marker.
- [ ] No invented authors, years, titles, or DOIs.
- [ ] No promotional or inflated language about AI.
- [ ] British English throughout.
- [ ] APA 7 in-text citation format used consistently.
- [ ] Paragraphs flow as connected prose; no orphan bullet points.
- [ ] Researcher voice and hedging preserved where present.
- [ ] Section closes by linking forward, not by summarising itself.
