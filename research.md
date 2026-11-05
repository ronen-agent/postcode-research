# PostCode: Research Direction

PostCode's conceptual product design and terminology are described in [`product-design.md`](product-design.md). A broader catalog of potentially fruitful questions is retained in [`notes/research-question-catalog.md`](notes/research-question-catalog.md); inclusion there does not make a question part of the current governing program.

## 1. Motivation

The proposition motivating PostCode is:

> **Humans should be able to practice the discipline of software design and architecture in collaboration with agents that implement the software, without needing to be programmers themselves.**

This is an aspiration to investigate, not a claim that architectural practice can already be separated from programming-language proficiency. The question is whether humans can develop and exercise architectural judgment without needing to learn how to read or write conventional programming-language source.

PostCode deliberately excludes programming-language source from its human-facing presentations to investigate that possibility. This is a product-design choice, not a finding that every architectural task can be supported without source-language literacy. Inadequacies and unanswerable questions are evidence about the limits of the approach.

A practitioner would still need substantial computational and architectural knowledge: behavior, state, concurrency, interfaces, responsibilities, invariants, failure handling, resource constraints, design tradeoffs, and the limits of available evidence. The question is whether that knowledge and the judgment needed to exercise it can be acquired and practiced without the traditional apprenticeship of writing and debugging code.

The analogy is to building architecture: architects practice a design discipline, collaborate with specialists who construct buildings, and use drawings, models, specifications, and prose as working artifacts. They still need to understand construction and its constraints. Software differs in important ways—source code is also a precise executable description, and architectural concepts often map ambiguously to implementation—but the analogy suggests that *practicing architecture* is a more useful framing than merely *supervising implementation*.

The immediate research question is:

> **What representations and interactions support architectural understanding, reasoning, design, and evaluation beyond what a capable conversational coding agent already provides?**

This deliberately sets a strong baseline. Coding agents can already inspect repositories, explain behavior, propose designs, create diagrams, and maintain written notes. PostCode must earn its usefulness against that practice, not against a weakened text-only conversational baseline.

The current leading hypothesis is that **shared architectural representations**, grounded in **partial, qualified, retained understanding**, may serve as working artifacts for humans and agents: helping them explore one architectural concern, change perspective, revise an account, compare alternatives, record an intention, and examine how an implementation realizes it. They may be textual, structured, or visual. Established software-architecture concepts and notations provide starting vocabulary, not an asserted universal program ontology. This is a deliberate choice to draw on an existing discipline rather than wait for shared concepts to emerge solely from source investigations. A borrowed concept should be refined or set aside when it obscures consequential behavior or fails to support useful reasoning.

The research remains open to finding that excellent conversation and ordinary agent-generated diagrams and notes are sufficient for many or all of these purposes.

A broader motivating question remains:

> **What does programming become when humans increasingly delegate implementation to agents?**

This includes whether conventional programming-language source should remain the canonical persistent representation of software. PostCode does not directly investigate that choice. Conventional source might continue to be ideal for agents and for durable implementation even if humans work mainly through architectural representations.

### 1.1 Competence and learning through practice

Programming has traditionally served both to produce software and to develop the judgment necessary to design and maintain it. A person can learn principles of software architecture without being proficient in a particular programming language, but it remains an open question how much implementation-derived experience is necessary for sound architectural judgment.

Imagine someone educated in software design and architecture without conventional coding proficiency. Their working interactions with coding agents might resemble those of an experienced developer using chat today. But their conceptual repertoire, practical intuition, and preferred representations might differ. Less experienced practitioners may need more concrete scenarios, opportunities to explore alternatives, and feedback from consequences; experienced practitioners may delegate more decisions. Neither implies that PostCode is primarily an educational product.

PostCode does not initially investigate software-architecture education or skill acquisition as an independent empirical program. It investigates support for **practicing** architecture, whether the practitioner's judgment is mature or developing. Such practice might itself help develop expertise, as professional practice normally does, but claims about learning would require distinct evidence.

