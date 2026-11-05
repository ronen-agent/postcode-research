# Research Question Catalog

Status: exploratory catalog; questions here are not governing commitments, roadmap items, or requirements that PostCode answer everything listed

This note preserves potentially fruitful questions beyond the compact set that currently organizes [`research.md`](../research.md#5-research-questions). Questions may become timely as construction, formative evidence, related work, or collaboration exposes a concrete reason to pursue them.

The catalog is deliberately broader than the active program. It should remain curated: combine duplicates, remove questions that no longer open a meaningful line of inquiry, and add context when a question's relevance would otherwise be obscure.

## Architectural competence and participation

- Which parts of architectural judgment arise from direct implementation experience, and which can be developed through conceptual study and practice?
- Can people without conventional programming proficiency recognize infeasible, unsafe, or disproportionately expensive designs when their implementation consequences are presented architecturally?
- Which concrete scenarios, feedback loops, and encounters with consequences help a developing practitioner acquire sound judgment?
- How do experienced developers' preferred representations differ from those of people educated in architecture without a programming apprenticeship?
- When is delegation appropriate, and when does meaningful human participation require direct exploration of alternatives and consequences?
- What would constitute evidence that a source-independent interface supports architectural practice without implying that it teaches architecture?

## Attention, concepts, and representation

- Which architectural concerns and levels of detail deserve attention at different stages of a task?
- Can PostCode help people discover consequential questions rather than merely answer questions already asked?
- Which established concepts—responsibility, boundary, ownership, state, interaction, contract, concurrency, failure, and others—transfer usefully across software, and where do they distort what matters?
- Which established visual notations or combinations remain useful when evidence, uncertainty, and partiality must remain visible?
- When are prose and ordinary agent-generated diagrams sufficient?
- Does a coherent working understanding require a stable conceptual core, or can it remain largely task-specific and perspectival?
- Can human and agent participants share useful conceptual referents without permanent semantic identity or source-level names?
- Which questions need new PostCode-native concepts rather than established architecture vocabulary?

## Partial and retained understanding

- Under what conditions do partial, qualified, overlapping accounts support cross-perspective reasoning?
- When do retained accounts instead become stale, fragmented, contradictory, or too expensive to reconcile?
- What should be retained as durable architectural understanding, what should remain a transient view, and what belongs only in conversation?
- How should later investigation extend or challenge an earlier account without silently treating it as current implementation evidence?
- Can a useful investigation remain bounded to one concern while still exposing dependencies on omitted concerns?
- Does the principal value of retention lie in accumulated knowledge, continuity of attention, stable references, or the ability to revisit evidence?

## Design, implementation, and change

- How much useful architectural reasoning can be performed on a hypothetical design before implementation or execution evidence exists?
- Can implemented states, hypothetical alternatives, and intended designs be compared using related concepts without disguising differences in evidence and authority?
- What helps people notice consequential deviations, unexpected architectural effects, or unresolved questions after an agent implements a change?
- When is a conceptual diff more useful than an ordinary patch explanation, and what perspectives should determine salience?
- Does PostCode-mediated development produce independently useful conceptual clarity or merely tool-relative projectability?
- Which conventions help architectural practice across tools and projects, and which merely compensate for current PostCode limitations?
- Does PostCode work differently when present from a project's inception, introduced during continued development, or applied to unfamiliar software?
- Can intended architecture remain useful as implementation evolves without becoming an authoritative model that conceals divergence?

## Evidence, trust, and account quality

- Which architectural claims can mechanical analysis establish, which require interpretation, and which remain unavailable?
- When does explicit qualification increase trust, and when does it make representations too cumbersome to use?
- Can factual account quality be assessed independently of whether a representation was pleasant, persuasive, or useful?
- What should PostCode report when evidence cannot support an architectural decision?
- How should derived facts, recorded rationale, behavioral observations, tests, and interpretation be investigated together without collapsing their distinctions?
- When does recorded rationale become too stale or unreliable to help?
- What can test intent and observed behavior establish at an architectural level without losing consequential implementation detail?
- How should changes in PostCode's own analyses remain distinguishable from changes in the investigated software?
- When do architectural representations create convincing but misleading coherence from partial, conflicting, or weakly supported information?

## Comparison with capable agents and other systems

- Which capabilities add value beyond capable agent chat with repository tools, ordinary diagrams, and retained notes?
- Which PostCode mechanisms can be reproduced adequately through prompting and ordinary documents?
- Does specialized investigation improve account quality, or merely add structure and cost?
- Can collaboration benefit from shared references and continuity even when individual explanations are no better than capable chat?
- How does a design agent's access to implementation source, PostCode, or both affect architectural reasoning?
- Which existing program-comprehension, architecture-recovery, moldable-development, visualization, or oversight tools can supply analyses or interaction patterns that PostCode should reuse?
- What specific conjunction, guarantee, composition, or interaction—if any—constitutes a contribution beyond established approaches?

## Context, transfer, and limiting cases

- Which findings transfer across codebases, domains, architectural styles, programming languages, and development stages?
- Which concepts generalize across languages, and which mechanisms must remain language- or paradigm-specific?
- Can specialized investigation make software in unfamiliar or specialized languages accessible more effectively than general-purpose agents can investigate it directly?
- What important implementation facts routinely escape architectural projection?
- Are some consequential decisions impossible to support reliably without implementation-language proficiency?
- Does PostCode help with understanding but remain too awkward for directing creation—or help with greenfield design but fail to recover existing software?
- When does capable conversation leave too little remaining value to justify a dedicated environment?
- Which negative or mixed findings reveal a boundary of a particular capability, and which challenge the projection-based approach itself?

## Possible contribution outcomes

The following tensions can guide speculative papers or bounded investigations without presupposing which side will hold:

- Architectural representations become routine working artifacts—or remain occasional summaries.
- Specialized investigation produces better-qualified accounts—or adds machinery without improving what matters.
- Better accounts improve architectural decisions and review—or fail to affect outcomes.
- Epistemological guarantees matter more than any particular representation—or prove too burdensome in practice.
- Representation selection becomes the central capability—or users prefer direct control of familiar views.
- Established architectural vocabulary transfers across languages—or conceals language-specific semantics.
- Qualified comparison supports design and implementation review—or correspondence among accounts remains too interpretive to help.
- PostCode-native software develops useful conceptual clarity—or co-adapts in ways that undermine transfer.
- Partial retained understanding supports coherent movement across perspectives—or fragments into irreconcilable accounts.
- Ordinary agent chat proves sufficient for broad classes of work—or exposes recurring needs for specialized, retained investigation.
