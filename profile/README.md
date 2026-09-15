# ORINOCO-Lite

ORINOCO-Lite helps research groups adopt the ORINOCO approach to structured, linked metadata and website generation without needing to run the full ORINOCO infrastructure stack all the time.

![ORINOCO self-hosted components](https://hub.psychoinformatics.de/orinoco/artwork/src/branch/main/selfhost_components.svg)

## What this organization is about

This organization develops a lightweight, GitHub-native path for building and maintaining rich knowledge bases that can drive research group websites, CVs, project reports, and related outputs.

The goal is to make efficient use of linked-web technologies, established ontologies, and ORINOCO-compatible metadata models while keeping the deployment story approachable for teams already comfortable with GitHub.

## How ORINOCO-Lite works

Instead of requiring permanently deployed heavy infrastructure, ORINOCO-Lite reuses familiar GitHub capabilities:

- **GitHub repositories** store metadata records and associated content
- **GitHub Actions** provide ephemeral workflow-time services, including `dump-things-server` when needed
- **GitHub Pages** serves generated websites
- **git-annex** can manage larger content across supported storage backends
- **shacl-vue** can support advanced metadata editing workflows

This makes it possible to keep site-specific repositories self-contained and actionable while still following ORINOCO-compatible schemas and graph-oriented concepts.

## Main building blocks

### `orinoco-lite-dev`

A development home for reusable ORINOCO-Lite components, including:

- the `orinoco-lite` CLI
- reusable GitHub Actions for data logistics inside workflows
- the specification for `site-specific/` content and metadata layout
- tooling and apps such as `packages/curation-review-app` for PR-driven metadata curation

### Template repositories

ORINOCO-Lite templates are intended to help bootstrap new sites quickly while reusing the shared tooling, actions, and conventions developed here.

### `site-specific/` repositories

Each deployment keeps its own metadata records and related materials in a dedicated repository, potentially linked into a template-based site via submodules.

These repositories are meant to follow the same general schemas and concept models while organizing files in a practical filesystem hierarchy.

## Immediate targets

- [`con-site-specific`](https://github.com/ORINOCO-Lite/con-site-specific) for the Center for Open Neuroscience
- `psychoinformatics-site-specific` to help reproduce and demonstrate the Psychoinformatics group website workflow
- `repronim-site-specific` as an early adopter path for ReproNim

## Principles

ORINOCO-Lite puts special emphasis on [STAMPED principles](https://stamped-principles.org), especially:

- **Self-containment**
- **Tracking**
- **Actionability**

The aim is for `site-specific/` repositories to contain the information needed to materialize and serve complete website content from versioned records.

## Relationship to upstream ORINOCO

This organization may also host forks or mirrors of upstream projects that need fixes or extensions to support the lightweight workflow, including related ORINOCO ecosystem components.

## Follow the effort

If you are interested in knowledge-graph-driven research websites, metadata curation, or GitHub-based scholarly infrastructure, explore the repositories in this organization and follow the ongoing work.
