# PostCode research watch — historical handover

**Handover prepared:** 2026-10-12 (Europe/London).  
**Record type:** Retrospective synthesis of research-watch messages in a ChatGPT conversation; **not** a new literature search.  
**Intended repository location:** `records/research-watch/historical-handover.md`.  
**Coverage:** Six identifiable research-watch replies, in their preserved conversational order, plus directly related bibliography discussions and later corrections. **The actual execution/report date of each reply is not recoverable from the available conversation.** Publication, announcement, issue, and preprint dates below are *source dates reported in the conversation*, not dates on which the watch ran. The handover date is not a report-run date.

## Reconstruction and evidence conventions

- No new sources were retrieved for this handover. Links, dates, findings, and characterizations below are transcribed or paraphrased from earlier watch reports and follow-up discussion. **Neither the linked source contents nor their present availability have been independently rechecked here.**
- **Inspected scope:** The watch replies generally did not preserve tool logs or exact reading depth. A report's description of a website, documentation, paper, benchmark, or repository establishes that the earlier assistant *reported information from it*, **not** that a full paper, running implementation, or whole repository was inspected. Each entry identifies what the conversational record does and does not support.
- **Bibliography state:** An uploaded snapshot of `related-work.md` (available during the conversation) already contained **CodeSkyline** and **Code2UML**. Later, an expanded bibliography was proposed in chat and a downloadable `related-work-updated.md` was supplied. The user subsequently reported taking that file to Work for integration, with Work re-examining some sources and changing other documents. **The actual repository state after Work's review is unknown here.** “Proposed” does not mean “merged.”
- Bibliographic titles/attributions may be abbreviated where that is all the watch recorded. Do not silently promote reported acceptance, precision statistics, release dates, or feature claims to verified facts.
- Research framing evolved from a read-only, source-secondary investigation tool toward a broader human conceptual interface for **understanding, directing, and supervising** agent-mediated software development, including projects developed with PostCode from inception. Later novelty assessments should use this broader scope.

## Chronology of identifiable watch reports (execution dates unknown)

| Order | Watch-report headline | Findings first raised in that report | Report date |
|---|---|---|---|
| 1 | Provenance-aware systems | SwiftUI Semantic Audit; Graphify | Unknown |
| 2 | Broad deterministic projection system | Archbird | Unknown |
| 3 | AI changes visualization economics | Merino et al. 2026; Liang et al. 2026 | Unknown |
| 4 | Agent change review and spec-driven visualization | Whiteboard (/dev/fast); Rosa et al. 2026 | Unknown |
| 5 | Provenance graph and disposable projections | Roteiro; Cygnus | Unknown |
| 6 | Agent oversight and assurance evidence | Sun et al. 2026; Ferris and Bonilla 2026 | Unknown |

The last report describes preprints dated October 5–6, 2026. That is a **lower bound on the claimed knowledge timeline**, not a recoverable execution date. No evidence establishes the precise intervals between these reports, or exhaustive coverage of any intervening period.

## Findings (consolidated; ordered by initial mention)

### 1. SwiftUI Semantic Audit — semantic architecture evidence and diffs

