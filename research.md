# PostCode: Research Direction

PostCode's conceptual product design and its terminology are described in [`product-design.md`](product-design.md).

## 1. Motivation

The proposition motivating PostCode is:

> **Humans should be able to practice the discipline of software design and architecture in collaboration with agents that implement the software, without needing to be programmers themselves.**

This is an aspiration to investigate, not a claim that architectural practice can already be separated from programming-language proficiency. The distinction is not between *seeing* and *not seeing* source. It is between needing to **know how to read and write conventional programming-language source** and being able to design, understand, and evaluate software without that proficiency.

A practitioner would still need substantial computational and architectural knowledge: behavior, state, concurrency, interfaces, responsibilities, invariants, failure handling, resource constraints, design tradeoffs, and the limits of available evidence. The question is whether that knowledge and the judgment needed to exercise it can be acquired and practiced without the traditional apprenticeship of writing and debugging code.

The analogy is to building architecture: architects practice a design discipline, collaborate with specialists who construct buildings, and use drawings, models, specifications, and prose as working artifacts. They still need to understand construction and its constraints. Software differs in important ways—source code is also a precise executable description, and architectural concepts often map ambiguously to implementation—but the analogy suggests that *practicing architecture* is a more useful framing than merely *supervising implementation*.

The immediate research question is how to support such architectural practice in human–coding-agent collaboration, and in particular:

> **What representations and interactions improve architectural understanding, reasoning, design, and evaluation beyond what a capable conversational coding agent already provides?**

This deliberately sets a strong baseline. Coding agents can already inspect repositories, explain behavior, propose designs, create diagrams, and maintain written notes. PostCode must earn its usefulness against that practice, not merely against manual source reading or text chat without tools.

The current leading hypothesis is that **shared architectural representations**, grounded in **partial, qualified, retained understanding**, may serve as working artifacts for humans and agents: helping them explore one architectural concern, change perspective, revise an account, consider a design, and examine how an implementation realizes it. They may be textual, structured, or visual. Established software-architecture concepts and notations provide starting vocabulary, not an asserted universal program ontology. This is a deliberate choice to draw on an existing discipline rather than wait for shared concepts to emerge solely from source investigations. A borrowed concept should be refined or set aside when it obscures consequential behavior or fails to support useful reasoning.

The research remains open to finding that excellent conversation and ordinary agent-generated diagrams and notes are sufficient for many or all of these purposes.

A broader motivating question remains:

> **What does programming become when humans increasingly delegate implementation to agents?**

This includes whether conventional programming-language source should remain the canonical persistent representation of software. PostCode does not directly investigate that choice. Conventional source might continue to be ideal for agents and for durable implementation even if humans work mainly through architectural representations.

### 1.1 Competence and learning through practice

Programming has traditionally served both to produce software and to develop the judgment necessary to design and maintain it. A person can learn principles of software architecture without being proficient in a particular programming language, but it remains an open question how much implementation-derived experience is necessary for sound architectural judgment.

Imagine someone educated in software design and architecture without conventional coding proficiency. Their working interactions with coding agents might resemble those of an experienced developer using chat today. But their conceptual repertoire, practical intuition, and preferred representations might differ. Less experienced practitioners may need more concrete scenarios, opportunities to explore alternatives, and feedback from consequences; experienced practitioners may delegate more decisions. Neither implies that PostCode is primarily an educational product.

PostCode does not initially investigate software-architecture education or skill acquisition as an independent empirical programme. It investigates support for **practicing** architecture, whether the practitioner's judgment is mature or developing. Such practice might itself help develop expertise, as professional practice normally does, but claims about learning would require distinct evidence.

Research may help identify which architectural concepts and experiences are essential to effective collaboration, and where proficiency in conventional programming remains important. It should not presume that removing source reading automatically produces competent architects.

Conventional source has served as an implementation medium, an inspection medium, and a learning medium. Agent-mediated development raises the possibility that these roles can separate; PostCode primarily studies human-facing architectural practice.

