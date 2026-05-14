---
name: qualitative-findings-analysis
description: Analyse qualitative interview data for an education-research study — initial coding, category development, theme development, quote selection, reflexive memos, and trustworthiness notes. Use when the user asks to "code interview transcripts", "develop themes", "select quotes", "write reflexive memos", or "review my coding". Designed around teachers' experiences of generative AI, differentiation, diverse learners, workload, professional judgement, affordances, constraints, and ethics. Does NOT perform statistical analysis unless explicitly requested.
tags: [Qualitative, Coding, Themes, Reflexivity, Education Research]
version: 0.3.0
---

# Qualitative Findings Analysis

Support rigorous, reflexive analysis of qualitative interview data — initial coding, category and theme development, quote selection, memo-writing, and trustworthiness notes — for an interpretive education-research study.

This skill is designed for a doctoral study of Australian secondary teachers' experiences of using generative AI to differentiate for diverse learners (RQ1–RQ3). The default methodological frame is reflexive thematic analysis (Braun & Clarke), used inside an interpretive phenomenological or constructivist paradigm.

## Scope

### What this skill does
- proposes initial codes from transcript excerpts
- groups codes into candidate categories and reviews their coherence
- develops, names, and refines themes that capture shared meaning
- selects representative quotes (with participant pseudonym and excerpt provenance) to illustrate themes
- drafts reflexive memos that surface the analyst's positionality and decision-making
- writes trustworthiness notes (credibility, dependability, confirmability, transferability) grounded in concrete actions taken
- flags areas where the data does not yet support a claim

### What this skill does NOT do
- **No statistical analysis.** No frequency counts presented as findings, no significance tests, no effect sizes, no claims of representativeness, unless the user explicitly asks for descriptive counts and accepts they are descriptive only.
- **No quantification of qualitative themes** ("8 of 12 teachers said X") unless the user explicitly requests it and the design supports it.
- **No generalisation beyond the participants.** Findings are about these teachers, in this setting, at this time.
- **No invented quotes.** Every quote must be traceable to a transcript excerpt the user has provided. If a quote is illustrative but the source is not in front of you, write `[exact quote to be inserted from <participant>]` rather than approximating.
- **No invented participants.** Use only pseudonyms the user has supplied or asked you to generate.
- **No paper-ready Findings prose.** Theme statements and analytic memos are not the same as the polished Findings chapter; hand polished prose to `qualitative-academic-writing`.

## Substantive focus for this project

This skill should be alert to — but not assume in advance — the following analytic territories that recur in the literature and may surface in interviews:

- **Differentiation as decision-making**: how teachers describe deciding *what* to differentiate, *for whom*, and *when* AI enters that decision.
- **Diverse learners**: students with disability, EAL/D learners, high-ability learners, students experiencing disadvantage, neurodivergent learners — and how teachers characterise their needs.
- **Workload and time**: AI as time-saver, time-shifter, or new source of work (prompt-crafting, output-checking).
- **Professional judgement**: where teachers describe overriding, accepting, or adapting AI outputs, and the reasoning they give.
- **Affordances**: what AI lets teachers do that they could not (or would not) do otherwise.
- **Constraints**: hallucinations, generic outputs, curriculum/context mismatch, equity-of-access concerns, school policy limits.
- **Ethical considerations**: data privacy, student consent, attribution and academic integrity, bias and stereotyping in outputs, dependency, transparency with students and parents.
- **Change over time (RQ2)**: how teachers narrate shifts in their practice — what they used to do, what they do now, what they attribute the change to.

Treat each of these as a sensitising concept, not a pre-set code. The codes must come from the data.

## Standard workflow

### 1. Orient to the data and the question

Before coding, confirm:
- which RQ(s) the current analytic pass is serving
- which transcripts (or transcript segments) are in scope
- whether this is a first pass (open / initial coding) or a later pass (refining categories, building themes, checking themes against data)
- which methodological frame is in use (default: reflexive thematic analysis)

If any of these are unclear, ask before producing codes.

### 2. Initial (open) coding

