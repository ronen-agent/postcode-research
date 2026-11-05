# PostCode: Research Methodology

This document describes how building and using PostCode can produce trustworthy research evidence.

The research questions are described in [`research.md`](research.md). The conceptual product design through which the research is conducted is described in [`product-design.md`](product-design.md).

## 1. Methodological Stance

PostCode is a development project conducted as formative research.

Building the system is necessary because many of the relevant questions cannot be answered in advance: which projections prove useful, which architectural questions remain inadequately supported, how much qualification users need, and which abstractions survive contact with real software.

The initial method is therefore sustained use, observation, and revision rather than a fixed efficacy experiment.

To preserve evidence from that use, designated formative episodes should capture enough interaction history and contemporaneous reporting to reconstruct what happened and support later interpretation. This is formative evidence, not a comprehensive behavioral dataset. The minimum requirements and limitations are described in [Formative Evidence Capture](#formative-evidence-capture).

The central formative question is:

> **What is required for representations to support useful human architectural practice with coding agents, and what do they contribute beyond capable agent chat?**

The governing methodological loop is:

```text
build
  ↓
use during real development
  ↓
observe limitations, friction, success, and surprise
  ↓
formulate findings based on the evidence
  ↓
revise design, research questions, or roadmap
  ↓
use again
```

The process is directed by what the evidence supports. Positive, negative, limiting, mixed, and unexpected findings should all be allowed to redirect the work.

## 2. Formative Use

Formative use should deliberately seek variation across projects, tasks, architectures, domains, and programming languages as suitable opportunities arise. No single context is representative; contrasting cases help expose context-specific assumptions and reduce the risk of optimizing PostCode for one setting. The method does not require comprehensive coverage of every dimension.

Each formative research episode—a bounded period of use analyzed as a unit—should identify the PostCode version and investigated repository states. When the episode produces research records, it should keep the relevant version stable for the episode and deliver those records to a designated research destination.

Formative use should include both inspection-only investigations and development tasks. Inspection-only use isolates PostCode's support for understanding software; development tasks additionally exercise direction, change supervision, and interaction with coding agents.

Differences among these contexts should be formulated as findings and fed back into the methodological loop.

### 2.1 PostCode on PostCode

PostCode must initially be developed without the benefit of PostCode itself. Once it becomes minimally usable, it can be introduced into its own continued development. This bootstrapping transition creates an unusually tight formative context: the tool, its design, and the software being investigated can evolve together.

Using PostCode while developing PostCode provides sustained access to the developer's own questions, intentions, and moments of friction.

It is especially useful for discovering:

- missing lenses and projection capabilities;
- unsuitable presentation choices;
- awkward navigation and failures to preserve relevant views, their lineage, or retained architectural understanding;
- failures in agent-context exchange;
- distinctions the current design vocabulary does not capture;
- ways in which PostCode and the software developed through it co-adapt.

This context is primarily formative self-study, not an efficacy experiment. It is intended to expose missing representations, bad abstractions, insufficient precision, awkward interactions, and limits of the underlying idea.

It also has important limitations. The developer is motivated to exercise PostCode and can change both the tool and its subject in response to friction. It cannot by itself establish how other developers would behave or whether PostCode improves on capable coding-agent chat.

<a id="existing-project-development"></a>

### 2.2 Continued Development of an Existing Project

One useful formative context is to apply PostCode during the continued development of an existing project already familiar to the investigator. PostCode's author has a suitable pre-existing personal project. It remains in progress and undeployed, so it presents genuine development needs that were not invented to exercise PostCode. It also has no specific delivery deadline, allowing some tolerance of formative friction without interfering with time-critical work.

Prior familiarity makes it possible to compare PostCode's projections with an established understanding of the system, but remains a confound when interpreting the resulting observations. The project's specific product details are not relevant here. As with every formative context, however, characteristics of its domain and development circumstances should be considered when interpreting observations.

This context can expose:

- assumptions created by PostCode's own architecture;
- difficulty introducing PostCode during continued development;
- interactions with pre-existing design and decision artifacts;
- projections needed for work in a different domain;
- whether PostCode supports ordinary tasks rather than only self-directed demonstrations.

Existing-project development is not evidence about unfamiliar-user comprehension.

### 2.3 Ab initio project

Developing a separate new project with PostCode present from its inception tests whether projections can support the creation and continued supervision of software, rather than only the reconstruction of an existing implementation.

Unlike PostCode-on-PostCode, the tool and its subject are distinct. Unlike existing-project development, the project begins without a pre-existing implementation or development history. This context can expose whether intentions, rationale, requirements, and conceptual structure can be captured as they arise; whether PostCode's existing projection capabilities are useful for guiding a new project's early development; and how PostCode-mediated supervision affects the software being produced.

### 2.4 Unfamiliar open-source software

Unfamiliar OSS projects provide software whose development PostCode did not influence and for which the investigator lacks a pre-existing mental model.

They can test whether PostCode can:

- establish enough orientation to begin a useful investigation;
- derive useful concepts from the evidence an arbitrary repository provides;
- expose where missing rationale or history limits projection;
- avoid relying on private conventions shared by PostCode and PostCode-native software;
- generalize across application domains;
- accommodate substantially different software architectures;
- identify concepts that generalize across programming languages;
- identify concepts and mechanisms that remain language-specific.

OSS use should involve genuine questions or development tasks where possible. Artificial tours of repositories may reveal projection defects, but they provide weaker evidence about sustained usefulness.

## 3. Evaluating Projection Capabilities

Every lens, projection capability, recurring view construction, or representation-selection rule introduced into PostCode embodies a provisional claim that it will help satisfy some human information need. Formative use should evaluate that claim rather than assume usefulness from the apparent reasonableness of the design.

Not every small capability needs a separately formalized hypothesis. When a capability has a consequential or recurring role, however, its intended information need and expected contribution should be clear enough to compare with what happens in use.

Evaluate architectural representations in genuine design or investigation tasks, using established structural or behavioral notations where useful. Compare against capable coding- or design-agent chat with repository access, ordinary diagrams, and retained notes.

Interpret evidence using the three analytic levels identified in the [research direction](research.md#specialized-architectural-expertise): usefulness for direct human investigation, quality of architectural accounts, and contribution to collaborative architectural practice. Evidence at one level does not establish the others, and an episode or contribution need not address all three.

When investigation compares architectural accounts, preserve what each account concerns—such as an implemented state, a hypothetical alternative or an intended design—together with its provenance and qualifications. Preserve observations as separately scoped evidence rather than treating them as another account modality. Assess the comparison's claims and usefulness separately from the quality or feasibility of the designs being compared.

Relevant observations include:

- the task, information need, and contribution the capability was intended to make;
- how the result entered the investigation relative to human intent and whether system-initiated investigation contributed;
- how the result was constructed, including relevant evidence, qualifications, provenance, and composition;
- whether it satisfied the information need or supported a useful next step;
- whether the representation's textual, structured, or visual form helped expose relationships, consequences, or gaps beyond comparable conversation, ordinary agent-generated diagrams, and retained notes;
- whether retained knowledge was reused, revised, compared, or challenged without disguising its evidentiary basis;
- whether architectural change review distinguished what changed from whether the implementation realized the intended design;
- what the human pursued next, including requests for more detail, alternative representations, reported inadequacy, or abandonment;
- which information was useful, missing, misleading, or unnecessarily prominent;
- whether qualifications and limitations were understood and trusted; and
- which contextual differences appear consequential.

These observations should combine reconstructable interaction evidence with contemporaneous annotations or other direct reports, as described in [Formative Evidence Capture](#formative-evidence-capture). More detailed candidate observations are retained in [`notes/formative-evidence-candidates.md`](notes/formative-evidence-candidates.md). Findings may support retaining, revising, replacing, or removing a capability and may motivate changes to the application, roadmap, research questions, or conceptual design.

## 4. Interpreting Formative Use

To gather formative evidence, the developer will deliberately use PostCode during real development work and tolerate some friction before deciding whether the available representations suffice.

That tolerance is useful during formative self-study because sustained use exposes missing representations and awkward interactions. It also means that continued use alone is not an unbiased measure of PostCode's success.

When PostCode creates friction, the useful question is not merely whether it failed. Ask:

> **Was the problem in lens selection, projection capability, presentation, interaction, available evidence, or the underlying idea?**

Possible interpretations include:

- the needed lens does not exist;
- the lens exists but lacks necessary information;
- the projection contains the information but the selected presentation shows it poorly;
- the system selected an inappropriate lens or presentation;
- the available repository evidence cannot support the desired claim;
- the available representations cannot support the architectural reasoning or verification needed for this question;
- a capable conversational agent with ordinary diagrams and notes provides the same help without a dedicated PostCode capability;
- the projection-based approach is poorly suited to the activity.

Formative use should also help determine which textual results belong in transient conversation, which should become retained views, and which should contribute to longer-lived retained architectural understanding.

### 4.1 Reported Limitations and Inadequacy

When reported uncertainty or a limitation in a projection influences development, formative observation should preserve what was reported and any stated cause, how it was used, and what effects followed. The development response—including any change to the program or available evidence, or a decision to continue without change—is itself part of the evidence. If the program was changed to enable stronger projection guarantees, analysis should not assume that the change was beneficial or harmful. If the finding instead motivates a change to PostCode, that change is a methodological intervention: the original observation should be preserved, and subsequent observations interpreted in relation to the revised PostCode version.

Reports that a view or explanation is inadequate should require neither a diagnosis nor a written justification. Record such feedback with the information need, view, qualifications, captured basis, and relevant surrounding activity where available. Feedback indicates a perceived shortcoming, not necessarily an incorrect claim; absence of feedback does not establish adequacy.

Activity outside PostCode cannot reliably be observed. Voluntary contemporaneous accounts can add context, but recorded activity cannot establish every unmet need or action taken when PostCode was insufficient.

### 4.2 Evaluating Conventions

Conventions and other deliberate changes to the development setting are methodological interventions as well as possible engineering choices. Record their rationale, timing, and intended role where possible. Interpretation should distinguish independently useful conceptual clarity from tool-relative projectability, and effects of an intervention from properties that already existed.

Local adoption creates an opportunity for observation; it does not establish benefit, necessity, causation, or transferability. Candidate conventions and more detailed evaluation questions are retained in [`notes/candidate-conventions.md`](notes/candidate-conventions.md).

<a id="6-formative-logging"></a>
<a id="formative-evidence-capture"></a>

## 5. Formative Evidence Capture

Formative evidence should combine reconstructable interaction history with contemporaneous subjective observations. The conceptual product capability is described in [Research Observation Support](product-design.md#research-observation-support).

At minimum, a research episode should preserve or reference:

- the task and information need;
- the PostCode version and investigated repository states;
- consequential requests, views, projections, captured bases, qualifications, and limitations;
- relevant choices, navigation, comparisons, and agent-context interactions;
- explicit inadequacy reports or contemporaneous annotations; and
- what happened next, where that is available and material to interpretation.

Automatic capture is preferable where retrospective reconstruction would be unreliable, but it need not be exhaustive and may be supplemented by task records, external conversations, or manual notes. Additional fields should be driven by the research question; [`notes/formative-evidence-candidates.md`](notes/formative-evidence-candidates.md) retains a broader candidate inventory.

The resulting record is primarily a **design instrument**, not an unbiased behavioral dataset. Instrumentation may affect behavior, subjective reports are not standardized effectiveness measures, and the investigator decides when to persevere, report inadequacy, or revise the system.

## 6. From Formative Evidence to Design Knowledge

Individual events do not automatically constitute findings. A design finding should remain traceable through a chain such as:

```text
consequential problem or information need
  → design conjecture and implemented response
  → formative episode or implementation experience
  → recorded evidence and contrary cases
  → bounded interpretation
  → transferable design knowledge or revised question
```

Analysis should distinguish artifact behavior, architectural-account quality, design knowledge, bounded experience, and claims about developer behavior. It should triangulate interaction records, contemporaneous reports, development artifacts, repository history, and independent checks where appropriate rather than treating any single source as decisive.

Findings should identify the mechanism believed to matter, the context in which it appeared, relevant interventions and alternative explanations, contrary or failed cases, and the boundary of the supported claim. The investigator's simultaneous roles as designer, implementer, user, and analyst should remain explicit.

Transferability comes from sufficiently detailed problem framing, design rationale, mechanism, evidence, context, and limitations so that others can judge applicability—not from treating the formative cases as a representative sample. Findings may revise the product design, application, roadmap, methodology, research questions, or prospective contribution.

<a id="8-evidence-and-claim-scope"></a>
<a id="evidence-and-claim-scope"></a>

## 7. Evidence and Claim Scope

The methodology distinguishes forms of evidence by the claims they can support.

The governing distinction is:

> **Formative use can produce design findings and hypotheses; independent evaluation is required for general claims about developer behavior.**

The restriction on displaying source applies to PostCode's human-facing interface, not to independent research validation. Architectural claims should be assessed separately against suitable implementation evidence, tests, runtime observations, or expert inspection. User satisfaction and the absence of inadequacy reports do not establish that an explanation is correct.

### 7.1 Formative self-study

Evidence from sustained formative use, reconstructable episodes, contemporaneous inadequacy reports, other observations, and resulting design changes can help determine what is required to support architectural investigation. It supports design findings, bounded observations about the developer's experience, and hypotheses for later investigation.

Because this self-study involves a developer with extensive programming experience, using a code-independent interface does not test whether someone without programming-language proficiency could exercise comparable architectural judgment. The [unfamiliar-language challenge](ROADMAP.md#46-unfamiliar-language-challenge) offers a partial test of reliance on implementation-language knowledge, but is not a substitute for studying practitioners who have not learned conventional programming.

### 7.2 External exploratory use

External users can reveal assumptions caused by the author's prior knowledge, vocabulary, workflow, and willingness to tolerate friction. Exploratory use can refine tasks, instrumentation, and hypotheses without yet supporting broad comparative claims.

### 7.3 Formal user studies

If a specific mature claim warrants them, user studies can support appropriately scoped findings about developer behavior and whether architectural tasks can be completed without programming-language proficiency, including preference, effectiveness, speed, comprehension, confidence, and trust. They are an optional extension rather than the expected endpoint of the initial program, and should identify the relevant population, tasks, methods, outcomes, and development contexts rather than act as a single final verdict on PostCode.

All findings should remain scoped to their evidence. Negative and mixed findings should be treated with the same discipline as positive ones; a technique may be useful for one task, repository, language, or development context and unhelpful for another.

<a id="84-comparisons-and-reuse-assessments"></a>

### 7.4 Comparisons and reuse assessments

Comparative evaluation should preserve the three levels distinguished in [Evaluating Projection Capabilities](#3-evaluating-projection-capabilities). Consequential factual claims and design outcomes require assessment independent of participants' satisfaction with the investigation.

When related systems are assessed, distinguish the question being asked and the evidence required:

- **Analysis validation and reuse:** inspect versioned implementations and exercise representative cases to establish what their results mean, which guarantees and limitations apply, and whether integration can preserve PostCode's contracts. Similar terminology or deterministic execution alone does not establish equivalent semantics. Reuse assessment also considers integration effort and support for formative evidence capture.
- **Interface comparison:** compare identified versions on specified human tasks, with the information, tools, setup, and assistance available in each condition made explicit. A capable conversational coding or design agent with repository tools, ordinary diagrams and retained notes is a primary comparator, rather than a deliberately impoverished text-only chat. When comparing code-independent architectural practice, neither condition should expose programming-language source to the human; differences in design agents' source access must be treated as an explicit experimental variable. Select comparators for the question under study; an analysis provider need not be a suitable interface comparator, and a useful interface need not supply reusable analyses.
- **Sustained-use evidence:** observe understanding, direction, and supervision across development episodes and changing program states. Success on isolated questions or benchmark cases does not establish viability as a routine working surface.

Project documentation establishes reported capabilities, not demonstrated guarantees or effectiveness. Agent-monitor benchmarks may supply useful cases for analysis or supervision, but model performance on them does not itself establish human usefulness. Comparative self-study retains the limitations described above; general claims about developer behavior still require independent evaluation. Record the assessment's version, scope, evidence, and unresolved questions so that reuse decisions and research claims can be judged separately.

<a id="9-relationship-to-development-workflows"></a>

## 8. Relationship to Development Workflows

This methodology overlays software-development workflows. Its evidence-capture process does not prescribe how the projects in which PostCode is used plan and implement their work or require access to particular planning, task, or outcome mechanisms.

<a id="91-development-of-postcode-itself"></a>

### 8.1 Development of PostCode Itself

PostCode's own application development is a special case. Implementing lenses, projections, presentations, and supporting infrastructure may expose considerations that affect the project-level design, research strategy, methodology, roadmap, or other overview documents, independently of any observations produced by using PostCode.

To keep those considerations from being lost, the [task-record requirements](application/task-records.md) require the application repository to preserve durable records of substantive implementation tasks. The application repository owns the operative protocol that produces those records. They are application-development artifacts rather than observations from using PostCode. In addition to examining formative evidence captured during PostCode-on-PostCode use, the research process should examine concluded application-task outcomes for possible implications.
