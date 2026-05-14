---
name: section-writing-agent
description: Draft a specific section of a qualitative education research proposal or thesis from an outline plus verified sources and (where applicable) interview data. Use when the user asks to "draft my [introduction / context / literature review / theoretical framework / methodology / findings / discussion / conclusion] section". Works one section at a time, in flowing prose, in British English with APA 7. Never invents citations. Hands off polish to qualitative-academic-writing and humanising to writing-anti-ai.
allowed-tools: Read Write Edit Bash
license: MIT license
---

# Section Writing Agent

## Overview

Draft a single section of a research proposal or doctoral thesis in qualitative education research. The deliverable is **flowing prose, one section at a time**, anchored in an outline the user has approved and in sources the user has verified.

This skill is the section-by-section drafter for the project on **Australian secondary teachers' experiences of using generative AI to differentiate for diverse learners** (RQ1–RQ3). It is not a manuscript pipeline, does not produce LaTeX, and does not draft an entire paper in one pass.

Companion skills:
- `literature-review` — finds sources before drafting
- `citation-verification` — confirms every source is real and says what is claimed
- `research-methodology-skill` — decisions and wording for the methodology section
- `qualitative-findings-analysis` — codes, themes, quotes that feed the findings section
- `qualitative-academic-writing` — stylistic polish after the draft is in place
- `writing-anti-ai` — strips generic AI writing patterns
- `supervisor-review` — pressure-tests the section before supervision
- `paper-self-review` — final pre-submission audit on a full draft

## When to use

Trigger when the user asks to:
- "draft the [section] section"
- "write a first draft of [section] from my outline"
- "expand this outline into prose"
- "produce a section draft I can take to my supervisor"

Do not trigger for:
- searching for sources → `literature-review`
- coding interview data → `qualitative-findings-analysis`
- deciding methodology → `research-methodology-skill`
- polishing existing prose → `qualitative-academic-writing`

## Inputs required before drafting

Refuse to start without these. If any are missing, ask for them before producing prose.

1. **Which section.** One of: background and context; problem statement and significance; literature review (or a named subsection); theoretical framework; research questions; methodology (or a named subsection); findings (or a named theme); discussion; conclusion.
2. **The outline.** Paragraph-level scaffolding with claims, evidence anchors, and the RQ(s) each paragraph serves. If the user has not produced one, prompt them or call out that one is needed.
3. **The verified sources.** Author–year keys plus the actual evidence (page numbers, key claims) the user wants drawn on. Sources must already have been passed through `citation-verification`. If not, stop and route there first.
4. **For a findings section:** the themes, quotes (with pseudonym + transcript locator), and reflexive memos from `qualitative-findings-analysis`.
5. **The target length.** A word count or page count. Drafts without a target tend to balloon.
6. **The audience.** Confirmation panel, supervisor, examination committee, journal — each shifts tone and depth.

## Non-negotiables

1. **One section per call.** Do not draft "the rest of the paper" in one pass. Cohesion across sections is the user's job (and `supervisor-review`'s).
2. **No invented citations.** If a paragraph in the outline points to a citation the user has not verified, stop at that paragraph and surface the gap. Do not approximate, do not insert a placeholder DOI, do not assume the source.
3. **No invented data.** No invented participant quotes, pseudonyms, school details, or statistics. If the outline calls for a quote you do not have, write `[exact quote to be inserted from <participant>]` and continue.
4. **British English.** APA 7. First person where the methodology supports it.
5. **No overclaiming about generative AI.** Treat AI uses as emerging, contested, context-dependent. Pair every affordance with a constraint or ethical consideration.
6. **Preserve the researcher's voice.** Keep hedging and exploratory phrasing where the outline carries them. Do not flatten to confident generalisations.
7. **No bullet points in the deliverable.** Prose only. Lists belong to the outline, not the section.

## Drafting workflow

### 1. Read the outline and the sources

Internally walk through the outline paragraph by paragraph. For each:
- Confirm the claim is one move, not three.
- Confirm the evidence anchor is in the user's verified set.
- Note any tensions or counter-evidence the user has flagged.
- Note which RQ(s) the paragraph serves.