- **Identity:** *SwiftUI Semantic Audit*; technical project. Named maintainers not recorded.
- **Primary link supplied:** https://swiftui-audit.dev/
- **Source/publication date and status:** 2026 project; exact first-publication or version date not preserved.
- **Inspected scope evidenced by conversation:** Earlier watch report described the project's website/technical descriptions: a deterministic semantic twin of SwiftUI ownership/data flow, separation of extraction from agent judgment, semantic snapshot diffs, a watcher, freshness checks, and explicit limits of behavioral proof. Whether implementation was cloned, run, or code-reviewed is **not established**.
- **PostCode overlap:** Trustworthy source-grounded projections; epistemic distinction between architecture facts and interpretation; semantic/projection diffs for agent-authored changes; live updating and stale-data signaling; engineering supervision through higher-level evidence.
- **Assessment at first report:** *Meaningful prior art; substantial narrowing of novelty for the conjunction “deterministic facts + agent interpretation + semantic diff + explicit limits,” but not fatal to PostCode's human source-secondary, sustained-investigation question.* SwiftUI-specific; source remains a verification surface; primarily evidence for coding agents.
- **Later treatment:** Reiterated as high-priority prior art for semantics/diffs. No documented retraction or material change in judgment.
- **Suggested follow-up:** Inspect the actual implementation, exact guarantees, and what “semantic diff” compares; distinguish source-derived facts from agent-authored explanations. Test whether the mechanism could serve as a narrow comparison baseline.
- **Bibliography status:** Proposed for addition in chat; included in an assistant-generated updated bibliography; **actual Work/repository integration unknown**.

### 2. Graphify — cross-language provenance-tagged knowledge graph **(identity unresolved)**

- **Identity:** “Graphify,” described as a codebase-graph project; authors/maintainers and repository **not reliably identified**.
- **Link originally supplied:** https://graphify.com/what-is-graphify — **subsequently flagged in conversation as not clearly identifying the described code-analysis project**. Do not use as a validated primary-source citation.
- **Source/publication date and status:** Not established.
- **Inspected scope evidenced by conversation:** Initial watch reply described a claimed architecture (Tree-sitter extraction plus inferred semantic relationships; `EXTRACTED`, `INFERRED`, `AMBIGUOUS` tags; confidence; architecture reports; cross-language support), but no reliable primary-source identity or implementation inspection is recoverable.
- **PostCode overlap if identified:** Cross-language structure and semantic projections, epistemic/provenance labels, interactive architecture summaries, agent investigation without repeated source reads.
- **Assessment at first report:** Moderate novelty impact for provenance-tagged cross-language projections, but a different center of gravity (agent knowledge graph, not sustained human conceptual interface).
- **Later correction:** The supplied URL could not be reliably matched to the described project. The later consolidated bibliography explicitly **deferred** Graphify as an *unverified research lead*, not established prior art. This supersedes the initial confident characterization.
- **Suggested follow-up:** Resolve the project identity and find a real repository or primary technical publication before revisiting its claims. Avoid repeatedly rediscovering the same ambiguous brand name without new identifying evidence.
- **Bibliography status:** Proposed only as a clearly provisional/unverified lead. **Not established as a confirmed citation; current repository integration unknown**.

### 3. Archbird — deterministic cross-language architecture map and projections

- **Identity:** *Archbird*; technical software project. Maintainers not recorded in the conversation.
- **Primary links supplied:** https://archbird.org/ ; https://pypi.org/project/archbird/0.0.1/
- **Dates/status reported:** First PyPI release **2026-07-16**; watch described contemporary technical documentation, but neither a version snapshot nor date of later features was recorded. Project documentation, not established peer-reviewed validation.
- **Inspected scope evidenced by conversation:** Watch described technical documentation for deterministic language-neutral map/IR; files, symbols, dependencies, interfaces, tests, build routes, components; C/C++, Python, JavaScript/TypeScript/TSX, R; provider provenance, uncertainty and incompleteness; Query/Path and overview/architecture/test/evidence projections; browser explorer; live revisions and structural differences; differentiated per-test observation evidence. **No successful installation, source audit, or independent execution is documented.**
- **PostCode overlap:** Exceptionally broad: qualified cross-language source projections, independently chosen human views, uncertainty/freshness, evidence links, tests as differentiated evidence, repository watching, structural/projection-like diffs, exploration for humans and agents.
- **Assessment at first report:** **Significant mechanism-level novelty impact**. The broad set of underlying techniques should not be claimed as individually new. Initially distinguished from PostCode by its focus on deterministic architecture evidence, verification, and controlled structural changes, rather than whether projections become the human's sustained source-secondary working surface or whether natural-language information needs select lenses/views.
- **Later change in assessment:** Consolidation recommended treating Archbird as an **experimental baseline or possible reusable foundation**, not merely a related-work citation. This is a material prioritization change, not a repudiation of the initial overlap.
- **Suggested follow-up:** Actually install/run it on representative repositories; audit how provenance and limits appear to humans; inspect projection API/diffs/test semantics; compare its interaction workflow against PostCode's broader understand/direct/supervise questions before rebuilding similar infrastructure.
- **Bibliography status:** Repeatedly proposed as **high-priority** addition; included in an assistant-generated draft; **actual Work/repository integration unknown**.