For each transcript segment:
- Generate codes that stay close to the participant's language ("in-vivo" where the phrase is striking and meaning-bearing).
- Use short, descriptive labels (3–6 words). Prefer gerunds for action codes ("checking AI output against curriculum").
- Code at the meaning unit, not the line — a meaning unit may be a sentence or a paragraph.
- Record both semantic codes (what the participant said) and latent codes (the analyst's reading of what is going on) when latent reading is warranted, marking them as such.
- Do not force every excerpt to fit an existing code. New codes are expected.

Output format for a coding pass:

```md
### Participant: Maya (pseudonym), transcript p.4, lines 88–112

> "I'll often start with what ChatGPT gives me and then strip out everything
> that won't land with my Year 9 class … the kids in the back row need
> something more concrete."

Codes:
- using AI output as a starting draft (semantic)
- adapting for specific class context (semantic)
- attending to within-class diversity (latent)
- teacher as filter for AI output (latent)

Memo: Maya frames AI as a draft generator she edits, not as a finished
product. This connects to the "professional judgement" sensitising concept;
worth comparing to <other participant> who described accepting outputs more
directly.
```

### 3. Category development

Group related codes. Categories are descriptive clusters, not yet themes.
- Review every code in the corpus for the pass.
- Cluster by shared meaning, not shared keyword.
- Name each category descriptively (e.g. "How teachers vet AI outputs before use").
- Flag codes that fit poorly anywhere — these often signal a new category or a tension.
- Record the boundary of each category: what counts in, what does not.

### 4. Theme development

Themes are interpretive — they capture a pattern of shared meaning organised around a central concept.
- A theme is not a topic summary ("Workload") but an analytic claim about a pattern ("Teachers describe AI as redistributing rather than reducing workload").
- Each candidate theme needs: a name, a one-sentence definition, the categories/codes it draws on, the range of participants whose data it speaks to, and the data that does *not* fit (negative cases).
- Test each theme against the data: re-read excerpts, check whether the theme still holds, refine or split as needed.
- Distinguish overarching themes from sub-themes only when the structure earns it; do not force hierarchy.

Theme template:

```md
### Theme: Teachers as filters, not consumers

**Definition.** Participants positioned themselves as professionals who edit,
adapt, or reject AI outputs in light of their knowledge of specific students,
rather than as users who apply AI suggestions directly.

**Drawn from categories:** vetting AI outputs; adapting for class context;
overriding AI on curriculum fit.

**Participants represented:** Maya, Daniel, Priya, Sam (4/10).

**Negative case:** Lina described accepting outputs with minimal editing for
low-stakes tasks; treat as boundary condition rather than disconfirmation.

**Relation to RQ:** Speaks primarily to RQ1 (how teachers use AI to
differentiate) and RQ3 (constraints around output quality).

**Open question:** Does this filtering stance shift over time? Compare to
RQ2 data on practice change.
```

### 5. Quote selection

Select 2–4 quotes per theme. Criteria:
- **Illustrative power**: the quote shows the theme in action without needing heavy gloss.
- **Range**: across the theme's participants where possible, not all from one voice.
- **Provenance**: every quote tagged with pseudonym + transcript locator (page/line or timestamp).
- **Fidelity**: light editing only (`[…]` for elision, `[clarifying word]` for grammatical bridges); do not paraphrase a quote into being more articulate.
- **Negative case**: include at least one quote that complicates the theme where one exists.

### 6. Reflexive memo

After each substantive coding/theming pass, write a short reflexive memo (150–300 words). Cover:
- decisions made in this pass and the reasoning
- where the analyst's prior beliefs (about AI, teaching, differentiation) may have shaped what was noticed or missed
- emotional reactions to the data that may signal interpretive bias
- next analytic moves to test or extend this pass

Reflexive memos are part of the audit trail. They are not throwaway; they belong with the analysis output.

### 7. Trustworthiness notes

Record concrete actions that support trustworthiness — do not write generic claims.
- **Credibility**: member reflection (sharing themes back with participants), peer debriefing with supervisor, extended engagement.
- **Dependability**: audit trail of coding decisions, version of codebook, memo log.
- **Confirmability**: traceability from quote → code → theme → claim; reflexive memos that make the analyst's hand visible.
- **Transferability**: thick description of context (school, sector, year level, subject), so a reader can judge fit to their setting.

State what was done, not what is "ensured". Trustworthiness is demonstrated, not declared.

## Output bundle

For a substantive analytic pass, produce:

```
findings-analysis/
├── codebook.md              # codes with definitions and examples
├── categories.md            # category groupings with boundaries
├── themes.md                # candidate or refined themes (use template above)
├── quote-bank.md            # selected quotes with provenance, organised by theme
├── reflexive-memos.md       # dated memos, append-only
└── trustworthiness-notes.md # concrete actions taken
```

In read-only or audit mode (user asks to review existing coding without writing files), return the same content inline rather than creating the bundle.

## Working with sensitising concepts without forcing them

The substantive focus areas listed earlier (workload, professional judgement, ethics, etc.) are sensitising — they tell you where to look, not what to find.
- If a sensitising area is absent from the data, say so; do not invent it.
- If a sensitising area appears but in unexpected form, follow the data, not the prior expectation.
- Tag codes with the sensitising area they speak to only after coding, never before.

## Quality bar before reporting findings

- [ ] Every theme has a definition, supporting codes, participant range, and at least one negative case considered.
- [ ] Every quote is traceable to a real transcript excerpt.
- [ ] No frequency claims unless the user has asked for them.
- [ ] No generalisation beyond the participants.
- [ ] At least one reflexive memo accompanies the pass.
- [ ] Trustworthiness notes describe actions taken, not aspirations.
- [ ] Themes are interpretive claims, not topic labels.

When the analysis is ready to become written Findings, hand off to `qualitative-academic-writing`.
