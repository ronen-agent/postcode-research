# Application Repository Setup

This document is for the human establishing or reviewing the PostCode application repository. It describes material to adopt into that repository. It is not itself an operative instruction for application-development agents.

## `README.md`

The repository's `README.md` should initially contain:

```markdown
# PostCode

PostCode is a software-development environment for practicing software design and architecture with coding agents. Its human-facing interface uses qualified architectural representations rather than presenting programming-language source.

PostCode presents task-appropriate views of program structure, behavior, history, rationale, and other evidence. Projections preserve their provenance, epistemological status, and limitations so that derived facts, recorded assertions, observations, and interpretation are not presented as equally authoritative.

As an initial simplification, PostCode's projections and views are read-only. Humans continue to direct program changes by instructing coding agents in prose.

See [`foundation/product-design.md`](foundation/product-design.md) for the conceptual product design.

## Observability

To support the [PostCode Research Project](https://github.com/ronen/postcode-research), PostCode records and exports observations, including relevant interaction events and contemporaneous user reports, for later analysis.
```

## `foundation/`

The repository should contain the following adopted foundation material:

```text
foundation/
  README.md
  product-design.md
  task-records.md
```

The adopted documents should be copied verbatim from the following research-project documents:

- `foundation/product-design.md` from [`../product-design.md`](../product-design.md);
- `foundation/task-records.md` from [`task-records.md`](task-records.md).

`foundation/README.md` should contain:

```markdown
# Adopted Foundation

The documents in this directory are adopted foundation material for developing PostCode. Application-development agents should read and follow them where applicable, but must not modify them as part of ordinary development. The human may explicitly adopt revised versions.

## Governing Documents

- [`product-design.md`](product-design.md) is the adopted governing conceptual description of PostCode. It defines the product hypothesis and the principles the application must preserve. It is aspirational about implementation status; application plans and decisions must conform to it unless the human explicitly authorizes a foundation revision.
- [`task-records.md`](task-records.md) defines the durable application-development records required by the PostCode Research Project. The application repository owns the operative task protocol that satisfies those requirements.
```

## `AGENTS.md`

The repository's `AGENTS.md` should include the following elements:

- **Task protocol**

  The application repository should maintain its own operative task protocol at an app-owned location. `AGENTS.md` should identify that protocol, require application-development agents to follow it, and state that it must satisfy `foundation/task-records.md`.

- **Adopted foundation**

  ```markdown
  ## Adopted Foundation

  Treat the documents under [`foundation/`](foundation/README.md) as adopted, governing material. Read and follow the documents relevant to the work. Do not modify any file under `foundation/` unless the human explicitly asks to revise or adopt foundation material.
  ```
