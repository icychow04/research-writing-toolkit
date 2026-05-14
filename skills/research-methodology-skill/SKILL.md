---
name: research-methodology-skill
description: Design and write the methodology of a qualitative education-research study. Use when the user asks to choose between paradigms or methodologies (interpretivism, constructivism, descriptive vs. interpretive/hermeneutic phenomenology, reflexive thematic analysis), plan sampling and recruitment, design semi-structured interviews, work through ethics, articulate trustworthiness and reflexivity, state limitations, or generate proposal-ready methodology wording. Compares options before committing.
allowed-tools: Read Write Edit Bash
license: MIT license
---

# Research Methodology Skill

## Overview

Helps a doctoral candidate design and write the methodology of a qualitative education-research study, and produce proposal-ready wording for each methodological choice. Default project context: Australian secondary teachers' experiences of using generative AI to differentiate for diverse learners.

This skill is decision-support first, drafting second. Before producing wording, it surfaces the alternatives, the trade-offs, and the alignment questions that matter for the study's research questions.

Companion skills:
- `qualitative-academic-writing` — turns methodology decisions into polished prose
- `qualitative-findings-analysis` — runs the analysis the methodology specifies
- `supervisor-review` — pressure-tests the methodology before supervision
- `literature-review` / `citation-verification` — sourcing and verification

## When to use

- "Should I use descriptive or interpretive phenomenology?"
- "Help me write the methodology section."
- "How many participants is defensible?"
- "Design my semi-structured interview protocol."
- "What's my reflexivity stance?"
- "What are the limitations of my design?"
- "How do I argue for reflexive thematic analysis here?"
- "Check whether my paradigm, methodology, and methods align."

## Core principle: alignment beats labels

A methodology section is judged less on which boxes are ticked and more on whether the choices line up. Every decision must answer the question: *does this serve the research questions, given the paradigm?* Mismatches are the most common doctoral-panel critique.

Default alignment chain for this project:

```
Paradigm (interpretivist / constructivist)
  └─ Methodology (interpretive phenomenology — Heideggerian / hermeneutic
                   OR descriptive phenomenology — Husserlian
                   OR reflexive thematic analysis as standalone)
       └─ Sampling (purposive, criterion-based, possibly with snowballing)
            └─ Data generation (semi-structured interviews; possibly artefacts)
                 └─ Analysis (reflexive thematic analysis OR phenomenological
                              analysis appropriate to the chosen tradition)
                      └─ Trustworthiness, reflexivity, ethics, limitations
```

When the user changes one link, check the others.

## Decision support

### Paradigm

| Paradigm | Ontology | Epistemology | Fit for this study |
|---|---|---|---|
| Positivism | Single objective reality | Knowledge as discoverable, measurable | Poor — assumes effects to measure |
| Post-positivism | Reality exists but is imperfectly knowable | Approximation, falsification | Possible but constrains interpretive depth |
| **Interpretivism** | Multiple constructed realities | Knowledge is co-constructed through interpretation | **Strong fit** — teachers' lived experience is interpretive |
| **Constructivism** | Reality is constructed by participants in context | Meaning is built socially and individually | **Strong fit**, overlaps with interpretivism |
| Critical theory | Reality is shaped by power relations | Knowledge serves emancipation | Possible if the study foregrounds equity/power |
| Pragmatism | What works, in context | Multiple methods serving practical aims | Possible but weak for a phenomenological framing |

Default: interpretivism, with constructivist commitments named. The two are often paired in education research; the candidate should state how they understand the relationship rather than treating them as interchangeable.

### Methodology

Three commonly considered options for this study:

#### Descriptive phenomenology (Husserlian)
- Goal: describe the essential structures of the phenomenon as experienced.
- Researcher stance: bracketing (*epoché*) — set aside preconceptions to access the phenomenon afresh.
- Analysis: e.g. Colaizzi's or Giorgi's steps; produces an "essence" statement.
- **Strengths** for this study: foregrounds teachers' lived experience without imposing theory; respects participant voice.
- **Tensions** for this study: bracketing is hard to defend when the researcher is themselves an educator with strong prior views; the search for an "essence" can flatten meaningful differences across teachers, sectors, and learners.