## 2. Beyond Conversational Collaboration

A capable coding agent can already inspect an artifact and present the information useful for a particular purpose. Software adds unusually high demands on the precision and qualification of those explanations. For example, identifying three statically known callers is different from asserting that a function has only three possible callers.

A conversational agent can also generate drawings, state diagrams, architecture descriptions, and maintained Markdown accounts. **Generating a diagram is therefore not, by itself, a distinctive PostCode contribution.**

The hypothesis to investigate is that a shared, explorable architectural working surface might offer something further: coherent and revisable referents, multiple views of selected architectural concerns, explicitly qualified connections to implementation evidence, and continuity between intended designs and later implementation investigations. Such artifacts might let humans notice relationships, test assumptions, challenge explanations, or reason independently in ways that successive prose responses or disconnected illustrations do not support as effectively.

Architectural views should not aspire to encode every detail of a software system. PostCode may retain overlapping, partial and occasionally competing accounts; absence from an account does not imply absence from the software. An investigation of responsibility boundaries may establish enough to draw a structural view, while subsequent investigation of asynchronous behavior requires new evidence, yields a different view, and may force reconsideration of earlier claims.

The value of visual representations, their appropriate level of detail, the selection of what merits the human's attention, and the value of retaining structured architectural knowledge are all empirical questions. Excellent agent chat—**including ordinary ad hoc diagrams and notes**—is the principal practical comparison, alongside source-oriented interfaces when appropriate.

A central epistemological discipline remains essential. Machine-readable structure and persuasive diagrams do not turn an interpretation into a verified property of the implementation. Source, tests, runtime observations, recorded design intent, and agent inference contribute different kinds of evidence and must remain distinguishable.

## 3. What PostCode Investigates

There are at least three distinct representation questions:

1. **Human representation:** Through what representations and interactions can humans practice software design and architecture with coding agents?
2. **Agent representation:** What representation is most useful for coding agents to consume and manipulate?
3. **Persistent program representation:** What should be the canonical durable representation from which the program is built?

PostCode directly investigates the first.

Even a maximally successful PostCode—one in which developers can conduct sustained software work without routinely inspecting conventional programming-language source—would not establish that source should disappear.

Agents might still work best with conventional source. Conventional source might still be the best canonical representation. Alternatively, some future system might use a different human-readable or machine-oriented representation as its persistent source.

Those are separate research questions.

PostCode may weaken one historical reason for privileging conventional programming-language source: the assumption that humans need to work directly with it to understand programs and make architectural decisions.

A related but separate question is whether working directly with conventional source is also necessary for humans to **learn** the concepts and acquire the judgment required for effective software development. PostCode does not initially investigate that educational question, although the concepts that prove useful in architectural practice may eventually provide evidence relevant to it.

This separation is methodological rather than a claim about the eventual programming system.

PostCode investigates **human architectural practice in collaboration with coding agents**, including conceptual understanding, design, direction and evaluation. Its initial tools may remain read-only, with design changes directed through prose.

It does not initially investigate whether coding agents themselves would benefit from a richer semantic representation, nor whether such a representation should eventually become the persistent program. Starting with established architectural concepts does not imply that a complete architecture can be mechanically recovered from arbitrary source.

### 3.1 Creation, continued development, and existing software

There is another distinction within the human-facing question.

PostCode can participate in software development at different points in a program's lifecycle:

- PostCode may support architectural design and subsequent development from a program's inception;
- PostCode may be introduced during the continued development of an existing codebase;
- PostCode may be used to investigate and evaluate changes to an unfamiliar codebase whose development it has never participated in.

These cases may behave differently.

When PostCode participates from the beginning, concepts, intended architectural relationships, specifications, rationale and other information may be available as part of the design process rather than reconstructed later from implementation artifacts. A structural or behavioral model produced during design is a recorded intention, not automatically an established fact about the software that agents subsequently implement. Comparing intended and implemented architecture—perhaps from a newly chosen perspective—is a distinct research opportunity.