### 4. Merino, Ghafari & Nierstrasz (2026) — AI and actionable visualization

- **Identity/title as reported:** L. Merino, M. Ghafari & O. Nierstrasz, *Towards Actionable Visualization: Ten Years Later, What Generative AI Changes and What It Cannot*.
- **Primary identifier:** https://arxiv.org/abs/2608.22151
- **Date/status reported:** Presented at VISSOFT 2026 on **2026-09-15**, according to the watch; arXiv identifier `2608.22151` indicates a 2026 preprint. Conference presentation claim was **not independently reverified for this handover**.
- **Inspected scope evidenced by conversation:** Watch described arguments and specific passages about cheap, disposable question-specific visualizations; translating vague developer questions into deterministic visualization specifications; choosing view forms; incorporating agent tool calls/intermediate results/proposed diffs in supervisory views; and faithfulness/source traceability. The record does **not** establish full-paper review or systematic assessment of evaluation evidence.
- **PostCode overlap:** Nearly direct anticipation of PostCode's “why now?” argument: reduced generation and selection cost, task-specific lenses/views, views as temporary query results, incorporation into agentic supervision, and trust/evidence.
- **Assessment at first report:** **Substantial/high novelty impact** on AI changing software-visualization economics, automatic selection of presentations, ephemeral task-specific views, and navigable visualization of agent changes. The research question of sustained source-secondary *human* development and the stronger per-claim epistemic contract appeared less directly addressed.
- **Later change in assessment:** Became an **essential introduction citation**, paired with the authors' 2018 work. It would be misleading to claim these “why now?” insights as independently novel PostCode ideas. No contrary correction recorded.
- **Suggested follow-up:** Read the whole 2026 paper beside the 2018 predecessor; identify its actual study/validation scope, if any; carefully delimit novelty in the continued-development rather than per-query visualization workflow.
- **Bibliography status:** 2018 predecessor already present in uploaded `related-work.md`. **2026 paper proposed as new entry** in chat and assistant-generated updated bibliography; **actual Work/repository integration unknown**.

### 5. Liang et al. (2026) — tests as evidence in LLM software engineering

- **Identity/title as reported:** Liang et al., *Test-Driven Approaches to Software Engineering with Large Language Models: A Survey of Phases, Tasks, and Agent Skills*.
- **Primary identifier:** https://arxiv.org/abs/2609.12012
- **Date/status reported:** **2026-09-10** preprint; a survey of **87 records** was claimed in the watch report. The count and precise scope are unverified here.
- **Inspected scope evidenced by conversation:** Watch characterized a survey/taxonomy explaining why test passing alone does not establish behavioral equivalence, validity of feedback, or process adherence. No full systematic reading documented.
- **PostCode overlap:** Tests as *qualified evidence* rather than generic proof of correctness; useful for test-intent/realization/evidence distinctions.
- **Assessment at first report:** **Low direct novelty impact**, but valuable conceptual prior art; does not propose tests as human-facing program projections.
- **Later treatment:** Proposed for test/evidence subsection; no material change or rejection recorded.
- **Suggested follow-up:** Inspect survey's taxonomy and exact claims; look for source papers that directly map test intent/behavior into human-facing views.
- **Bibliography status:** Proposed in chat and included in assistant-generated updated bibliography; **actual Work/repository integration unknown**.