#### Interpretive / hermeneutic phenomenology (Heideggerian / van Manen / Smith's IPA)
- Goal: interpret the meaning of the experience, recognising the researcher as part of the interpretation.
- Researcher stance: reflexive engagement — preconceptions are made visible and worked with, not bracketed away.
- Analysis: iterative hermeneutic circle; or IPA's idiographic case-then-cross-case approach.
- **Strengths** for this study: lets the researcher's situatedness in Australian secondary education become an analytic resource; preserves nuance across participants.
- **Tensions** for this study: harder to bound the analysis; requires sustained reflexive memoing.

#### Reflexive thematic analysis (Braun & Clarke) — as standalone methodology
- Goal: identify and interpret patterns of shared meaning across data, with the researcher's subjectivity treated as a resource.
- Researcher stance: reflexive engagement; themes are produced, not discovered.
- Analysis: six recursive phases.
- **Strengths** for this study: flexible, well-documented, aligns naturally with interpretivism; can be paired with sensitising concepts without becoming framework-driven.
- **Tensions** for this study: not a phenomenology — does not centre lived experience qua experience; the candidate must decide whether phenomenological framing is essential.

**Comparison table for the user's decision:**

| Question | Descriptive phen. | Interpretive phen. | Reflexive TA |
|---|---|---|---|
| Centres lived experience? | Yes (essence) | Yes (meaning) | Indirectly (patterns) |
| Treats researcher as resource? | No (bracketing) | Yes | Yes |
| Best with small, deep sample? | Yes | Yes | Yes (but flexible) |
| Best with cross-case patterns? | Weak | Moderate (IPA) | Strong |
| Requires phenomenological tradition fluency? | High | High | Moderate |
| RQ fit if RQs ask "How do teachers experience..."? | Strong | Strong | Moderate |
| RQ fit if RQs ask "What changes over time..."? | Weak | Strong | Strong |

Surface this comparison when the user is choosing; do not pre-empt the choice.

### Sampling and recruitment

- **Strategy**: purposive, criterion-based. Criteria for this study typically include: currently teaching secondary in ACT; using generative AI for differentiation; at least one term of sustained use; teaching across a range of subjects/sectors to support transferability.
- **Sample size**: for reflexive TA with semi-structured interviews, 10–15 participants is defensible; for IPA, 6–10. Justify against the chosen methodology and the depth of engagement, not against quantitative power.
- **Saturation language**: Braun & Clarke argue against "data saturation" in reflexive TA — it imports a positivist logic. Use "information power" (Malterud et al., 2016) or argue from depth-of-engagement and analytic sufficiency instead.
- **Recruitment**: gatekeeper approval (school leadership, sector body); professional networks; snowballing; pre-screening for inclusion criteria; clear opt-in consent process.
- **Equity in recruitment**: deliberate effort to include teachers across public/Catholic/independent sectors, subject areas, and career stages — not just those most enthusiastic about AI.

### Semi-structured interviews

- **Duration**: 60–90 minutes; one interview per participant unless the design calls for follow-up.
- **Mode**: in-person or video; record audio with consent; professional or AI-assisted transcription with researcher verification.
- **Protocol design**:
  - 4–7 main questions, each with 2–3 probes.
  - Open with a grand-tour question ("Walk me through a time recently when you used AI to differentiate for a particular student or group...").
  - Move from concrete practice → reflection on practice → change over time → affordances/constraints → ethics.
  - Close with an open invitation ("Is there something I haven't asked about that matters here?").
- **Pilot**: at least one pilot interview to test the protocol; report pilot decisions in the methodology.

### Ethics

- HREC approval from the candidate's institution; describe approval pathway and any sector-level approvals (e.g. ACT Education Directorate, Catholic Education, individual independent schools).
- Informed consent: participants, school leadership where required; consent to record, transcribe, quote with pseudonym.
- Data management: secure storage, retention period, access controls, data destruction timeline; alignment with institutional and Australian Privacy Principles.
- Sensitive content handling: students are not participants but may be referred to — describe how the study protects student privacy in transcripts and reporting.
- Withdrawal: clear process and stop-point (e.g. up to the start of analysis).
- Risk of harm: low but non-zero (professional reputation, employer relations); mitigation through pseudonymisation, member reflection, and care with quote selection.

### Trustworthiness

Use the chosen vocabulary consistently. For a reflexive-TA or interpretive-phenomenology design, Lincoln & Guba's four criteria are the common frame:

