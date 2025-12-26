---
title: Overview of Publishing Guidance
category: Guidelines
audience_roles:
  - Editor
  - Program Manager
activities:
  - Writing specifications
  - Publishing releases
tools:
  - PubHub
  - Website Rendering
layout: doc
---

## Context

Standards organizations often use Markdown and Git-based workflows to author technical specifications. While authoring and review are usually well understood, **publishing** introduces additional constraints: structure must be consistent, references must remain stable, and outputs must be suitable for long-term consumption by the industry.

This guidance explains the **publishing paths supported by Elastic Hub**, and how the related guidelines are organized. It does not prescribe a single approach. Instead, it helps you understand which publishing mechanism is appropriate for your context and where to find detailed guidance.

---

## What This Guidance Covers

This section of the guidelines helps you:

- Understand the publishing mechanisms supported by Elastic Hub
- Choose an appropriate rendering approach for your documents
- Write and structure content so it renders reliably as HTML, PDF , and ODF, OOXML
- Avoid common structural issues that affect published outputs

It is an orientation layer, not a technical reference.

---

## Publishing Paths Supported

Elastic Hub supports three primary ways of rendering standards content into HTML, PDF, ODF (OpenDocument Format (ISO/IEC standard)), and OOXML (Office Open XML, (ISO/IEC 29500)). Each serves a different purpose and maturity level.

---

## Publishing with PubHub (formerly MD2HTML)

PubHub is a publishing support tool designed for standards specifications stored in GitHub repositories.

It is typically used when:

- Specifications are versioned and released from Git
- Publishing needs to be reproducible from specific commits
- HTML, PDF, ODF, and OOXML outputs must remain consistent over time
- No rendering framework is installed in the content repository

With PubHub:

- Content is assembled from Markdown files based on a defined entry file
- Publishing is triggered from a repository, branch, and commit
- Outputs are generated without modifying the source repository
- Differences between published versions can be compared

PubHub supports publishing maturity without changing how authors write or review content.

Detailed guidance for PubHub—including document assembly and Markdown structuring—is available in the **PubHub-specific guidelines**.

---

## Publishing via Website Rendering (Nuxt-based)

Some organizations choose to render specifications directly as part of a website.

This approach is typically used when:

- Specifications are part of a broader public or member-facing site
- Content is rendered dynamically as HTML
- Publishing and presentation are tightly integrated
- The organization controls and maintains the website codebase

In this model:

- Rendering logic is installed alongside content in the repository
- Markdown is processed as part of the website build
- Published output is primarily HTML, with PDFs generated as needed

This approach requires more upfront setup but offers tighter integration with website presentation.

Guidelines for website-based rendering explain how content should be structured to ensure consistent display.

---

## Choosing the Right Approach

There is no single correct publishing path.

In practice:

- **PubHub** is often used for formal specification releases and archival publishing
- **Website rendering** is often used for living documents and ongoing visibility

Some organizations use both at different stages of their lifecycle.

Elastic Hub supports both approaches and helps organizations choose what fits their governance, maturity, and publishing needs.

---

## Important Note on Structure

Regardless of the publishing path, **document structure matters**.

If Markdown constructors, section hierarchy, or document assembly are inconsistent, published outputs may be incomplete or incorrectly rendered.

For this reason, detailed guidelines focus on *how to structure content*, not just how to render it.

---

## Where to Go Next

Depending on your needs, continue with:

- **Getting Started with PubHub (formerly MD2HTML)**
- **Structuring Markdown for technical specifications**
- **Defining document assembly and entry files**
- **Preparing content for HTML and PDF outputs**

Each topic is covered in a dedicated guideline.

---

## Summary

This guidance introduces the publishing approaches supported by Elastic Hub and explains how to navigate the related guidelines.

Publishing does not need to be complex or fragile. With appropriate structure and the right support mechanisms, standards organizations can publish specifications that are reliable, reviewable, and consumable—without changing how they work.