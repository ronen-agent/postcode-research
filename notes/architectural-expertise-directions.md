# Architectural expertise and comparative investigation directions

Recorded: 2026-11-04

Status: exploratory research note; not scheduled work or an application requirement

## Motivation

PostCode can be understood as contributing specialized architectural investigative expertise within a larger design process. Humans and agents may conduct their design conversation elsewhere while consulting, challenging, and extending PostCode's evidence-grounded accounts.

The specialization is a product-design choice whether or not PostCode eventually outperforms general-purpose agents. Superior expertise in understanding implemented software and investigating proposed designs is an aspiration; whether that superiority is achieved, and whether it improves architectural practice, are research hypotheses.

This perspective suggests capabilities and experiments beyond the immediate application journey. The governing conceptual commitments appear in [`product-design.md`](../product-design.md); the research hypotheses appear in [`research.md`](../research.md). This note preserves illustrative roles, examples, experimental conditions and possible later applications without making them requirements or roadmap commitments.

## Illustrative participant roles

A collaborative architectural process might involve:

- a **human architect**, contributing goals, requirements, domain knowledge, judgments, tradeoffs and decisions;
- a **design agent**, contributing alternatives, critique, collaborative reasoning and development of proposed solutions;
- **PostCode**, contributing qualified investigation of actual and proposed architecture, retained understanding, comparisons and challenges to assumptions;
- an **implementation agent**, translating accepted architectural intentions into working software.

These are roles, not necessarily separate systems, users or processes. One agent may perform design and implementation work, and a human may delegate or participate differently from task to task. The decomposition is useful for asking what expertise each participant contributes, not for prescribing a workflow or collaboration interface.

PostCode need not become a participant in the architectural conversation. Shared references, shared machine-readable context and access to investigation capabilities may be sufficient for humans and external agents to use its expertise.

## Comparative architectural investigation

A common capability underlies several apparently different activities: compare qualified architectural accounts from a chosen perspective, establish whatever correspondence the evidence supports, and expose differences, consequences and unresolved questions.

Relevant comparisons include:

- an implemented state and an earlier implemented state, to investigate architectural history;
- an implemented state and a hypothetical alternative, to examine a proposal;
- two hypothetical alternatives, to compare designs;
- an intended design and its resulting implementation, to evaluate realization;
- a prior implementation, intended change and resulting implementation, to distinguish what changed from whether it changed as intended.

The investigative expertise may be shared, but the guarantees are not. Actual-to-actual comparison can use evidence from both implementations. Actual-to-hypothetical comparison is conditional on the proposed account. Intended-to-implemented comparison may depend on interpretive correspondence. A persuasive alignment or diagram does not establish feasibility, correctness or conformance.

Retaining architectural understanding concerns how qualified knowledge persists; investigating hypothetical architecture expands the subject matter on which PostCode can operate. An open question is how much useful architectural reasoning can be supported by a proposed design alone and which questions require implementation or execution evidence.

## Cockatiel issue illustration

