# M.E.F Programing Service S.R.L

**M.E.F Programing Service S.R.L** is an independent software company based in Romania, focused on AI-assisted developer tooling, MCP project indexers, and controlled tool-use workflows for software engineering.

We build tools that help AI systems navigate real codebases more accurately by separating three concerns:

```text
Find code.
Read code.
Do not guess code.
```

## Current focus

Our current work is centered around deterministic project indexers and MCP-based code navigation.

Instead of asking an AI model to read large files blindly, our tools expose compact project metadata first:

* files
* symbols
* imports
* modules
* source ranges
* project structure
* management/status information

The model can then request the exact source range it needs before making implementation claims.

This keeps AI-assisted code analysis more focused, more reproducible, and less dependent on broad context dumping.

## Projects

### mcp-cpp-project-indexer

A Python-based C++ source-range indexer for large, module-heavy C++ and C++20 projects.

It maps files, symbols, data declarations, includes, and C++20 module metadata to exact source ranges so MCP clients can locate and read only the relevant code.

It is not a compiler, LSP replacement, semantic analyzer, refactoring engine, or call-graph builder.

Repository:
[mcp-cpp-project-indexer](https://github.com/mef-programming/mcp-cpp-project-indexer)

### MCP Project Indexers

A multi-language project-indexer family built around a shared TypeScript core.

The goal is to provide a consistent MCP/HTTP/management surface across multiple programming languages, with language-specific parsing and symbol extraction layers.

Current and planned language targets include:

* TypeScript / JavaScript
* Python
* C#
* Go
* Java
* Rust

Repository:
[mcp-typescript-project-indexer](https://github.com/mef-programming/mcp-typescript-project-indexer)

## Design principles

We prefer deterministic routing facts over generated summaries.

AI tools should not claim behavior from metadata alone. Metadata answers where code is. Source ranges show what the code says. The model can then reason from the source it actually read.

Core principles:

* source-grounded answers
* exact line ranges
* compact metadata before source reads
* no fake semantic certainty
* no hidden call-graph claims
* local-first developer workflows
* MCP-compatible tool surfaces
* management/status endpoints for operational visibility

## Company

Website:
https://www.mef-programming.eu

Contact:
[mw@mef-programming.eu](mailto:mw@mef-programming.eu)

Founder:
Mike Walter
