# PostCode Research Project

> *Humans should be able to practice the discipline of software design and architecture in collaboration with agents that implement the software, without needing to be programmers themselves.*

This is a research aspiration, not an established possibility. It asks whether people can develop and exercise architectural judgment without needing proficiency in reading or writing conventional programming-language source. They would still need substantial knowledge of computation, software behavior, design principles, and their consequences.

The PostCode Research Project investigates how to support that practice, and **what can improve it beyond capable natural-language collaboration with coding agents**. Its current leading hypothesis is that shared visual architectural representations, developed through progressive investigation and grounded in partial, qualified, retained knowledge, might help people reason about designs, examine implementations, and revisit architectural questions from different perspectives.

The project builds the [PostCode application](https://github.com/ronen/postcode) to explore these hypotheses. Representations should draw where useful on established software-architecture concepts and visual notations, without pretending to constitute a complete or authoritative model of the software. The application preserves the provenance, epistemological status, and limitations of what it presents. Initial visual representations remain read-only; humans and agents develop and revise their understanding through conversation.

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