- **Credibility**: peer debriefing with supervisor(s); member reflection (sharing themes with participants); sustained engagement; methodological coherence.
- **Dependability**: audit trail (codebook versions, reflexive memos, decision log); transparent reporting of analytic steps.
- **Confirmability**: traceability from quote → code → theme → claim; reflexive memos visible in the audit trail; supervisor cross-checks.
- **Transferability**: thick description of context — sector, school setting, subject, year level, participant background — so readers can judge fit.

State actions actually taken or planned; avoid generic declarations. Braun & Clarke's recent work also offers an alternative vocabulary (e.g. "quality criteria for reflexive TA") that the user may prefer — name the choice and stay consistent.

### Reflexivity

- Articulate the researcher's position: prior teaching experience, prior views on AI in education, relationships to the sector, year level, or subject area.
- Distinguish *personal*, *interpersonal*, *methodological*, and *contextual* reflexivity. State which the researcher will keep memoed and how.
- Describe how reflexivity will feed back into analytic decisions, not just sit as a stand-alone statement.
- For a researcher who is themselves an Australian secondary educator: name the insider/outsider tensions and how they will be handled.

### Limitations

Limitations should match the design, not be generic. For this study they typically include:
- Findings are bounded to the participating teachers, the time of the study, and the AU/ACT context — they are not generalisable in a statistical sense.
- The sample is shaped by self-selection: teachers willing to discuss AI use may differ from teachers who are not.
- Single-interview design limits longitudinal claims about practice change beyond what teachers themselves narrate.
- The researcher's situatedness shapes interpretation; reflexivity mitigates but does not remove this.
- Rapid policy and tool evolution: findings reflect a specific moment in a fast-moving field.

Avoid limitations that the design does not actually face (e.g. "small sample size" if the chosen methodology calls for small samples — name instead what the small sample means for the *kind* of claim that is licensed).

## Alignment check

After any methodological draft, work through this matrix and report mismatches:

| Element | Stated | Implied by other elements | Mismatch? |
|---|---|---|---|
| Paradigm | | | |
| Methodology | | | |
| Researcher stance (bracketing/reflexive) | | | |
| Sampling logic | | | |
| Sample size justification | | | |
| Data generation | | | |
| Analysis approach | | | |
| Trustworthiness vocabulary | | | |
| Limitations | | | |

If, for example, the section says "descriptive phenomenology" but the reflexivity statement embraces the researcher's prior knowledge as analytic resource, surface that tension and propose either changing the methodology label or revising the stance.

## Producing proposal-ready wording

When the user asks for wording, follow three steps:
1. Confirm the decisions on each element above (or surface the open questions).
2. Draft paragraph-by-paragraph in the order: paradigm → methodology → sampling → data generation → analysis → ethics → trustworthiness → reflexivity → limitations.
3. Hand the prose to `qualitative-academic-writing` for British English / APA 7 polish if the user wants a final pass.

Wording defaults:
- First person ("I will...") for the researcher's reflexive actions; avoid third-person ("The researcher will...") unless the user's institution requires it.
- Justify, do not just declare. Each decision sentence is followed by a "because..." or "to..." that ties it to the RQs or paradigm.
- Cite methodologists (e.g. Braun & Clarke for reflexive TA; van Manen or Smith for interpretive phenomenology; Husserl/Giorgi for descriptive phenomenology; Lincoln & Guba or Tracy for trustworthiness; Malterud et al. for information power) — but only after `citation-verification` has confirmed the sources are in the user's library.

## What this skill does not do

- Does not finalise prose style (hand off to `qualitative-academic-writing`).
- Does not search the literature (hand off to `literature-review`).
- Does not verify references (hand off to `citation-verification`).
- Does not code data or build themes (hand off to `qualitative-findings-analysis`).
- Does not produce a numerical scoring of methodology quality.

## Quality bar

- [ ] Every methodological choice is justified against alternatives, not declared.
- [ ] The paradigm → methodology → methods → analysis chain holds together.
- [ ] Sample size justification is methodologically grounded, not quantitative.
- [ ] Ethics goes beyond "HREC approval obtained" into substantive considerations.
- [ ] Reflexivity is positioned as analytic resource, not a one-off statement.
- [ ] Limitations match the design.
- [ ] No methodologists are cited until the user confirms the source is in their library.