When introduced into an existing project, some such information may already exist in source, tests, documentation, version history or previous development context, while other information may need to be recovered or may simply have been lost.

When applied to an unfamiliar codebase, PostCode must derive useful projections from whatever evidence the repository and its history provide.

The project should investigate all three situations rather than assuming that results from one generalize to the others.

It is plausible, for example, that PostCode proves awkward or limited when reconstructing conceptual structure from arbitrary existing software, while projects developed through PostCode from their inception work well because their conceptual structure and development history co-evolve with the interface.

The reverse is also plausible. Existing implementations may provide exactly the concrete ground truth from which useful projections can be derived, while directing the creation of software primarily through projections and higher-level concepts may prove awkward, ambiguous, or less useful than current prose + source-code interaction with coding agents.

Or the different cases may reveal different strengths.

This makes the point at which PostCode enters a program's lifecycle a research dimension in its own right.

### 3.2 How does PostCode-mediated development affect the software?

There are two related but distinct questions. First, using PostCode may cause software and its recorded development context to evolve differently without any explicit policy requiring that result. Second, experience may suggest that agents should deliberately be asked to preserve particular language-agnostic properties of the software and its recorded development context during PostCode-mediated collaboration.

#### 3.2.1 Emergent effects

This raises a further question:

> **Does software created or evolved through PostCode-mediated architectural collaboration differ in significant ways from software developed through ordinary coding-agent conversations?**

Differences might appear in the implementation itself, in the information preserved alongside it, or in both.

For example, sustained interaction at a conceptual level might create pressure for implementations whose structure corresponds more clearly to the concepts through which humans reason about the software.

Such software might exhibit greater **conceptual clarity**: architectural boundaries, responsibilities, effects, invariants, behavior, tests or other implementation properties might correspond more clearly to the conceptual structure through which the human reasons about and directs development.

That could be an independently useful property of the software.

But another possibility is merely **tool-relative projectability**: software developed with PostCode becomes unusually easy for PostCode's particular analyses and projections to interpret without becoming clearer or better according to any independently useful criterion.

This distinction matters.

PostCode and PostCode-native software could co-adapt in ways that make the environment appear highly successful while reducing its ability to generalize to arbitrary software. Conversely, pressure toward projectability might turn out to encourage properties—such as clearer conceptual structure—that remain valuable even outside PostCode.

Whether either effect occurs is an open question.

#### 3.2.2 Deliberate conventions for PostCode-mediated development

PostCode-mediated development may also benefit from explicitly stated conventions for how coding agents implement and document changes. Such conventions would not prescribe the source-language realization in detail. They would instead encourage language-agnostic properties of the software and its recorded development context that help a human understand, design, direct and evaluate the software without routinely working through source.

Possible candidates might concern correspondence between conceptual and implementation boundaries, the discoverability of effects and invariants, the expression of behavior through tests, or the preservation of links among human requests, implementation changes, rationale and verification. These are hypotheses to investigate rather than conventions PostCode currently endorses.

Deliberate conventions raise the same distinction between independently useful conceptual clarity and tool-relative projectability described above. They might also conceal limitations in PostCode by adapting the software to the tool rather than improving the tool's ability to work with arbitrary software.

The project should therefore distinguish effects that arise through ordinary PostCode-mediated development from effects produced by explicit instructions to coding agents. Experience should determine which conventions prove useful, how far they generalize across projects and languages, and whether they should remain project choices, become PostCode recommendations, or eventually be represented or checked by PostCode itself.

## 4. Why Agent-Mediated Development Changes the Problem