### 6. Whiteboard (/dev/fast) — canvas for inspecting agent changes

- **Identity:** *Whiteboard*, attributed to `/dev/fast`; maintainers not individually named in record.
- **Primary link supplied:** https://github.com/devdotfast/whiteboard
- **Date/status reported:** Public launch **2026-09-24**; open-source project, according to watch. Specific release tag and feature dates not preserved.
- **Inspected scope evidenced by conversation:** Watch described repository/technical descriptions: read-only desktop workspace alongside Claude Code/Codex; agent-produced sequence/ER diagrams linking to source; AST-aware semantic diff, pseudocode presentation, and decision log. **Not established that repository code was thoroughly inspected or application run**.
- **PostCode overlap:** Human review through non-source representations, source-linked explanations, semantic-level diffs, separation from external coding agents, records of decisions.
- **Assessment at first report:** Significant novelty impact for the projection-diff/agent-change-review branch: representing agent changes above source level is already an implemented project direction. More change-review-centered than PostCode's ongoing program investigation; agent explanations may not have PostCode's desired epistemological guarantees.
- **Later treatment:** Recommended direct technical inspection of what is actually available and its guarantees; no reversal of assessment.
- **Suggested follow-up:** Verify feature implementations and semantics of AST-aware diff, diagram generation, human verification, and decision provenance. Consider as a comparison for change-review tasks.
- **Bibliography status:** Proposed and put in an assistant-generated updated bibliography; **actual Work/repository integration unknown**.

### 7. Rosa, Linares-Vásquez & Robles (2026) — spec-driven visualization

- **Identity/title as reported:** Rosa, Linares-Vásquez & Robles, *Re-Imagining Software Visualization for Spec-Driven Development*.
- **Primary link supplied:** https://shiftmanifesto.com/research/spec-visualization/
- **Date/status reported:** Presented at VISSOFT 2026 on **2026-09-15**, according to the watch. Preprint/publication metadata not independently established here.
- **Inspected scope evidenced by conversation:** Watch described conceptual work visualizing individual specifications, relationships, traceability into generated code, co-evolution, and integrated task-oriented workspaces. No implementation study or full-paper inspection established.
- **PostCode overlap:** Another conceptual interface centered on higher-level information rather than source, especially creation and continued development with agents; traceability and evolution of intent/implementation.
- **Assessment at first report:** Moderate novelty impact: source need not be primary is not a novel *general* thesis; specs as authoritative intent versus PostCode's derived qualified representations of actual program.
- **Later change in assessment:** After the reorganized `research.md` broadened PostCode to **directing**, **supervising**, and **ab initio** development, the assistant explicitly judged the work **more relevant than previously credited**, and cautioned that a sharp “spec vs projection” separation understates overlap. This supersedes the earlier narrow framing.
- **Suggested follow-up:** Obtain the actual paper/preprint and verify venue; study how spec/code co-evolution is handled and compare against projects where PostCode is present from inception.
- **Bibliography status:** Proposed in chat, with placement in agentic human-role literature; included in draft bibliography. **Actual Work/repository integration unknown**.

### 8. Roteiro — derived/authored/inferred program knowledge

- **Identity:** *Roteiro*; technical software project. Maintainers not recorded.
- **Primary link supplied:** https://roteiro.dev/
- **Date/status reported:** An **2026-08-15** roadmap issue reportedly used the term “lenses”; project release/publication date not established.
- **Inspected scope evidenced by conversation:** Watch described project documentation: Git/content-addressed knowledge graph, incremental generation; `derived` deterministic source facts, `authored` design rationale/annotations, `inferred` model/embedding hypotheses with confidence; structured and natural-language queries and generated views. No cloned implementation or independent run evidenced.
- **PostCode overlap:** Particularly close to PostCode's epistemological/provenance classes and navigable source-plus-rationale representations.
- **Assessment at first report:** **Significant novelty impact** on treating derived, recorded/authored, and interpreted/inferred knowledge as distinguishable queryable categories. Graph substrate serves humans and agents; PostCode still has a distinct hypothesis about sustained human working views and adaptive selection.
- **Later treatment:** Elevated alongside Archbird and Merino 2026 as one of the **central** references; not a novelty claim to list provenance types alone. No contradiction recorded.
- **Suggested follow-up:** Inspect tagging/confidence behavior and whether its epistemic qualifications actually survive human presentation at the claim level; assess its fit as a reusable evidence source.
- **Bibliography status:** Proposed and included in draft bibliography; **actual Work/repository integration unknown**.

