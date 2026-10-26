# PostCode Research Project

> *Humans should be able to practice the discipline of software design and architecture in collaboration with agents that implement the software, without needing to be programmers themselves.*

The PostCode Research Project investigates how best to support that practice. Capable coding-agent conversations already allow substantial software-design work without the human reading source code. The research asks what further representations, interactions, and tools—if any—can improve that collaboration, including for people who have not learned to read or write programming-language source.

One leading hypothesis is that shared visual architectural representations, grounded in partial, qualified, retained understanding, can help people reason about designs, examine implementations, and revisit architectural questions from different perspectives. The research draws on established software-architecture concepts and visual notations without assuming that any representation provides a complete or authoritative account of the software.

The project explores these questions by building the [PostCode application](https://github.com/ronen/postcode), which presents task-appropriate views of program structure, behavior, history, rationale, and other evidence while preserving the provenance, epistemological status, and limitations of their content.

The research proceeds by studying PostCode during real software development. The application is intended to record and export observations, including relevant interaction events and contemporaneous user reports. This evidence stream will support later analysis of how PostCode is used, where it succeeds or fails, and how the design should evolve.

The application is developed in a separate repository so that it can stand alone as a software project. Once minimally functional, it will be used to understand and supervise its own further development.

## Status

See [`STATUS.md`](STATUS.md) for the project's current status.

See [`ROADMAP.md`](ROADMAP.md) for planned work and candidate directions.

## Documents

- [`research.md`](research.md) defines the research motivation, questions, and possible contributions.
- [`product-design.md`](product-design.md) describes the conceptual product design. It is copied verbatim into the application repository as `foundation/product-design.md`, where the adopted version governs application design and development. Revisions are adopted explicitly; see [application repository setup](application/repository-setup.md).
- [`methodology.md`](methodology.md) describes how building and using PostCode can produce research evidence.
- [`research-strategy.md`](research-strategy.md) describes how findings may shape the broader research direction and publication strategy.
- [`related-work.md`](related-work.md) records relevant prior work and comparisons.
- [`candidate-conventions.md`](candidate-conventions.md) collects design conventions that may be useful during PostCode-mediated development.
- [`application/repository-setup.md`](application/repository-setup.md) describes the minimal requirements for the application repository to participate in the PostCode research project.

## License

This project is licensed under the [Apache License 2.0](LICENSE).
