# research-writing-toolkit

A personal Claude Code plugin of skills for doctoral qualitative education research.
Refactored from a general scientific-writing bundle to support a study of
**Australian secondary teachers' experiences of using generative AI to
differentiate for diverse learning needs** (RQ1–RQ3).

## Skills

| Skill | Use when... |
|---|---|
| `literature-review` | Searching, mapping, or synthesising literature across academic databases |
| `citation-verification` | Any time references, APA 7 citations, or source claims are involved — before they enter a draft |
| `section-writing-agent` | Drafting a specific proposal or thesis section from outline + sources |
| `qualitative-academic-writing` | Improving qualitative academic prose, applying British English and APA 7, fixing AI-style writing patterns while preserving the researcher's voice |
| `qualitative-findings-analysis` | Coding interview transcripts, building categories and themes, selecting quotes, writing reflexive memos and trustworthiness notes — qualitative only, no statistics |
| `research-methodology-skill` | Designing methodology — paradigm, phenomenological options, reflexive thematic analysis, sampling, semi-structured interviews, ethics, trustworthiness, reflexivity, limitations, and alignment |
| `supervisor-review` | Honest, supportive, supervisor-style feedback before supervision meetings or before sending drafts |
| `writing-anti-ai` | After drafting, to reduce generic AI writing patterns (inflated symbolism, promotional language, AI vocabulary) |
| `paper-self-review` | Before submitting a complete proposal or chapter draft — full quality audit |
| `review-response` | Drafting responses to formal reviewer, examiner, or supervisor comments — letter-style |

## Routing at a glance

```
need sources                 → literature-review
need to verify a source      → citation-verification
need to write a section      → section-writing-agent  → qualitative-academic-writing (polish)
need to code data            → qualitative-findings-analysis
need methodology wording     → research-methodology-skill
need a check pre-meeting     → supervisor-review
need to humanise AI prose    → writing-anti-ai
need a full pre-submit audit → paper-self-review
need a rebuttal letter       → review-response
```

For more detailed routing rules, see [`CLAUDE.md`](CLAUDE.md).

## What changed in this refactor

- `scientific-writing` → **`qualitative-academic-writing`**: removed IMRAD/biomedical assumptions; defaults to British English and APA 7; refuses to invent citations; pushes back on overclaiming about generative AI.
- `results-analysis` → **`qualitative-findings-analysis`**: removed statistical analysis as a default behaviour; rebuilt around reflexive thematic analysis, quote selection, reflexive memos, and trustworthiness; substantively oriented to teacher AI use and differentiation.
- `peer-review` → **`supervisor-review`**: shifted from formal reviewer voice to supportive supervisor voice; structured around what a doctoral supervisor would say in the next meeting.
- **New: `research-methodology-skill`** — paradigm, phenomenology (descriptive vs. interpretive), reflexive thematic analysis, sampling, interviews, ethics, trustworthiness, reflexivity, limitations, and alignment checking, with proposal-ready wording.

Subsequent clean-up pass:

- `section-writing-agent` — rewritten for drafting qualitative proposal and thesis sections one at a time, in flowing prose, from a verified outline and verified sources. LaTeX/ML pipeline content removed.
- `paper-self-review` — rewritten as a doctoral self-review checklist covering alignment, research questions, literature review coherence, qualitative methodology, claim audit (with explicit AI-overclaim watch), and APA 7 / British English surface conformance.
- Legacy biomedical, IMRAD, statistical, ML, LaTeX scientific-report, and schematic-generation files removed from `qualitative-academic-writing`, `qualitative-findings-analysis`, `supervisor-review`, `section-writing-agent`, and `paper-self-review`.

`citation-verification`, `writing-anti-ai`, and `review-response` remain unchanged; the routing rules in `CLAUDE.md` keep their use aligned with this study.

## Install (Claude Code CLI)

```
/plugin marketplace add <git-url-or-local-path>
/plugin install research-writing-toolkit@research-writing-toolkit
```

Or copy/symlink the contents of `skills/` into `~/.claude/skills/`.

## Attribution

Originally bundled from upstream MIT-licensed sources. The renamed skills have
been substantially rewritten for qualitative doctoral education research.
Original copyrights and licences remain with their respective authors.

- Original `literature-review`, `scientific-writing`, `peer-review` —
  [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills)
- Original `citation-verification`, `results-analysis`, `writing-anti-ai`,
  `paper-self-review`, `review-response` —
  [Galaxy-Dawn/claude-scholar](https://github.com/Galaxy-Dawn/claude-scholar)
- Original `section-writing-agent` —
  [Ar9av/PaperOrchestra](https://github.com/Ar9av/PaperOrchestra)