### 9. Cygnus — append-only evidence graph and disposable views

- **Identity:** *Cygnus*, technical project “in development”; maintainers not established.
- **Primary link supplied:** https://www.river.io/cygnus/
- **Date/status reported:** 2026, exact announcement/publication date not captured; feature maturity unknown.
- **Inspected scope evidenced by conversation:** Watch described public project overview: provenance-bearing immutable observations, append-only graph, disposable projections, Swift/Python/C/Rust relationships, revisions, per-function coverage and per-test attribution. No implementation audit or run evidenced.
- **PostCode overlap:** Evidence → graph → disposable projection architecture, cross-language static relationships, test evidence linked to source, revision-specific state.
- **Assessment at first report:** Narrowed novelty for such an architecture and its test-linked projections; weaker weight than mature/published prior art because marked in development. Less explicit about per-claim epistemological guarantees and sustained source-secondary human development.
- **Later treatment:** Retained as qualified technical lead; no change in assessment documented.
- **Suggested follow-up:** Recheck maturity, source availability, actual semantics/guarantees and the distinction between announced and implemented features.
- **Bibliography status:** Proposed in chat/draft; **actual Work/repository integration unknown**.

### 10. Sun et al. (2026) — *What Did the Agent Actually Do?*

- **Identity/title:** Sun et al., *What Did the Agent Actually Do? Evidence-Grounded Oversight for Long-Horizon Agents*.
- **Primary identifier:** https://arxiv.org/abs/2610.06406
- **Date/status reported:** Paper dated **2026-10-05** in watch; preprint (peer-review/acceptance not established).
- **Inspected scope evidenced by conversation:** Watch described an Evidence-Grounded Behavior Graph (EBG), deterministic evidence extraction, semantic monitoring, source-linked behavior relationships, and a benchmark called **SilentSwap** in the earlier report; a later bibliography draft referred instead to **AgentMonBench**. **The benchmark naming/content is inconsistent in the preserved conversation and must be checked against the paper.** Watch summarized claimed model-comparison performance, but the actual experiments/methods were not reconstructed from full text here.
- **PostCode overlap:** Evidence-grounded agent supervision, task-specific evidence views, provenance links, inspecting behavior changes not exposed by passing tests.
- **Assessment at first report:** Moderate-to-significant overlap at the evidence-based monitoring mechanism level; focused on detecting consequential agent choices, not using projections as the continuously updated human conceptual interface to software.
- **Later treatment/correction:** Proposed as a high-priority benchmark/evaluation lead; **the record's SilentSwap vs AgentMonBench discrepancy is unresolved**, not silently reconciled.
- **Suggested follow-up:** Read the paper to confirm title/authors, benchmark identity, construction and eligibility for re-use; check whether scenarios actually concern code behavior and passing tests; evaluate the benchmark as a possible source of supervised-change tasks.
- **Bibliography status:** Proposed and included in assistant-generated draft; **actual Work/repository integration unknown**.

### 11. Ferris & Bonilla (2026) — assurance of AI-written software