Research may help identify which architectural concepts and experiences are essential to effective collaboration, and where proficiency in conventional programming remains important. It should not presume that a source-independent interface automatically produces competent architects.

Conventional source has served as an implementation medium, a foundation for program understanding, and a medium for learning software development. Agent-mediated development raises the possibility that these roles can separate; PostCode primarily studies human-facing architectural practice.

## 2. Beyond Conversational Collaboration

A capable coding agent can already inspect an artifact and present the information useful for a particular purpose. Software adds unusually high demands on the precision and qualification of those explanations. For example, identifying three statically known callers is different from asserting that a function has only three possible callers.

A conversational agent can also generate drawings, state diagrams, architecture descriptions, and maintained Markdown accounts. **Generating a diagram is therefore not, by itself, a distinctive PostCode contribution.**

The hypothesis to investigate is that a shared, explorable architectural working surface might offer something further: coherent and revisable referents, multiple views of selected architectural concerns, explicitly qualified connections to implementation evidence, and continuity between intended designs and later implementation investigations. Such artifacts might let humans notice relationships, test assumptions, challenge explanations, or reason independently in ways that successive prose responses or disconnected illustrations do not support as effectively. This shared-representation hypothesis describes one way PostCode's specialization might support direct investigation and architectural collaboration.

<a id="specialized-architectural-expertise"></a>

PostCode deliberately specializes in evidence-grounded architectural investigation and retained understanding for direct human use and within larger human–agent design processes. That specialization is a product-design choice whether or not it eventually outperforms general-purpose agents. The product aspires to develop architectural investigative expertise—both in understanding implemented software and in investigating proposed designs—superior, along relevant dimensions, to what capable general-purpose coding or design agents ordinarily provide. Whether it achieves that superiority, and whether its expertise improves architectural practice, are research hypotheses rather than established advantages.

Evidence and possible claims should remain separated at three levels:

1. **Direct human investigation:** whether PostCode supports useful orientation, questioning, understanding, and exploration.
2. **Architectural-account quality:** whether its specialization produces accounts that are accurate, appropriately qualified, relevant, systematic, reusable, or otherwise valuable.
3. **Architectural practice:** whether using those accounts changes human–agent design, direction, review, or outcomes.

These are analytic levels, not three efficacy claims the project must eventually establish. Useful investigation need not establish comparative superiority; better accounts need not improve design decisions; and continuity, shared references, or disciplined comparison might improve collaboration even when individual explanations are not intrinsically superior.

Architectural views should not aspire to encode every detail of a software system. PostCode may retain overlapping, partial and occasionally competing accounts; absence from an account does not imply absence from the software. An investigation of responsibility boundaries may establish enough to draw a structural view, while subsequent investigation of asynchronous behavior requires new evidence, yields a different view, and may force reconsideration of earlier claims.

The value of visual representations, their appropriate level of detail, the selection of what merits the human's attention, and the value of retaining structured architectural knowledge are all empirical questions. Excellent agent chat—**including ordinary diagrams and retained notes**—is the principal practical comparison.

A central epistemological discipline remains essential. Machine-readable structure and persuasive diagrams do not turn an interpretation into a verified property of the implementation. Source, tests, runtime observations, recorded design intent, and agent inference contribute different kinds of evidence and must remain distinguishable.

<a id="likely-contribution-model"></a>

### 2.1 Likely contribution model

The most realistic primary contribution is constructive, evidence-grounded design knowledge about what is required to support architectural practice without requiring programming-language proficiency from the human: a consequential problem framing; a working artifact; the design and implementation insights required to construct it; evidence from sustained formative use; and well-scoped lessons about useful mechanisms, tensions, limitations, and unresolved questions.

PostCode assumes relevant computational, design, and architectural proficiency. Whether that proficiency can be acquired without prior programming experience is a separate question outside the project's current scope.

A bounded demonstration that consequential architectural work can be performed without exercising proficiency in the implementation language would itself be a substantial result.

