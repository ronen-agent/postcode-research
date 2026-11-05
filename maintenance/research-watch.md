# PostCode Research Watch

This procedure defines how to review research and technical projects relevant to PostCode and prepare findings and proposed document changes. It can be used for a scheduled or manual review. Paths written in backticks are relative to the repository root.

## Purpose and scope

Identify genuinely new and consequential findings that overlap the current questions in [research.md](../research.md) and the bibliography in [related-work.md](../related-work.md). Assess relevance to the current architectural-practice questions, including work that challenges PostCode's hypotheses or improves a capable conversational baseline, rather than searching only for systems that resemble its implementation.

Use the three analytic levels in [research.md](../research.md#specialized-architectural-expertise) and [methodology.md](../methodology.md#3-evaluating-projection-capabilities) to assess relevance: direct human investigation, architectural-account quality, and contribution to collaborative architectural practice. A finding may matter at any one level; evidence at one level does not establish the others. These are not mandatory efficacy endpoints. Assess contributions against the [likely contribution model](../research.md#likely-contribution-model), including the [design knowledge that construction and formative use can support](../methodology.md#6-from-formative-evidence-to-design-knowledge).

Search directions include architectural investigation and judgment; design alternatives, trade-offs and rationale; retained, revisable accounts and multiple perspectives; comparison of implemented, hypothetical and intended architecture; evidence and uncertainty; and sustained, source-independent practice. Include specialized investigation used by external agents as well as human-facing environments. Education, agent representations, and cross-paradigm work are relevant when they illuminate current questions, without turning exploratory notes or adjacent topics into adopted commitments.

Prepare proposed additions and corrections for human review. Do not treat a review as authorization to change the project's direction.

## 1. Establish the current basis

1. Read the current `research.md`, `product-design.md`, `methodology.md`, and `related-work.md`. Consult `research-strategy.md`, `ROADMAP.md`, `STATUS.md`, and relevant exploratory notes as needed to interpret relevance and project status. Record the document revision or version used and any limitations on its currency.
2. Read previous reports under `records/research-watch/`, other available run records, and pending, accepted, or rejected proposals and their review decisions. These may contain findings or rejection reasons absent from the current bibliography. State any gaps in access to this history rather than assuming another chat or local record is available.
3. Verify access to the essential research documents and research sources. If essential access fails, identify the limitation and preserve useful partial results. Do not describe an incomplete review as completed or as establishing that no relevant findings exist.

Integration of a proposal establishes that its contents entered the repository, not that a human independently verified its sources or endorsed each comparison. Preserve review-basis qualifications and distinguish recorded substantive review decisions from publication or merge status.

Treat [historical-handover.md](../records/research-watch/historical-handover.md) as a retrospective record for deduplication and follow-up, not independently verified evidence. Its preparation date does not establish a successful search date or coverage interval. Reconcile its historical assessments and unknown integration statuses with current research documents and proposal history.

## 2. Search and screen

Search academic papers, preprints, and credible technical projects using primary publication and project sources. Follow citations and relevant earlier work when a finding or change in PostCode's framing reveals an important gap. Include established architecture and human–computer interaction literature where relevant; do not require coding-agent terminology or recent publication. After a material reframing, make a bounded reassessment of affected entries and previously screened leads, recording what was reconsidered so later weekly runs need not repeat it. This is a selective research watch, not a systematic literature review or an exhaustive novelty assessment.

Use the last recorded successful coverage date with a seven-day overlap to accommodate indexing delays. For the first run, or when no reliable coverage date is available, start with the preceding fourteen days and disclose the limited baseline. If an earlier report provides a reliable date, extend coverage from that date rather than silently skipping a gap. Record the actual date range searched. Older newly discovered work may be included when consequential, but label it as newly found rather than newly published.

For each promising candidate:

- Verify its identity, authors or maintainers, date, publication status, and stable identifier or canonical URL. Distinguish publication dates from update and discovery dates.
- Compare against the bibliography, earlier reports, and proposal history using DOI, arXiv identifier, repository URL, title, authors, and substantive content. A renamed paper, conference version, or new project release is not automatically a new finding.
- Revisit known work when new evidence or a material change in PostCode's research framing changes its relevance or comparison. Explain that change, distinguish reassessment from a new publication, and retain prior rejection reasons unless the changed basis addresses them.
- Read enough primary material to support the proposed comparison and state exactly what was inspected. An inaccessible full paper can remain a qualified lead; do not infer its methods or results from a title or snippet.
- Separate reported features from implemented capabilities, demonstrated guarantees, and evidence of human usefulness. Compare PostCode's actual claims with the work's actual scope. Lack of a human-interface evaluation limits human-usefulness claims but does not exclude consequential design knowledge, account-quality methods, baselines, or evaluation material.
- Identify design requirements, rationale, implementation insights, mechanisms, tensions, and failures that bear on PostCode. Distinguish proposed principles from lessons supported by construction or use; record their context, evidence, contrary cases, and limits on transfer. A prototype or experience report is neither automatically a contribution nor disqualified by lacking a comparative study.
- Apply the [comparison rules](../methodology.md#84-comparisons-and-reuse-assessments): identify the baseline's tools, repository access, diagrams, retained context, and assistance. Record human programming experience separately from human source exposure and agent source access; source-independent use by experienced programmers does not establish practice without programming expertise. Distinguish factual account quality, reference agreement, participant perception, and design outcomes.

Report a candidate only if it materially affects a research question, a plausible contribution, a design or evaluation method, or a concrete opportunity for closer investigation or reuse. General AI news, weak keyword overlap, and routine releases do not meet this threshold. Methodological literature warrants inclusion when it addresses a concrete PostCode evidence or contribution question; this is not a general research-methods watch.

## 3. Prepare proposed changes

For each consequential finding, record:

- Citation, stable link or identifier, publication status, and relevant dates.
- Review basis and remaining uncertainties.
- Specific overlap with PostCode, with references to the relevant research questions or design claims and the analytic level(s) informed where applicable. Explain what can be learned from the work as well as which stronger conclusions are not supported.
- Implications for apparent novelty at the level of problem formulation, design rationale, mechanisms, and lessons as well as features and outcomes: what is shared, what distinction remains untested, and what the available evidence cannot establish. Established components can support new design knowledge; established lessons still require attribution.
- Whether closer investigation is warranted and a concrete next step. Assess infrastructure reuse, architectural-account evaluation, and comparison of human-facing or collaborative workflows separately where relevant.

Add or revise entries in `related-work.md` using its existing style, including review-basis notes. Keep provisional leads explicitly provisional. Propose corrections to positioning statements when supported by the evidence; do not invent a stronger distinction to preserve a novelty claim.

Make changes to other research documents only where the finding directly requires an attribution, qualification, or consistency correction. Put larger changes to research scope, methodology, product design, or priorities in the report as recommendations for human decision.

For a run with actionable findings, include a report at `records/research-watch/YYYY-MM-DD.md`, adding a descriptive suffix if necessary to avoid a collision. Record the run date and timezone, baseline revision, search coverage and principal searches/sources, findings, duplicate checks, proposed changes, and limitations. Record consequential exclusions or rejected near-matches when useful to prevent repeated investigation; do not log every search hit. Link relevant earlier reports and proposals. Prior reports are historical evidence; add a dated correction rather than silently rewriting their original conclusions.

## 4. Validate and record the outcome

Verify citations, review qualifications, consistency with the current research documents, and the proposed edits. State what was checked and what remains uncertain. Distinguish historical assessments from new evidence and interpretation.

For a completed review, record the actual search coverage and whether there were consequential findings. When there are none, return that outcome without manufacturing a finding or a document change. If no durable coverage record is available to a later review, use the most recent accessible record and accept repeated searching rather than assuming an unrecorded interval was covered.

A targeted reassessment does not advance the recurring search-coverage checkpoint unless it also completes and records the required date-window search. Record its scope separately so a later weekly run does not silently skip an interval.

An incomplete or failed review must not advance the successful coverage date. Identify unresolved access limitations, partial coverage, and any decision needed to continue. Publication and notification are handled by the invoking workflow.