- **Identity/title as reported:** Ferris and Bonilla, *A Case Study in Assuring AI-Written Software*.
- **Primary identifier:** https://arxiv.org/abs/2610.08651
- **Date/status reported:** Paper dated **2026-10-06** according to watch; reportedly accepted to a NeurIPS 2026 Meta-Agents Workshop. Acceptance claim unverified here.
- **Inspected scope evidenced by conversation:** Watch described a single observational healthcare-platform case study of an operator without formal SWE training using agents, tests, monitoring, independent agent review and staging. Described proxy failures, missing/omitted checks, and assurance gaps. No indication of independent verification or complete paper reading in the preserved record.
- **PostCode overlap:** Motivates non-source human supervision and a strong epistemological contract: checks are only evidence of what they truly observe, not generalized correctness claims; agent-mediated development from a human conceptual standpoint.
- **Assessment at first report:** Low direct projection-tool novelty impact, significant conceptual/methodological relevance. More than a source-inspection alternative: evidence can itself fail, so PostCode must represent what claims the evidence warrants.
- **Later treatment:** Recommended alongside tests-as-evidence survey for stronger conceptual framing; no correction or reversal recorded.
- **Suggested follow-up:** Review actual case scope, failure examples, and generalizability limits; consider whether its assurance failure modes furnish requirements or evaluation tasks for PostCode.
- **Bibliography status:** Proposed and included in draft; **actual Work/repository integration unknown**.

## Earlier adjacent work already in the research bibliography

These references appeared in the uploaded `related-work.md` before the retrospective integration discussion. They should **not** be presented as newly discovered by the six reconstructable watch replies unless independent watch-run evidence is found.

- **CodeSkyline**, *A Code-Map Visualization with Juxtaposed Views for Program Comprehension and Navigation* (reported VISSOFT 2026): multiple juxtaposed views, a multiweek adoption study, and occasional continued use. The initial related-work snapshot already contained it. Citation metadata and exact study findings merit checking; closest to multi-view and sustained-use questions, but not necessarily source-secondary development.
- **Văduva et al., Code2UML**, arXiv:2605.24453: agent-supported multi-language UML with explicit high precision versus low recall tradeoff in prior discussion. Already in the initial snapshot. Relevant to intentionally incomplete, qualified projections.
- **Merino, Ghafari & Nierstrasz (2018)**, *Towards Actionable Visualization for Software Developers*: pre-existing foundational adoption-cost hypothesis. Already in the initial snapshot; compare with the **newly surfaced 2026 follow-up** above.
- **Gao et al., CodeMap** (ICPC 2026): close comprehension/abstraction-switching system, with source still a verification surface; already in the initial snapshot.
- **Davis et al., MAGE** (arXiv:2608.25174), **Dhanorkar et al.** oversight study (arXiv:2606.05391), and further architecture/agent works were already present. Retain as bibliography context, not watch-run discoveries reconstructed here.

## Deferred, rejected, and corrected leads

1. **Graphify identification:** **Deferred / not verified.** Initial report was confident, but later conversation specifically questioned the supplied URL's relationship to the described project. Require a corroborated repository/primary source before using it as prior art.
2. **Sun et al. benchmark identity:** **Unresolved discrepancy.** Earlier watch called it “SilentSwap”; later consolidation used “AgentMonBench.” Could be sub-benchmark versus parent, a misdescription, or something else; **do not infer the resolution** without opening the paper.
3. **Rosa et al. importance:** **Revised upward.** Original description emphasized spec-first work unlike PostCode's projection-first work; later `research.md` widened PostCode to directing, ab initio development, and possible co-evolution of software/conceptual knowledge. That broader scope increases overlap.
4. **Archbird's significance:** **Revised upward in practical priority.** Beyond citation, potentially a baseline or reusable technology to test source-secondary workflow hypotheses without reconstructing all analysis machinery.
5. **Evidence/provenance novelty:** **Narrowed across multiple reports.** SwiftUI Semantic Audit, Archbird, Roteiro, and Cygnus all weaken claims that provenance-aware facts plus disposable code projections or semantic diffs are new mechanisms.
6. **Visualization economics novelty:** **Narrowed by Merino et al. 2026.** The 2018 paper was initially used to motivate PostCode's hypothesis; the 2026 authors' follow-up reportedly makes nearly the same “cheap, task-specific, AI-selected views” argument. Cite rather than present this as an uncited original claim.
7. **Source-secondary framing:** No reported finding directly disproves the *full* PostCode inquiry, but avoid claiming a novel general idea of non-source human interfaces: Rosa et al. and others address adjacent variants. The strongest remaining distinction is an empirical inquiry into **sustained understanding, directing, and supervising through task-adaptive, qualified projections**, across development contexts.
8. **Peer-review and implementation maturity:** Many findings are technical sites or preprints. “Implemented,” “published,” or “presented” in earlier alerts was not consistently substantiated with reviewed code or archival citations; treat them as *reported descriptions* until reviewed in the new watch.