Comparative account-quality findings, evidence of changed architectural practice, or broader studies may strengthen or extend that contribution, but they are not its required endpoint. A credible contribution may instead identify requirements for source-independent practice, explain why apparently attractive mechanisms fail, characterize where qualified retained accounts help, or establish boundaries beyond which ordinary agent chat or programming-language knowledge remains necessary.

## 3. What PostCode Investigates

There are at least three distinct representation questions:

1. **Human representation:** Through what representations and interactions can humans practice software design and architecture with coding agents?
2. **Agent representation:** What representation is most useful for coding agents to consume and manipulate?
3. **Persistent program representation:** What should be the canonical durable representation from which the program is built?

PostCode directly investigates the first. Its architectural accounts may also be shared with design and implementation agents as part of human–agent architectural practice; this does not turn the project into a general investigation of the representations on which agents themselves reason best.

Even a maximally successful PostCode—one enabling sustained architectural practice without programming-language literacy—would not establish that source should disappear as an implementation artifact.

Agents might still work best with conventional source. Conventional source might still be the best canonical representation. Alternatively, some future system might use a different human-readable or machine-oriented representation as its persistent source.

Those are separate research questions.

PostCode may weaken one historical reason for privileging conventional programming-language source: the assumption that humans need to work directly with it to understand programs and make architectural decisions.

A related but separate question is whether programming-language proficiency is necessary for humans to **learn** the concepts and acquire the judgment required for effective software development. PostCode does not initially investigate that educational question, although the concepts that prove useful in architectural practice may eventually provide evidence relevant to it.

This separation is methodological rather than a claim about the eventual programming system.

PostCode investigates **human architectural practice in collaboration with coding agents**, including conceptual understanding, design, direction and evaluation. Its initial tools may remain read-only, with design changes directed through prose.

It does not initially investigate whether coding agents themselves would benefit from a richer semantic representation, nor whether such a representation should eventually become the persistent program. Starting with established architectural concepts does not imply that a complete architecture can be mechanically recovered from arbitrary source.

### 3.1 Creation, continued development, and existing software

PostCode may participate from a program's inception, enter during continued development, or investigate unfamiliar existing software. These contexts exert different pressure. Development from inception may preserve intentions, rationale, and conceptual structure as they arise; continued development must interact with an existing implementation and history; unfamiliar software tests what can be recovered from evidence PostCode did not help shape.

