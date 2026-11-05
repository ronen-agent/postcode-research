# PostCode Research Project

> *Humans should be able to practice the discipline of software design and architecture in collaboration with agents that implement the software, without needing to be programmers themselves.*

The PostCode Research Project asks how to facilitate that practice: what representations, interactions, tools, and forms of collaboration help humans understand, design, direct, and evaluate software without requiring programming-language proficiency?

Today's capable general-purpose agents already provide substantial help, at least for experienced developers, by inspecting repositories, explaining software, and discussing design alternatives without requiring the human to read source. The follow-up question is what specialized capabilities, if any, can improve on that starting point.

The project investigates these questions by building the [PostCode application](https://github.com/ronen/postcode), designed to provide specialized, evidence-grounded architectural investigation and retained understanding for humans working alone or in collaboration with agents to understand, design, and evaluate software. Humans and agents may conduct their conversations elsewhere while using PostCode's partial, qualified accounts as shared working resources. Those accounts may be textual, structured, or visual. They draw on established architectural concepts without claiming to form a complete or authoritative model of the software.

The research distinguishes three questions: whether PostCode supports useful direct human investigation; whether its specialization produces better architectural accounts than capable general-purpose agents; and whether using those accounts improves human–agent architectural practice and its outcomes. PostCode may support understanding implemented software, examining hypothetical alternatives, recording intentions, reviewing implementations, and revisiting architecture from different perspectives. Comparisons among implemented states, hypothetical alternatives, and intended designs must preserve their different meanings and evidentiary bases.

The research proceeds by studying PostCode during real software development. The application is designed to record and export relevant interaction events and contemporaneous user reports for later analysis of its use, limitations, successes, and design evolution. It is developed in a separate repository so that it can stand alone as a software project; using it during its own continued development provides one important formative context.

## Status

See [`STATUS.md`](STATUS.md) for the project's current status.

See [`ROADMAP.md`](ROADMAP.md) for planned work and candidate directions.

## Documents

- [`research.md`](research.md) defines the research motivation, questions, and possible contributions.
- [`product-design.md`](product-design.md) describes the conceptual product design. It is copied verbatim into the application repository as `foundation/product-design.md`, where the adopted version governs application design and development. Revisions are adopted explicitly; see [application repository setup](application/repository-setup.md).
- [`methodology.md`](methodology.md) describes how building and using PostCode can produce research evidence.
- [`research-strategy.md`](research-strategy.md) describes how findings may shape the broader research direction and publication strategy.
- [`related-work.md`](related-work.md) records relevant prior work and comparisons.
- [`application/repository-setup.md`](application/repository-setup.md) describes the minimal requirements for the application repository to participate in the PostCode research project.

The [`notes/`](notes/) directory holds not-yet-adopted ideas, background material, and other non-primary documents:

- [Candidate conventions for PostCode-mediated development](notes/candidate-conventions.md), retained for consideration rather than as endorsed practices.
- [Cross-paradigm stress tests for architectural representations](notes/cross-paradigm-architectural-concepts.md), an exploratory proposal for testing conceptual portability across language paradigms, not scheduled work or an application-language commitment.
- [Architectural expertise and comparative investigation directions](notes/architectural-expertise-directions.md), illustrative roles, experiments, applications, and scope boundaries arising from the governing research direction.

## License

This project is licensed under the [Apache License 2.0](LICENSE).
