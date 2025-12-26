---
title: Publishing Structure — How Specifications Are Assembled
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

Technical specifications are rarely written as a single document.

In standards organizations, specifications are usually developed over time, across multiple files, by different contributors, and reviewed in stages. Publishing those specifications reliably requires more than rendering text—it requires **clear structure**.

This guidance explains how document structure is understood when publishing specifications using PubHub (formerly MD2HTML). It is an orientation page intended to help you **think correctly about structure** before applying specific rules or constructors.

---

## What “Publishing Structure” Means

Publishing structure describes **how a specification is assembled and understood as a complete document**, independent of how it is authored.

In practice, this includes:

- How individual files are combined into a single specification  
- How sections are ordered and identified  
- How metadata (title, version, status) is applied  
- How references, terminology, and legal material are included  
- How readers navigate the final HTML or PDF output  

Structure is not about formatting.  
It is about **predictability, clarity, and long-term consistency**.

---

## Why Structure Matters in Standards Work

In consensus-based standards development:

- Documents are reviewed repeatedly over long periods  
- References must remain stable across versions  
- Terminology must be used consistently  
- Legal and licensing material must be unambiguous  
- Published outputs must be reproducible and auditable  

Without clear structure, even well-written content can become difficult to review, publish, or maintain.

PubHub supports publishing by **making structure explicit**, not by enforcing a particular writing style.

---

## How PubHub Approaches Structure

PubHub treats a specification as an **assembled artifact** rather than a single file.

At a high level:

1. Content is authored in multiple Markdown files  
2. A designated entry file defines how those files are assembled  
3. Metadata and ordering are applied consistently  
4. The complete document is rendered as HTML and PDF  

This approach allows organizations to:

- Keep content modular during development  
- Publish complete, coherent documents  
- Reproduce outputs from specific versions of content  

PubHub does not change how contributors write. It supports how content is assembled and published.

---

## Conceptual Elements of Document Structure

When preparing a specification for publishing, structure typically includes the following conceptual elements:

- **Front matter** — document identity and metadata  
- **Introduction and scope** — purpose and boundaries  
- **Normative and informative content** — clearly distinguished  
- **References** — structured and stable  
- **Terminology and abbreviations** — defined once, reused consistently  
- **Legal and licensing material** — explicitly included  
- **Indexes and navigation aids** — generated automatically  

Each of these elements has specific guidance, but they should first be understood as **parts of a whole**.

---

## What This Page Does *Not* Do

This page does not:

- Describe specific Markdown or HTML constructors  
- Provide syntax examples  
- Define file formats or configuration properties  
- Explain version-specific behavior  

Those details are covered in **dedicated, focused guidelines**.

This page exists to establish the **mental model** that makes those details easier to apply correctly.

---

## When to Read This Guidance

This orientation is most useful when:

- You are starting to develop a specification for the first time  
- You are transitioning from informal drafts to formal releases  
- You are introducing new editors or contributors  
- You are reviewing or refactoring an existing document set  

It is less useful once you are already applying specific publishing rules.

---

## Where to Go Next

Once you understand how publishing structure works conceptually, continue with the guidance most relevant to your task:

- **Defining document assembly using an index file**  
- **Structuring front matter and document metadata**  
- **Managing references (normative and informative)**  
- **Defining terminology and abbreviations**  
- **Handling legal disclaimers and licenses**  

Each topic is covered in its own guideline and can be applied independently.

---

## Summary

Publishing structure is what turns a collection of files into a coherent technical specification.

PubHub supports publishing outputs; governance and editorial decisions remain with the organization. It does this by making document assembly explicit and repeatable.

Understanding structure first makes every other publishing guideline easier to apply—and helps ensure that published specifications remain clear, stable, and consumable over time.