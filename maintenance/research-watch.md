# PostCode Research Watch

This procedure defines how to review research and technical projects relevant to PostCode and prepare findings and proposed document changes. It can be used for a scheduled or manual review. Paths written in backticks are relative to the repository root.

## Purpose and scope

Identify genuinely new and consequential findings that overlap the current questions in [research.md](../research.md) and the bibliography in [related-work.md](../related-work.md). Include the broader questions of understanding, directing, and supervising agent-mediated software development, rather than searching only for systems that resemble PostCode's proposed implementation.

Relevant work may concern conceptual interaction, architectural representations, epistemological qualification, evidence and provenance, human architectural judgment, sustained development, development from inception, code-independent practice, or methods for studying these activities. Education and agent-facing representations matter when they illuminate PostCode's questions; their relevance does not expand the project's immediate scope automatically.

Prepare proposed additions and corrections for human review. Do not treat a review as authorization to change the project's direction.

## 1. Establish the current basis

1. Read the current `research.md` and `related-work.md`. Consult `product-design.md`, `methodology.md`, `research-strategy.md`, `ROADMAP.md`, and `STATUS.md` as needed to interpret relevance and project status. Record the document revision or version used and any limitations on its currency.
2. Read previous reports under `records/research-watch/`, other available run records, and pending, accepted, or rejected proposals and their review decisions. These may contain findings or rejection reasons absent from the current bibliography. State any gaps in access to this history rather than assuming another chat or local record is available.
3. Verify access to the essential research documents and research sources. If essential access fails, identify the limitation and preserve useful partial results. Do not describe an incomplete review as completed or as establishing that no relevant findings exist.

Treat [historical-handover.md](../records/research-watch/historical-handover.md) as a retrospective record for deduplication and follow-up, not independently verified evidence. Its preparation date does not establish a successful search date or coverage interval. Reconcile its historical assessments and unknown integration statuses with current research documents and proposal history.

## 2. Search and screen

Search academic papers, preprints, and credible technical projects using primary publication and project sources. Follow citations and relevant earlier work when a new finding reveals an important gap. This is a selective research watch, not a systematic literature review or an exhaustive novelty assessment.

Use the last recorded successful coverage date with a seven-day overlap to accommodate indexing delays. For the first run, or when no reliable coverage date is available, start with the preceding fourteen days and disclose the limited baseline. If an earlier report provides a reliable date, extend coverage from that date rather than silently skipping a gap. Record the actual date range searched. Older newly discovered work may be included when consequential, but label it as newly found rather than newly published.

For each promising candidate:

- Verify its identity, authors or maintainers, date, publication status, and stable identifier or canonical URL. Distinguish publication dates from update and discovery dates.
- Compare against the bibliography, earlier reports, and proposal history using DOI, arXiv identifier, repository URL, title, authors, and substantive content. A renamed paper, conference version, or new project release is not automatically a new finding.
- Revisit known work only when new evidence materially changes the comparison; explain what changed. Respect previous rejection reasons unless new evidence warrants reconsideration.
- Read enough primary material to support the proposed comparison and state exactly what was inspected. An inaccessible full paper can remain a qualified lead; do not infer its methods or results from a title or snippet.
- Separate reported features from implemented capabilities, demonstrated guarantees, and evidence of human usefulness. Compare PostCode's actual claims with the work's actual scope.

Report a candidate only if it materially affects a research question, a plausible contribution, an evaluation method, or a concrete opportunity for closer investigation or reuse. General AI news, weak keyword overlap, and routine releases do not meet this threshold.

## 3. Prepare proposed changes

For each consequential finding, record:

- Citation, stable link or identifier, publication status, and relevant dates.
- Review basis and remaining uncertainties.
- Specific overlap with PostCode, with references to the relevant research questions or design claims.
- Implications for apparent novelty: what is shared, what distinction remains untested, and what the available evidence cannot establish.
- Whether closer investigation is warranted and a concrete next step. Assess infrastructure reuse and comparison of human-facing workflows separately where relevant.

Add or revise entries in `related-work.md` using its existing style, including review-basis notes. Keep provisional leads explicitly provisional. Propose corrections to positioning statements when supported by the evidence; do not invent a stronger distinction to preserve a novelty claim.

Make changes to other research documents only where the finding directly requires an attribution, qualification, or consistency correction. Put larger changes to research scope, methodology, product design, or priorities in the report as recommendations for human decision.

For a run with actionable findings, include a report at `records/research-watch/YYYY-MM-DD.md`, adding a descriptive suffix if necessary to avoid a collision. Record the run date and timezone, baseline revision, search coverage and principal searches/sources, findings, duplicate checks, proposed changes, and limitations. Record consequential exclusions or rejected near-matches when useful to prevent repeated investigation; do not log every search hit. Link relevant earlier reports and proposals. Prior reports are historical evidence; add a dated correction rather than silently rewriting their original conclusions.

## 4. Validate and record the outcome

Verify citations, review qualifications, consistency with the current research documents, and the proposed edits. State what was checked and what remains uncertain. Distinguish historical assessments from new evidence and interpretation.

For a completed review, record the actual search coverage and whether there were consequential findings. When there are none, return that outcome without manufacturing a finding or a document change. If no durable coverage record is available to a later review, use the most recent accessible record and accept repeated searching rather than assuming an unrecorded interval was covered.

An incomplete or failed review must not advance the successful coverage date. Identify unresolved access limitations, partial coverage, and any decision needed to continue. Publication and notification are handled by the invoking workflow.