## Implications for apparent novelty (historical synthesis)

**Substantially occupied mechanism space:** deterministic cross-language architecture models; provenance classifications; incomplete/qualified static projections; automatic or agent-assisted visualization generation/selection; semantic change diagrams/diffs; tests linked to code and execution evidence; structured agent-oversight evidence.

**Research contribution still plausibly open:** whether task-adaptive, epistemically explicit projections provide a **sustained primary human conceptual interface for understanding, directing, and supervising agent-mediated software development**, with source retained as an escape hatch; which tasks/source semantics resist abstraction; how guarantees are shown at the point of use; and how use differs for unfamiliar existing software, continued development, and projects developed with PostCode from inception.

The prior watch repeatedly characterized this as **a potentially distinctive conjunction and experimental question, not a confirmed novelty claim**. Since source-review depth and some identities are uncertain, the new watcher should not inherit confident negative claims such as “no system does X” without fresh verification.

## Handover priorities for the new GitHub-based watcher

1. **Sync actual repository state:** Read current `related-work.md`, `research.md`, and any updated positioning or methodology files. The user said Work re-examined some sources and integrated/changed documents after the uploaded snapshot; this handover cannot know which findings survived that review.
2. **Deduplicate by stable identifier or verified project identity**, not by name alone; particularly Merino 2018 versus 2026, Sun benchmark naming, and ambiguous Graphify.
3. **Inspect high-priority primary sources:** Archbird first (as possible baseline), Merino 2026, Roteiro, CodeMap/CodeSkyline, SwiftUI Semantic Audit, Whiteboard, Sun et al. Benchmarks, Rosa et al., Ferris & Bonilla.
4. **Verify levels of evidence:** abstract vs full text; documentation claims vs functioning implementation; precise release/publication dates; peer-reviewed versus preprint; provenance and incompleteness *in user-visible output* versus merely in internal metadata.
5. **Monitor broader research framing:** not solely post-hoc inspection. Include human **direction**, software built **from inception**, and potential effects on software's conceptual clarity/projectability, distinguishing general improvements from tool-specific adaptation.
6. **Report only material *new* overlap:** All eleven findings above are historical leads, not new discoveries for future alerts. Raise them again only for a genuine new development (e.g., replication, revised mechanism, usable release, closer paper, or material correction).
7. **Do not automatically mark bibliography entries merged:** proposed draft text and file-download delivery do not establish the current GitHub version.

## Reconstruction limitations

- Exact scheduled-task run times and dates are absent from the provided conversation; hence **one handover file rather than fabricated per-date reports**.
- The conversation contains six identifiable watch replies; there may have been additional runs with no notification, but there is no reliable record of them. No exhaustive period coverage is asserted.
- Original web-tool logs, source snapshots, and precise inspection granularity for each watch run are unavailable here.
- Some paper and project details were stated by the earlier assistant but not independently corroborated in this retrospective.
- An interim uploaded `related-work.md` and a generated draft show what was *present or proposed* at those moments. Later Work changes to the repository are not available in this chat.
- No personal details, credentials, or full conversation transcript are retained in this public-repository handover.
