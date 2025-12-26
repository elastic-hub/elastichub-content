---
title: Preparing HTML and PDF Outputs
layout: doc
category: Guidelines
audience_roles:
  - Editor
  - Program Manager
  - Chair
activities:
  - Publishing specifications
  - Preparing releases
tool: PubHub
---

## Context

Publishing a technical specification is not only about producing an output file — it is about ensuring that the published content is **consistent, reliable, and interpretable** across formats.

In PubHub, the authoritative source of a specification is the **Markdown content itself**. HTML, PDF, and other output formats are derived representations of that source.

This guidance explains what “good output” means in this model, what PubHub guarantees, and what remains the responsibility of the standards organization.

---

## The Core Principle: Markdown as the Source of Truth

In PubHub, Markdown is the **single source of truth**.

This means:

- The content authored in Markdown must not differ by output format  
- HTML, PDF, and other formats must reflect the *same structure and meaning*  
- No format introduces or removes content implicitly  

If content appears differently across outputs, this is treated as a **structural issue in the source**, not a publishing variation.

---

## What “Good Output” Means

A “good” published output is one where:

- All content present in the Markdown source appears in every output format  
- Section structure, references, terminology, and ordering are preserved  
- Readers can rely on the document regardless of whether they access HTML, PDF, or another format  

Visual presentation may vary slightly between formats, but **content fidelity must not**.

---

## Structural Fidelity Over Visual Fidelity

PubHub prioritizes **structural fidelity**, not pixel-perfect visual identity.

This approach ensures that:

- Specifications remain consistent across formats  
- Content can evolve without format-specific rewrites  
- New output formats can be supported without reauthoring documents  

The goal is reproducibility and clarity, not format-specific optimization.

---

## Relationship to Authoring Guidelines

Output quality is a direct result of how source content is authored and structured.

Consistent outputs depend on:

- Clear document assembly definitions  
- Explicit front matter and metadata  
- Proper handling of references  
- Consistent terminology and abbreviations  
- Intentional inclusion of legal and licensing content  

This page should be read alongside:

- Publishing Structure — How Specifications Are Assembled  
- Defining Document Assembly Using `index.yaml`  
- Structuring Front Matter and Document Metadata  
- Managing References (Normative & Informative)  
- Terminology, Definitions, and Abbreviations  
- Managing Legal Disclaimers and Licenses  

---

## What PubHub Guarantees

PubHub guarantees that:

- The same Markdown source is used for all output formats  
- Content is rendered consistently according to its structure  
- Ordering, references, and terminology are preserved  
- Published outputs are reproducible from version-controlled sources  

PubHub does **not** alter content based on output format.

---

## What PubHub Does *Not* Guarantee

PubHub does not guarantee:

- Editorial correctness  
- Semantic or technical correctness  
- Legal correctness or compliance  
- Accessibility compliance beyond structural markup  
- Visual perfection across browsers, viewers, or devices  

Responsibility for content quality and correctness remains with the standards organization.

---

## Output Formats

Out of the box, PubHub produces:

- HTML outputs  
- PDF outputs  

The same source model supports additional formats such as ODF, OOXML, or others as required by the community. These formats follow the same principle: **derive from the same authoritative source without altering content**.

---

## Why This Model Matters

Treating Markdown as the source of truth allows standards organizations to:

- Avoid format-driven content divergence  
- Maintain long-term consistency across releases  
- Support future formats without restructuring documents  
- Build trust with implementers and reviewers  

This model scales with both organizational maturity and specification longevity.

---

## Summary

Preparing reliable HTML and PDF outputs starts with disciplined source authoring.

By treating Markdown as the authoritative source and prioritizing structural fidelity over format-specific behavior, standards organizations can publish specifications that remain consistent, reviewable, and dependable across formats.

PubHub supports this approach by rendering content predictably—without introducing editorial decisions or format-driven content changes.