A discussion exercise exploring how to address [Cockatiel issue #111](https://github.com/connor4312/cockatiel/issues/111) considered replacing or supplementing an execution-triggered circuit-breaker transition with a timer-driven transition.

With implemented-software capabilities alone, PostCode could investigate the existing policy responsibilities, composition, state, admission semantics and events. The human and design agent could develop the alternative externally. After implementation, PostCode could support architectural change review.

With hypothetical-account support, the proposed timer-driven behavior could also become qualified investigation material before an implementation agent translates it into code. Architectural participants could ask:

- How would the proposed state model differ from the implemented one?
- Which existing responsibilities, interactions or guarantees might it affect?
- Are there contradictions, missing information or unresolved assumptions?
- Which further architectural questions should be investigated before choosing a design?
- After implementation, where does the resulting software correspond to or depart from the intention?

This does not require PostCode to select the design, establish that the proposal is feasible, or simulate every consequence.

## Candidate source-access comparisons

One possible experimental variable is the implementation access available to architectural participants. Conditions might include:

1. a human working with a capable design agent that has ordinary repository access and can produce diagrams and notes;
2. the same participants and access, augmented with PostCode;
3. a human and design agent whose implementation investigations go exclusively through PostCode, while an implementation agent retains source access.

Comparing conditions 1 and 2 can test PostCode's added value when the design agent retains ordinary repository access. Comparing conditions 2 and 3 can test whether PostCode supplies enough architectural information for meaningful collaborative design and how restricting the design agent's direct source access changes architectural reasoning. Human-facing output remains independent of programming-language source in every condition.

Restriction could reduce anchoring on existing implementation choices and encourage attention to responsibilities, constraints and alternatives. It could instead conceal implementation constraints or opportunities necessary for good design. The direction of the effect must not be assumed.

Successful conversation, participant satisfaction or absence of inadequacy reports would not establish that the resulting architectural reasoning was correct. Account quality and design outcomes require independent assessment.

## Possible applications where implementation is difficult to use directly

### Restricted implementation access

A PostCode-like service might mediate architectural access to software held in a restricted environment. Human architects and design agents could investigate selected architectural properties while implementation agents operate inside that environment.

This is not a current security claim or application direction. Hiding source in a presentation does not create a security boundary; architectural information may itself be sensitive, and secure deployment would require access control, information-release policy and appropriate assurance.

### Specialized implementation languages or systems

An implementation may use an unfamiliar, proprietary, obscure or highly specialized language, paradigm or execution system. PostCode could potentially encapsulate reusable investigative knowledge through language- or system-specific analyses and expose qualified architectural information through concepts accessible to architectural practitioners and general-purpose design agents.

The benefit would not come merely from hiding unfamiliar code. It would depend on developing and validating investigative expertise that ordinary agents lack or would otherwise have to reconstruct. Existing architectural concepts and guarantees must not be assumed to transfer automatically.

This suggests a possible later research question:

> Can specialized, validated architectural investigation make software implemented in unfamiliar or specialized languages accessible to architectural practitioners and general-purpose design agents more effectively than those agents can investigate it directly?

The related question of cross-paradigm architectural vocabulary is discussed in [`cross-paradigm-architectural-concepts.md`](cross-paradigm-architectural-concepts.md).

## Evaluation directions

Possible future evaluation should keep at least three questions separate:

1. Does PostCode support useful direct human architectural investigation, considering orientation, understanding, questions discovered and information needs satisfied?
2. Does PostCode's specialization improve the architectural accounts produced, considering factual accuracy, qualification, relevance, reuse and challengeability?
3. Does using those accounts improve architectural collaboration or outcomes, considering alternatives explored, consequential questions noticed, decisions made, implementation review and resulting designs?

PostCode might succeed at any combination of these levels. Collaboration might benefit from persistent shared references even when individual explanations are no better than capable agent chat. Superior accounts might fail to affect a decision or might introduce enough friction to make the overall process worse.

Appropriate comparisons use capable general-purpose agents with realistic tools, repository access, diagrams and retained notes. Source access, retained context and assistance available in each condition should be explicit rather than varied accidentally.

## Scope boundaries

These directions do not make PostCode:

- a replacement for the broader software-development environment;
- a diagram generator whose output is valuable merely because it is visual;
- an architectural oracle or final decision-maker;
- a required host for human–agent design conversation;
- a general-purpose architecture simulator;
- a formal verification system;
- an authoritative consolidated architecture model;
- a secure information-mediation system merely because it withholds source;
- a product in which every lens must apply alike to implemented states, observations, hypothetical alternatives and intended designs.

The immediate application can continue to investigate implemented software. The broader conceptual design allows later journeys to incorporate hypothetical and intended accounts without treating implementation scheduling as a conceptual limitation.