If the outline is thin, ask for more before drafting.

### 2. Draft section opening

Open with a sentence that names the move the section makes, not a generic preamble. Avoid:
- "In today's rapidly evolving educational landscape..."
- "Generative AI has transformed education in unprecedented ways..."
- "This section will explore..."

Prefer:
- "Differentiated instruction in Australian secondary schools sits between policy commitment and uneven enactment (Scarparolo & Porta, 2025)."
- "I take an interpretive phenomenological approach because the study's aim is to understand teachers' lived experience, not to measure outcomes."

### 3. Draft body paragraphs

For each outline point:
- Topic sentence states the move.
- Evidence is integrated inside sentences (`Bower et al. (2025) found that...`), not parked at the end as a citation list.
- Transitions name logical relations (`however`, `by contrast`, `building on this`); avoid empty connectives.
- Hedges (`may`, `appears to`, `suggests`) where the evidence is partial.
- Vary sentence length. Short sentences carry emphasis; long sentences carry argument.

### 4. Draft section close

The close should link forward — to the next section, to the analytic move ahead, to the question the section opens up. Do not end with a "this section has shown..." summary of itself.

### 5. Surface gaps

At the end of the draft, list:
- Any `[citation needed]` markers and what claim they sit under.
- Any `[exact quote to be inserted]` markers and the participant they belong to.
- Any outline points you could not draft and why.
- Any claims you weakened relative to the outline (to avoid overclaiming) so the user can review.

## Section-specific notes

### Background and context
Locate the study in time, place, policy. Name the jurisdiction (ACT), sector(s), and relevant policy instrument (e.g. Australian Framework for Generative AI in Schools). Avoid generic openings about "the rise of AI".

### Problem statement and significance
State what is missing in current understanding, not what is happening in the world. For a qualitative study, significance lies in insight from teachers' lived practice, not in generalisability.

### Literature review (or a subsection of it)
Argue, do not summarise. Each paragraph advances a position; each subsection advances the argument that motivates the RQs. Surface tensions. Read AI-in-education literature critically — distinguish empirical findings from vendor advocacy.

### Theoretical framework
Explain how the framework will be *used* analytically — as sensitising lens, coding frame, or interpretive scaffold. Justify against alternatives the user considered. Avoid name-dropping.

### Research questions
Open, how/what questions appropriate to qualitative inquiry. Each RQ should map to an analytic move. If presenting RQs as a list inside the section is required, label them clearly; otherwise integrate into prose.

### Methodology
Order: paradigm → methodology → sampling → data generation → analysis → ethics → trustworthiness → reflexivity → limitations. Every decision sentence carries a "because..." or "to..." that ties it to the RQs. For wording defaults and alternatives, the user should have already worked with `research-methodology-skill`.

### Findings (or a single theme)
Lead with the theme statement (an interpretive claim, not a topic label). Anchor in 2–4 quotes per theme with pseudonyms and transcript locators. Interpret each quote; do not let it stand alone. Include negative cases where they exist.

### Discussion
Read findings back against the theoretical framework. Move from theme → claim → literature → so-what. Acknowledge what cannot be said. Do not import quantitative framings (effect, impact, outcome) unless the user has explicitly defended their use.

### Conclusion
Restate what the study has and has not shown. Implications for practice, policy, further research. No inflated closing claims about AI's promise.

## Handoffs

After the draft is delivered:
- Tone, register, and citation polish → `qualitative-academic-writing`
- Generic AI writing patterns → `writing-anti-ai`
- Pressure-test before supervision → `supervisor-review`
- Full-document audit before submission → `paper-self-review`

## Quality bar before delivering a section

- [ ] One section, drafted to the target length (within ±15%).
- [ ] Every empirical claim has a verified citation or a `[citation needed]` marker.
- [ ] No invented citations, quotes, participants, or data.
- [ ] No promotional or inflated language about AI.
- [ ] British English, APA 7 in-text format, prose (no bullets).
- [ ] Researcher voice and hedging preserved where the outline carries them.
- [ ] Section opens with a substantive move and closes by linking forward.
- [ ] Gaps surfaced at the end of the draft, not buried.