Software architecture, visualization, program-comprehension tools, and higher-level program representations long predate coding agents. [Merino, Ghafari, and Nierstrasz (2026)](https://arxiv.org/abs/2608.22151) discuss how generative AI reduces the cost of contextual visualizations, while [moldable development](https://arxiv.org/abs/2409.18811) and [Glamorous Toolkit](https://gtoolkit.com/) already demonstrate the importance of contextual tools. Relevant precedents and their overlap with PostCode are discussed in [`related-work.md`](related-work.md).

In conventional development, humans acquire and refresh much of their understanding of a program through the work of reading, writing, debugging, and changing its source. When coding agents take on more implementation work, that incidental source-level familiarity may diminish even though humans still need to make architectural decisions and evaluate what was built.

At the same time, capable agents make source-free architectural conversations practical: they can inspect a repository, explain how it works, explore design alternatives, generate diagrams, and maintain notes. Generative AI makes such representations cheap **for ordinary chat as well as for PostCode**. Cheap generation and automatic selection therefore help explain why this style of collaboration is possible now, but do not by themselves justify a dedicated projection environment.

The remaining question is whether **systematic, qualified, retained and navigable architectural information** improves collaboration beyond those conversational capabilities: for example, by helping people revisit a design through different perspectives, inspect evidence for architectural claims, recognize incomplete understanding, or compare intended architecture with the subsequent implementation. The importance of particular representations and the right amount of retained structure are questions for use and evaluation, not assumed advantages.

Source may remain useful or necessary for some tasks, and capable chat with diagrams and notes may prove sufficient for others. The research seeks the circumstances in which additional architectural representations and interactions materially help.

## 5. Research Questions

The central investigation is:

> **What would support the effective practice of software design and architecture by humans collaborating with coding agents without requiring programming-language proficiency—and what does a shared, qualified architectural working environment contribute beyond capable agent chat?**

PostCode investigates this through several related sets of questions.

**Architectural practice and attention**

- What knowledge and judgment does a human need to understand, design, direct, and evaluate software? Which aspects require conventional programming-language proficiency, if any?
- Which architectural concerns and levels of detail matter to the human at different stages of a task? Can agents and representations help people discover what deserves investigation, rather than merely answer questions already asked?
- When is delegation appropriate, and when does meaningful human architectural participation benefit from direct exploration, alternative designs, or concrete scenarios?
- Can a human reason about consequences and discover overlooked questions using shared representations more effectively than through conversation alone?

**Concepts, representations, and interaction**

- Which established architectural concepts—responsibilities, boundaries, interfaces, state, ownership, interactions, concurrency, failure, contracts, and others—provide useful starting points? Which require revision or remain language-specific in application?
- Which established visual notations, or combinations of notations, are useful working artifacts in architectural discussions? When are prose, ad hoc agent-generated diagrams, or source better?
- Can partial, qualified and potentially overlapping retained accounts support navigation and reasoning across multiple architectural perspectives without implying a complete program model? Does a coherent working understanding require some stable core, or can it remain largely task-specific?
- Does investigating asynchronous behavior after understanding a responsibility boundary, for example, reveal gaps or change earlier interpretations? What structure or grounding does such reuse need?
- Can the human and agent share stable conceptual referents as an investigation evolves, without assuming permanent semantic identities or source-level names?

**Design, implementation, and change**

- Can intended designs developed in human-agent conversation be examined against implementations using the same architectural vocabulary, while distinguishing requirements, observations, inference and unresolved correspondence?
- How do alternative perspectives change the evaluation of an intended design or its realization? What helps humans notice important architectural deviations or consequences after an agent implements a change?
- What representations help supervise revisions at the level of responsibilities, behavior, constraints and other architectural concerns rather than merely source diffs?
- Does PostCode-mediated practice change the resulting software or its recorded development context? If it becomes more projectable, is that independent architectural clarity or adaptation to PostCode? Can deliberate language-agnostic conventions help without imposing tool-specific structure?

**Epistemology, applicability, and evaluation**

- Which architectural claims can analysis establish, which require interpretation, and how can presentations convey appropriate scope, evidence, limitations and uncertainty?
- What can architectural representations convey about test intent, observed behavior, and the limits of verification without depending on source-language syntax?
- How does usefulness differ across new software, continued development, and unfamiliar repositories; across architectural styles and programming languages; and across experience levels?
- How does a shared architectural working environment compare with capable agent chat equipped with repository tools, diagrams and ordinary notes? Which benefits, if any, require PostCode-specific infrastructure?
- When does source access remain important, and when are qualified architectural representations sufficient?

These are research directions, not a requirement to answer all questions or to implement a comprehensive architecture model. Questions about how architectural competence is formally taught remain motivating rather than part of the initial empirical remit. Research should be free to discover that an established tool, a modest augmentation of chat, or no new interface is the best answer for some tasks.

<a id="possible-findings"></a>
## 6. What Might We Learn?

PostCode does not have a predefined experimental endpoint at which the project as a whole succeeds or fails.

It is intended as an ongoing development and research programme in which building and use produce a stream of findings—positive, negative, mixed and unexpected—that influence what is investigated and built next.

Some possible findings include the following.

### Architectural representations become a routine working surface

Humans and coding agents use qualified architectural representations as ongoing working artifacts for understanding, design and evaluation, rather than merely as occasional summaries or illustrations.

### Capable chat or source makes PostCode unnecessary for some tasks

Higher-level representations help in particular circumstances, but source remains extraordinarily useful and information-dense for broad classes of software investigation. Or a capable conversational coding agent, with ordinary diagrams and notes, offers equivalent architectural collaboration without PostCode-specific machinery.

Either would be an important finding rather than a failure of the research.

### Greenfield and existing-code use differ

PostCode proves substantially more useful when it participates in development from a project's inception than when reconstructing conceptual structure from arbitrary existing code—or the reverse.

The circumstances under which PostCode enters the development lifecycle may turn out to matter as much as the particular projections it provides.

### PostCode changes the resulting software

Software developed through PostCode-mediated architectural collaboration develops measurably or observably different characteristics from software developed through ordinary coding-agent conversations.

Those differences might be beneficial, harmful, neutral, or merely adaptations to PostCode itself.

### Projection diffs become particularly useful

Comparing projections across revisions proves useful for supervising agent-generated changes even if projections do not replace source for ordinary comprehension.

### Trust becomes particularly important

The most valuable contribution turns out to be explicit epistemological guarantees about what program views do and do not establish, rather than any particular representation.

### Established architectural vocabulary transfers—or does not

Starting with established architectural concepts and notations proves useful across implementation languages, perhaps after important qualification or extension. Alternatively, familiar architectural labels prove misleading without language-specific interpretation.

### Provenance becomes particularly important

A useful alternative to source turns out to be an environment that allows derived facts, recorded rationale, behavioral evidence and interpretation to be investigated together without collapsing their distinctions.

### Tests become a bridge

Behavioral test intent can often be separated usefully from source-language realization, while cases that resist abstraction expose important boundaries between language-independent behavior and implementation-specific properties.

### Representation selection becomes particularly important

The important capability turns out not to be any particular visualization or projection, but selecting which architectural concerns deserve attention, when, and at what level of detail.

### Visual artifacts support architectural reasoning

Shared structural and behavioral views help people develop and challenge architectural judgments, rather than merely restating an agent's explanations. Alternatively, the views contribute no significant benefit beyond ordinary conversational diagrams.

### Partial knowledge supports cross-perspective investigation

Qualified, revisable, overlapping accounts support coherent investigation across concerns without constructing a complete software model—or fragmentation and disputed correspondence make this approach too awkward.

### Intended and implemented architecture can be examined together

Using related architectural concepts during design and later implementation evaluation helps uncover consequential deviations or design weaknesses, even when correspondence remains interpretive. Alternatively, ordinary plans, code review, and chat provide enough support.

These are examples of discoveries the research could plausibly make, not outcomes PostCode is required to produce.

Different parts of the work may support different or even apparently conflicting findings. A projection may be useful for one class of investigation and actively unhelpful for another. A technique that works well in one language or codebase may fail to generalize. A workflow that works for PostCode-native software may work poorly for unfamiliar software, or vice versa.

Such boundaries are themselves part of what the project is intended to discover.

## 7. Negative and Limiting Findings

Negative evidence is not necessarily evidence that PostCode as a whole has failed.

A finding may instead establish the limits of a particular projection, technique, interaction model, abstraction or research hypothesis. Such findings should be treated as first-class results and allowed to redirect subsequent work.

Potential negative or limiting findings include:

- for broad classes of questions or development activities, projections prove less useful than source—for example by requiring more effort, taking longer, producing poorer understanding, or simply causing developers to prefer opening source;
- useful analyses cannot provide adequate guarantees;
- qualification necessary for trust makes projections cumbersome or difficult to interpret;
- automatic projection or presentation selection frequently chooses badly;
- developers must understand the available projection vocabulary well enough that automatic selection adds little;
- recorded rationale is too stale or unreliable to contribute usefully;
- test intent cannot be projected usefully without source-level detail;
- cross-language abstractions prove shallow or misleading;
- important implementation facts routinely escape projection;
- projection comparisons often fail to provide information developers find useful beyond conventional source diffs;
- PostCode works well only on projects whose development it has influenced;
- pressure toward projectability produces implementations optimized for PostCode's analyses without improving—and perhaps while degrading—other desirable software properties;
- conceptual-level interaction proves useful for understanding software but too awkward or underspecified for directing its creation;
- conceptual-level interaction works well for creating software but cannot reliably recover enough information from arbitrary existing code;
- capable agent chat with repository access, ordinary diagrams, and retained notes already provides most of the useful architectural workflow, leaving little role for a dedicated projection environment;
- architectural drawings offer convincing but misleading coherence, especially when composed from partial or conflicting evidence;
- known architectural notations fit poorly with the concepts that arise during real investigation, or cannot convey qualification without becoming unwieldy;
- partial retained accounts are too disconnected or difficult to reconcile across perspectives to support dependable architectural reasoning;
- intended architectural representations do not correspond sufficiently to implementations to support useful evaluation, even with explicit uncertainty.

Other negative findings will almost certainly arise from things that have not yet been anticipated.

Mixed results may be especially interesting.

The goal is not to prove that visual architectural models outperform conversation, or that conventional programming-language source should disappear.

It is to keep asking:

> **What helps humans practice software architecture as a discipline in collaboration with coding agents—and what, if anything, warrants a dedicated environment beyond chat?**

## 8. Research and Impact Goal

If the work proves worthwhile, it should make a meaningful contribution to understanding how programming evolves in an agent-mediated world.

Possible contributions may concern:

- architectural representations as working artifacts for human–agent software design and investigation;
- explicit comparisons with capable conversational agents and ad hoc visual explanations;
- partial, qualified architectural knowledge supporting multiple perspectives;
- connections and mismatches between intended architecture and implemented software;
- projections as substitutes or complements for source inspection;
- conceptual interfaces for directing agent-mediated software development;
- epistemological contracts for program views;
- automatic projection and representation selection;
- combining derived facts, recorded assertions, observations and interpretation;
- tests as projected behavioral evidence;
- projection diffs for supervising agent changes;
- persistence of human attention without semantic identity;
- the usefulness and limits of established language-independent architectural concepts and notations;
- conceptual clarity and projectability as properties of software;
- differences between PostCode-native, continued-development and unfamiliar-codebase use;
- circumstances in which source remains necessary.

The strategy for recognizing, communicating, and strengthening these contributions is described in [`research-strategy.md`](research-strategy.md).

The long-term question remains open:

> **What should the persistent program ultimately be?**

PostCode does not answer that question.

It investigates one part of the larger problem:

> **What helps humans practice software design and architecture with coding agents beyond what capable conversation already provides?**
