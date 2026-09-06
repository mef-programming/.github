# M.E.F Programing Service S.R.L

**Native Windows engineering, deterministic AI tooling, and evidence-based model evaluation.**

M.E.F Programing Service S.R.L is an independent software company based in Romania. We bring more than three decades of production C++ and Windows engineering into current work on controlled, auditable AI systems.

Our guiding principle is simple:

```text
Find the evidence.
Read the evidence.
Do not guess beyond the evidence.
```

## Engineering foundation

### SmartFTP and native Windows UI engineering

Founder Mike Walter has worked as a Senior C++ Engineer on [SmartFTP](https://www.smartftp.com/en-us/) since 1996.

The engineering work includes:

- a production Direct2D and DirectWrite rendering pipeline
- application UI systems built on Microsoft's undocumented DirectUI framework
- XML `.ui` definitions describing control structure and behavior
- a custom UxTheme-to-Direct2D renderer for native Windows theme parts
- DirectComposition-based presentation and interaction
- Ribbon, MDI, docking, floating and tabbed pane systems
- custom ListView, ComboBox, CommandBar and other UI controls
- adaptive layouts, DPI-aware behavior and Windows 11 support
- Windows UI Automation and accessibility support for custom-rendered controls
- long-term debugging, compatibility and regression work on an active commercial product

This work was designed and implemented without AI assistance. It is the production engineering foundation behind our current approach to AI tooling: explicit behavior, direct verification, controlled state and long-term maintainability.

## Current work

### Evidence-first AI developer infrastructure

We build infrastructure for tool-using AI systems that need tighter control than prompt-only workflows provide.

Current work covers:

- deterministic project and source-range indexers
- MCP-compatible tools and controlled tool routing
- exact source reads before implementation claims
- bounded execution and explicit failure conditions
- audit, replay and operational visibility
- reduction of unnecessary context and uncontrolled token use

Models may help generate proposals. They do not make final decisions, admit their own output as evidence, or replace direct inspection of the underlying source and system state.

### Specialized language systems - private research

We are developing and evaluating compact, task-specific language models for bounded stages of a larger system, including language understanding, controlled query construction and natural-language generation.

Operational knowledge remains in external data systems instead of being treated as permanently stored in model weights. Deterministic software and human review retain authority over validation and execution.

The active repositories, training material, architecture details and experimental results remain private while this work is under evaluation. We do not publish capability claims without measured evidence.

### ModelBuilder - new project under active development

ModelBuilder is a new native Windows teaching application that makes language-model development accessible to beginners without hiding the underlying process.

Its guided learning path begins with the fundamentals of text and tokenization, then leads through preparing data, building and training a model, evaluating results, fine-tuning and testing the model through direct interaction. Integrated explanations and interactive experiments connect each concept to the system the learner is building.

The application runs locally and is designed to expose intermediate states, measurements and failure conditions instead of presenting model training as a black box.

ModelBuilder remains a private, unreleased project. This public description intentionally omits implementation details and makes no completion claim.

## Public projects

### [mcp-cpp-project-indexer](https://github.com/mef-programming/mcp-cpp-project-indexer)

A deterministic source-range indexer for large, module-heavy C++ and C++20 codebases, implemented as a lightweight Python service.

It maps files, symbols, declarations, includes and module metadata to exact source ranges so an MCP client can locate and read only the relevant source.

It is intentionally not a compiler, LSP replacement, semantic analyzer, refactoring engine or call-graph builder. Metadata locates code; original source provides the evidence.

### [mcp-typescript-project-indexer](https://github.com/mef-programming/mcp-typescript-project-indexer)

A deterministic TypeScript and JavaScript source-range indexer for MCP-based code navigation.

It provides a consistent MCP-oriented surface for locating symbols, files, imports, exports and exact source ranges before an AI system explains or changes code.

Additional language work remains developmental and is not presented here as completed support.

## How we work

1. Define the problem, constraints and evidence required for success.
2. Inspect the existing system and reuse established tools before proposing new infrastructure.
3. Refine ideas through multiple rounds of criticism and comparison; never rely on one model response.
4. Produce a concrete plan before implementation begins.
5. Build the smallest testable increment.
6. Verify behavior directly against source code, runtime state, visual output or registered expectations.
7. Preserve failures, corrections and unresolved results instead of rewriting them into success.

For custom Windows interfaces, verification includes direct interaction, screenshots, high-zoom visual inspection, DPI and theme variation, accessibility-tree inspection and targeted debugging. Automation can support repeatability, but it does not replace expert visual and semantic judgment.

## Design principles

- source-grounded answers
- exact files, symbols and source ranges
- compact metadata before source reads
- deterministic checks before model judgment
- no fake semantic certainty
- no hidden call-graph or behavior claims
- explicit clarification, rejection and inconclusive outcomes
- local-first developer workflows
- MCP-compatible tool surfaces
- human authority over promotion and execution
- measurable behavior before scaling

## Company

**M.E.F Programing Service S.R.L**  
Independent software company - Romania

Founder and Lead Engineer: **Mike Walter**

Website: [www.mef-programming.eu](https://www.mef-programming.eu/)  
LinkedIn: [Mike Walter](https://www.linkedin.com/in/mike-walter-40b59224b/)  
Contact: [mw@mef-programming.eu](mailto:mw@mef-programming.eu)
