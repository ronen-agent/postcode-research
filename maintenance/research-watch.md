# Weekly PostCode Research Watch

This procedure governs an authorized scheduled review of new research and technical projects relevant to <https://github.com/ronen/postcode-research>. The scheduler controls timing; this file does not create or change a schedule. Paths written in backticks are relative to the repository root.

## Purpose and scope

Identify genuinely new and consequential findings that overlap the current questions in [research.md](../research.md) and the bibliography in [related-work.md](../related-work.md). Include the broader questions of understanding, directing, and supervising agent-mediated software development, rather than searching only for systems that resemble PostCode's proposed implementation.

Relevant work may concern conceptual interaction, task-adaptive representations, epistemological qualification, evidence and provenance, human oversight, sustained development, development from inception, source use, or methods for studying these activities. Education and agent-facing representations matter when they illuminate PostCode's questions; their relevance does not expand the project's immediate scope automatically.

Propose additions for human review using the `ronen-agent` GitHub account. The upstream repository is `ronen/postcode-research`; proposed changes belong on dedicated branches in the agent account's fork, with draft pull requests targeting upstream. A run may create the fork if needed. It must not write directly to upstream branches, merge a PR, or change project direction on its own. Keeping the fork current as described below is permitted.

## 1. Establish the current basis

1. Read the current root [AGENTS.md](../AGENTS.md) and this procedure from the upstream repository's default branch on GitHub and follow them. Do this explicitly even if the environment also loads repository instructions automatically.
2. Read the latest upstream default-branch versions of `research.md` and `related-work.md`. Consult `product-design.md`, `methodology.md`, `research-strategy.md`, `ROADMAP.md`, and `STATUS.md` as needed to interpret relevance and project status. Record the repository revision used. Do not rely solely on an environment's initial checkout or the chat's remembered copies.
3. Read previous watch reports, if present, under `records/research-watch/`, available previous run results in the scheduled chat, and relevant open, merged, and closed PRs in the upstream repository, including proposals from the agent's fork. PRs may contain proposals or rejection reasons not present on the default branch. Do not assume another chat's history or a laptop-local ledger is accessible.
4. Verify that the GitHub connection acts as `ronen-agent`, and check access to the essential documents, research sources, and operations needed to create or reuse a fork and publish a cross-repository PR. Do not fall back to the human's credentials or request upstream write access to overcome a limitation. If essential access fails, report the specific limitation and required action; do not claim a completed review or absence of relevant findings. Preserve useful partial results and distinguish them from a complete review.

For a chat using the GitHub connector, include an explicit instruction in the saved schedule prompt to read `AGENTS.md` and `maintenance/research-watch.md` on every run.

## 2. Search and screen

Search academic papers, preprints, and credible technical projects using primary publication and project sources. Follow citations and relevant earlier work when a new finding reveals an important gap. This is a selective research watch, not a systematic literature review or an exhaustive novelty assessment.

Use the last recorded successful coverage date with a seven-day overlap to accommodate indexing delays. For the first run, or when no reliable coverage date is available, start with the preceding fourteen days and disclose the limited baseline. If an earlier report provides a reliable date, extend coverage from that date rather than silently skipping a gap. Record the actual date range searched. Older newly discovered work may be included when consequential, but label it as newly found rather than newly published.

For each promising candidate:

- Verify its identity, authors or maintainers, date, publication status, and stable identifier or canonical URL. Distinguish publication dates from update and discovery dates.
- Compare against the bibliography, earlier reports, and PR history using DOI, arXiv identifier, repository URL, title, authors, and substantive content. A renamed paper, conference version, or new project release is not automatically a new finding.
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

Make changes to other research documents only where the finding directly requires an attribution, qualification, or consistency correction. Put larger changes to research scope, methodology, product design, or priorities in the PR's recommendations for human decision.

For a run with actionable findings, include a report at `records/research-watch/YYYY-MM-DD.md` in the proposal branch, adding a descriptive suffix if necessary to avoid a collision. Record the run date and timezone, baseline revision, search coverage and principal searches/sources, findings, duplicate checks, proposed changes, and limitations. Record consequential exclusions or rejected near-matches when useful to prevent repeated investigation; do not log every search hit. Link relevant earlier reports and PRs. Prior reports are historical evidence; add a dated correction rather than silently rewriting their original conclusions.

## 4. Publish for review

When there are actionable findings to publish, locate `ronen-agent`'s existing fork of `ronen/postcode-research`. Verify its upstream relationship rather than trusting its name. If no fork exists, create one under `ronen-agent`; normally it will be named `ronen-agent/postcode-research`. Do not overwrite an unrelated repository occupying that name. If the available tools cannot create or access the fork, report that specific setup requirement instead of changing the publication model.

Fetch or resolve the latest upstream default-branch revision on every run, even when the fork already exists. Use upstream's actual default branch name (currently `main`). Before preparing a new proposal branch, bring the corresponding fork branch up to date by fast-forwarding it when possible. If it contains divergent or fork-only work, preserve that work and create the new proposal branch directly from the latest upstream revision instead; do not reset or force-push it. If the available tools cannot establish that revision in the fork, report the limitation.

Create `research-watch/YYYY-MM-DD` in the fork from that verified upstream revision, adding a distinguishing suffix if needed. Keep existing proposal branches separate. Before publication, recheck upstream and relevant open PRs for intervening changes and duplicate proposals. If upstream has changed, reconcile and revalidate the proposal against the new revision before publishing; do not present a stale comparison as current.

Keep one coherent proposal for each finding. If an existing open watch PR already covers it, avoid opening a duplicate. Update an existing automation-owned branch only when it contains no intervening human changes and the update remains within its scope; otherwise report the overlap for review.

Verify citations, review qualifications, relative links, document consistency, and the final diff. Commit only the intended research documents and report, push the proposal branch to the agent's fork, and open a draft PR with that fork branch as the head and the upstream default branch as the base. The PR should explain the findings, their implications, proposed changes, review limitations, and any decisions needed. Link the report and primary sources. Do not include private chat context or credentials in public artifacts.

The human reviews and merges or rejects the proposal. Never merge a PR, force-push, delete branches, or modify repository settings as part of this watch. If publication fails, retain the prepared work where possible and report the failure without claiming a PR exists.

## 5. Report the outcome

When a proposal is ready, notify the human with the draft PR link and a concise account of why the findings matter and what needs review.

When there are no new consequential findings, create no branch, commit, or PR, and remain quiet. If the scheduler supports durable internal run state, record successful coverage there without a user notification. Otherwise, a future run must use the most recent accessible coverage record, accepting repeated searching rather than assuming an unrecorded interval was covered.

Notify on an actionable access or execution failure, or a decision requiring the human. Avoid repeating the same unresolved failure notification on every run unless its consequences change. An incomplete or failed run must not advance the successful coverage date.
