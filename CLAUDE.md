# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

This plugin bundles ten skills for a doctoral qualitative education-research project on **Australian secondary teachers' experiences of using generative AI to differentiate for diverse learning needs** (RQ1–RQ3). The job of this file is to route work to the right skill and to keep the skills consistent with each other.

## Routing rules

When a request matches one of the patterns below, invoke the named skill. When more than one applies, follow the chain. Do not silently merge skill responsibilities.

| The user is doing... | Skill to use |
|---|---|
| Searching, mapping, or synthesising literature across databases | `literature-review` |
| Anything involving references, APA 7 citations, or source claims — including verifying that a citation says what the draft claims it says | `citation-verification` (run *before* a citation enters any draft) |
| Drafting a specific proposal or thesis section from outline + sources | `section-writing-agent` |
| Improving qualitative academic prose, switching to British English, applying APA 7, preserving the researcher's voice | `qualitative-academic-writing` |
| Coding interview transcripts, developing categories or themes, selecting quotes, writing reflexive memos and trustworthiness notes | `qualitative-findings-analysis` |
| Designing methodology — paradigm, descriptive vs. interpretive phenomenology, reflexive thematic analysis, sampling, semi-structured interviews, ethics, trustworthiness, reflexivity, limitations, alignment | `research-methodology-skill` |
| Wanting honest, supportive feedback before supervision or before sending a draft to supervisors | `supervisor-review` |
| Polishing drafted prose to reduce generic AI writing patterns | `writing-anti-ai` (run *after* drafting, before final review) |
| Full pre-submission quality audit on a complete proposal or chapter | `paper-self-review` |
| Drafting a response to formal reviewer, examiner, or supervisor comments | `review-response` (only for formal written-comment letters, not for live supervisor feedback) |

## Common chains

- **Drafting a new section.**
  `literature-review` → `citation-verification` → `section-writing-agent` → `qualitative-academic-writing` → `writing-anti-ai` → `supervisor-review`

- **Designing/writing the methodology chapter.**
  `research-methodology-skill` (decisions and wording) → `qualitative-academic-writing` (polish) → `citation-verification` (methodologists cited) → `supervisor-review`

- **From interview data to Findings prose.**
  `qualitative-findings-analysis` (codes, themes, quotes, memos) → `qualitative-academic-writing` (Findings prose) → `citation-verification` (any literature woven in) → `supervisor-review`

- **Pre-submission of full proposal or chapter.**
  `paper-self-review` → fixes → `writing-anti-ai` → `supervisor-review`

- **Responding to written supervisor or examiner comments.**
  `review-response` → `qualitative-academic-writing` for any drafted revisions → `citation-verification`

## Non-negotiables across all skills

These apply to every skill in this toolkit, regardless of which one is active.

1. **British English.** `organisation`, `behaviour`, `analyse`, `centre`, `programme` (educational sense). Do not switch to US spelling silently.
2. **APA 7 citations.** Author–date in-text; reference list per APA 7 ordering.
3. **No fabricated citations, quotes, statistics, or participant data.** If a source is needed and is not in the user's Zotero library or supplied evidence, mark `[citation needed]` and stop.
4. **No overclaiming about generative AI.** Treat AI uses as emerging, contested, and context-dependent. Pair affordances with constraints and ethical considerations.
5. **Preserve the researcher's voice.** Keep hedged, exploratory, first-person reflexive phrasing intact unless the user asks otherwise.
6. **Qualitative by default.** Do not run statistical analysis or quantify themes unless the user explicitly asks. Reflexive thematic analysis is the default analytic frame; descriptive and interpretive phenomenology are the methodological alternatives the user is choosing between.
7. **Citations go through `citation-verification` before drafting.** Especially when the user is drafting the literature review, the methodology, or the discussion.

## What lives outside this toolkit

- The user's reference library is in **local Zotero**, queried via the `zotero` MCP server (Zotero desktop must be running). This toolkit does not store references.
- Project-level facts (current working directory, project overview, user role, working voice) are in the user's auto-memory at `~/.claude/projects/-Users-Shirley-Desktop-Proposal-resource/memory/`. Skills here should *read with* that memory, not duplicate it.
- For working with the actual `.docx` proposal drafts, prefer the `docx` skill; for the Obsidian vault, the `obsidian:*` skills.

## Refactor history

This toolkit was refactored from a general scientific-writing bundle:
- `scientific-writing` → `qualitative-academic-writing` (rewritten)
- `results-analysis` → `qualitative-findings-analysis` (rewritten; no statistics by default)
- `peer-review` → `supervisor-review` (rewritten; supervisor voice)
- new: `research-methodology-skill`

`literature-review`, `citation-verification`, `section-writing-agent`, `writing-anti-ai`, `paper-self-review`, and `review-response` carry their original SKILL.md content. Some reference files still contain biomedical examples — apply the routing rules and non-negotiables above to keep their use aligned with this qualitative project.
