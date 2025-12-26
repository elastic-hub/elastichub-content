---
title: Getting Started with PubHub (formerly MD2HTML)
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

Publishing technical specifications is often one of the most fragile parts of standards work.

Specifications are typically authored collaboratively in Markdown, reviewed over time, and stored in Git repositories. When it comes time to publish, teams are expected to produce consistent, reviewable outputs—usually HTML and PDF—while preserving references, structure, and version integrity.

PubHub (formerly known as **MD2HTML**) exists to support this publishing step. It does not change how specifications are authored or governed. Instead, it provides a reliable way to assemble Markdown content from GitHub repositories into publishable formats that standards organizations can depend on. PubHub supports publishing outputs; governance and editorial decisions remain with the organization.

---

## What This Guidance Helps With

This page helps you understand:

- What PubHub is intended to support  
- When PubHub is useful in a standards workflow  
- When PubHub is *not* required  
- What assumptions PubHub makes about how you work  
- Where to find detailed guidance on Markdown structure and publishing rules  

It is an orientation page, not a usage reference.

---

## When PubHub Is Relevant

PubHub is typically useful when:

- Specifications are authored in Markdown and stored in GitHub repositories  
- You need to publish consistent HTML and PDF outputs from versioned content  
- Reviews require stable anchors and references  
- Releases must be reproducible from specific commits  
- Publishing should align with existing governance and contribution workflows  

PubHub can be introduced at any time of the specifications lifecycle, most often introduced once a group has stabilized its document structure and is preparing candidate or approved releases, but it also can be introduced at the early stages of development to help the Editors and the group to validate its content in PDF or HTML.

---

## When PubHub Is Not Required

PubHub may not be necessary when:

- Content is still exploratory or informal  
- Documents are not intended for external consumption  
- Publishing is handled manually and infrequently  
- The group is not yet ready to standardize document structure  

Using PubHub too early can add unnecessary formality. It is intended to support publishing maturity, not drive it.

---

## How PubHub Fits into Standards Work

PubHub works with content as it exists in GitHub repositories.

A typical flow looks like this:

1. Markdown files are authored and reviewed through pull requests  
2. A designated entry file defines how content is assembled  
3. PubHub generates HTML and PDF outputs from a specific commit  
4. Published artifacts can be reviewed, shared, or archived  

This approach supports transparency and traceability without requiring authors to change how they write or collaborate.

---

## What PubHub Assumes

PubHub assumes that:

- GitHub is the source of truth for content  
- Markdown or HTML structures are used consistently across the specification  
- Structure matters (headings, sections, references)  
- Publishing is part of a governed release process  

PubHub does **not** assume:

- A specific editorial style  
- A particular governance model  
- Public exposure of all content  
- Use of AI or automation beyond publishing  

Those decisions remain with the organization.

---

## Where to Go Next

This page does not explain *how* to structure Markdown or configure publishing.

For practical guidance, continue with:

- **Structuring Markdown for technical specifications**  
- **Defining document assembly using an index file**  
- **Managing stable anchors and references**  
- **Preparing HTML and PDF outputs for review and release**  

These topics are covered in dedicated guidelines within the PubHub section.

---

## About the Name Change

You may encounter references to **MD2HTML** in older documentation or discussions.

MD2HTML was the original name of the publishing tool. It has since been renamed **PubHub** to better reflect its role as publishing support within standards workflows. Functionally, it serves the same purpose.

---

## Summary

PubHub helps standards organizations publish specifications with confidence by turning versioned Markdown content into reliable HTML and PDF outputs.

It is not a CMS, an authoring tool, or a governance system. It is a publishing support mechanism that fits into how standards groups already work.

Use it when publishing needs to be repeatable, reviewable, and dependable—and not before.