Findings from one context must not silently generalize to the others. PostCode may work best where conceptual structure co-evolves with the tool, or existing implementations may provide firmer evidence than speculative design work. The methodological roles of these contexts are described in [`methodology.md`](methodology.md#2-formative-use).

### 3.2 Co-adaptation, conceptual clarity, and projectability

PostCode-mediated development may change the software or its recorded context, either through ordinary use or through explicit conventions. Some changes may improve independently useful **conceptual clarity**; others may merely make the software easier for PostCode's current analyses to project. Co-adaptation can therefore produce genuine design knowledge while also making the tool appear more successful than it would be on arbitrary software.

Formative analysis should distinguish emergent effects from deliberate interventions and independently useful clarity from **tool-relative projectability**. Candidate conventions and their evaluation questions are retained in [`notes/candidate-conventions.md`](notes/candidate-conventions.md).

## 4. Why Agent-Mediated Development Changes the Problem

In conventional development, humans acquire and refresh much of their understanding of a program through the work of reading, writing, debugging, and changing its source. When coding agents take on more implementation work, that incidental source-level familiarity may diminish even though humans still need to make architectural decisions and evaluate what was built.

At the same time, capable agents make source-independent architectural conversations practical: they can inspect a repository, explain how it works, explore alternatives, generate diagrams, and maintain notes. Cheap generation and automatic selection help explain why this style of collaboration is possible now, but do not by themselves justify a dedicated environment.

The remaining question is what **systematic, qualified, retained and navigable architectural information** contributes beyond those conversational capabilities, both to direct human investigation and to collaboration: for example, by helping people revisit a design through different perspectives, inspect evidence for architectural claims, recognize incomplete understanding, or compare intended architecture with the subsequent implementation. The importance of particular representations and the right amount of retained structure are questions for use and evaluation, not assumed advantages.

Some questions may remain inadequately supported even after further investigation, while capable chat may suffice for others. Relevant precedents and their overlap with PostCode are discussed in [`related-work.md`](related-work.md).

## 5. Research Questions

The central investigation is:

> **What supports the effective practice of software design and architecture by humans collaborating with coding agents without requiring programming-language proficiency—and what does a shared, qualified architectural working environment contribute beyond capable agent chat?**

The current program is organized by these questions:

- What knowledge and judgment does architectural practice require, and which aspects—if any—depend on conventional programming-language proficiency?
- What does PostCode contribute to direct human investigation when no external design or implementation agent participates in the task?
- Which architectural concerns, concepts, and levels of detail matter during genuine tasks, and how should PostCode help participants discover what deserves attention?
- When do partial, qualified, retained accounts support reasoning across perspectives, and when do they become fragmented, misleading, or unnecessarily burdensome?
- Which architectural claims can analysis establish, which require interpretation, and how should scope, evidence, limitations, and uncertainty be conveyed?
- Can humans and agents share stable conceptual referents without presuming permanent semantic identities, authoritative accounts, or source-level names?
- Can implemented states, hypothetical alternatives, and intended designs be investigated and compared without disguising their different evidentiary bases?
- What helps humans notice consequential architectural changes, deviations, and unresolved questions after agents implement software?
- When and how do persistent textual, structured, or visual representations help people notice relationships, reason about consequences, or identify gaps beyond conversation, ordinary agent-generated diagrams, and retained notes?
- Which capabilities add value beyond capable agent chat with repository tools, diagrams, and retained notes, and which merely reproduce that practice with additional machinery?
- How do findings vary across new software, continued development, unfamiliar repositories, architectural styles, programming languages, and practitioner experience?

These questions guide the current program; they are not a requirement to answer everything before the work can contribute. The broader [research-question catalog](notes/research-question-catalog.md) preserves secondary and longer-term questions that may become important as evidence or opportunities arise.

<a id="8-research-and-impact-goal"></a>
<a id="contribution-and-claim-scope"></a>

## 6. Contribution and Claim Scope

PostCode has no predefined experimental endpoint at which the project as a whole succeeds or fails. Construction and use may contribute:

- design requirements, mechanisms, patterns, and failure modes for source-independent architectural practice;
- a documented artifact and the implementation knowledge needed to realize its conceptual design;
- conditional findings about when specialized investigation and retained accounts help or hinder;
- independently checked findings about the quality and limits of particular architectural accounts;
- concepts or mechanisms that transfer beyond PostCode;
- negative or mixed findings that narrow the plausible role of projections;
- practical tools, demonstrations, or workflows whose value is distinct from a general research claim.

The primary aim is not to prove that PostCode globally outperforms conversation or improves architectural outcomes. Claims should follow the available evidence. Formative self-study can support design findings, bounded observations about the developer's experience, and hypotheses. Independent checks can support claims about particular account contents or guarantees. General claims about developer behavior, architectural competence without programming experience, or comparative outcomes require evidence from appropriate participants and tasks that the initial program may never undertake.

Transferability comes from explaining the problem, context, mechanism, design rationale, evidence, contrary cases, interventions, and limits—not from presenting one developer's sustained use as representative. Negative, conditional, and unresolved results are first-class contributions when they are traceable and consequential. The broader question catalog preserves possible findings and limiting cases as questions rather than governing commitments.

The process for turning formative evidence into such findings is described in [`methodology.md`](methodology.md). The strategy for recognizing, communicating, and strengthening prospective contributions is described in [`research-strategy.md`](research-strategy.md).

The long-term question remains open:

> **What should the persistent program ultimately be?**

PostCode does not answer that question.

It investigates one part of the larger problem:

> **What helps humans practice software design and architecture with coding agents beyond what capable conversation already provides?**
