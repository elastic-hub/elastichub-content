---
title: Structuring Front Matter and Document Metadata
layout: doc
category: Guidelines
audience_roles:
  - Editor
  - Program Manager
activities:
  - Writing specifications
  - Publishing releases
tool: PubHub
---

## Context

Front matter establishes the identity, purpose, and boundaries of a technical specification.

In standards work, readers rely on front matter to understand **what a document is**, **who it is for**, **what it covers**, and **how it should be interpreted** before engaging with normative content. Poorly structured front matter often leads to confusion during review, misinterpretation by implementers, and repeated clarification requests.

This guidance explains how to structure **front matter and document metadata** for specifications published using PubHub (formerly MD2HTML), ensuring clarity and consistent rendering in HTML and PDF outputs.

---

## What This Guidance Enables

Applying this guidance helps you to:

- Clearly identify a specification and its publication status
- Provide readers with context before normative content begins
- Define the purpose and boundaries of the document
- Ensure front matter renders consistently in HTML and PDF outputs
- Align published documents with governance and release expectations

---

## When This Guidance Is Relevant

This guidance applies when:

- Preparing a technical specification for formal publication
- Publishing candidate or approved releases
- Introducing a document to a broader audience
- Establishing stable document identity across versions

It is especially important for documents intended for long-term reference.

---

## When This Guidance Is Not Required

This guidance may not be necessary when:

- Content is exploratory or internal
- Documents are informal discussion drafts
- The material is not intended for external publication

However, introducing front matter early can reduce rework as documents mature.

---

## What Constitutes Front Matter

Front matter typically includes:

- **Document metadata** (defined outside the content)
- **Introduction**
- **Scope**

These elements appear before normative sections and are intended to orient the reader.

---

## Document Metadata

Document metadata defines the **identity** of the specification and is provided through the document assembly configuration (e.g. `index.yaml`).

Common metadata includes:

- Document title
- Version
- Publication status
- Publishing organization
- Publication date
- Output identifiers and watermarks

This metadata is rendered on the front page of published HTML and PDF outputs.

Metadata should be stable, intentional, and aligned with the organization’s release process.

---

## Introduction Section

The **Introduction** provides a high-level overview of the specification.

It should:

- Explain the problem or requirement the specification addresses
- Describe the purpose of the document
- Establish relevance without technical detail
- Use clear, neutral, and formal language

The Introduction sets context for the reader but does not define requirements.

---

## Scope Section

The **Scope** section defines the boundaries of the specification.

It should:

- Clearly state what the document covers
- Identify the intended audience
- Describe any limitations or exclusions
- Avoid detailed technical descriptions

A well-defined scope reduces ambiguity and prevents misinterpretation of normative content.

---

## Ordering of Front Matter

Front matter should appear in the following order:

1. Document metadata (front page)
2. Introduction
3. Scope

Normative content should begin only after front matter is complete.

Maintaining a consistent order improves readability and review efficiency.

---

## Recommended Practices (DOs)

- Provide complete and accurate document metadata
- Keep the Introduction concise and non-technical
- Define scope explicitly and unambiguously
- Align metadata with formal release decisions
- Review front matter at each release stage

---

## Common Mistakes to Avoid (DON’Ts)

- Do not mix normative requirements into the Introduction
- Do not leave scope implicit or undefined
- Do not change document identity fields unintentionally between releases
- Do not duplicate metadata information inside content sections

These issues frequently cause confusion during review and publication.

---

## How PubHub Supports Front Matter

PubHub supports publishing outputs; governance and editorial decisions remain with the organization. It does this by:

- Renders document metadata consistently in HTML and PDF
- Preserves the structure and order defined by the authors
- Supports reproducible outputs across published versions

---

## Related Guidance

- Publishing Structure — How Specifications Are Assembled
- Defining Document Assembly Using `index.yaml`
- Managing Normative and Informative References
- Managing Terminology, Definitions, and Abbreviations

---

## Summary

Front matter and document metadata provide the foundation for understanding a technical specification.

By structuring these elements clearly and consistently, standards organizations improve readability, reduce ambiguity, and support reliable publication.

PubHub supports this process by rendering front matter predictably—without imposing editorial or governance decisions on the content.