---
title: Defining Document Assembly Using index.yaml
layout: doc
category: Guidelines
audience_roles:
  - Editor
  - Program Manager
activities:
  - Publishing releases
  - Preparing specifications
tool: PubHub
---

## Context

Technical specifications are typically authored as a collection of Markdown files rather than a single document. While this modular approach supports collaboration and review, publishing requires those files to be assembled into a **single, coherent artifact**.

In PubHub (formerly MD2HTML), document assembly is defined explicitly using an `index.yaml` file. This file describes **what the document is**, **how it should be identified**, and **which content files form the final specification**.

This guidance explains how to define document assembly using `index.yaml` so that published HTML, PDF and other output formats are predictable, reproducible, and aligned with governance expectations.

---

## What This Guidance Enables

Using `index.yaml` allows you to:

- Assemble multiple Markdown files into a single specification  
- Define document identity and publication metadata  
- Control the order in which content appears  
- Ensure releases are reproducible from specific repository states  
- Publish consistent HTML and PDF outputs  

This mechanism supports publishing maturity without changing how content is authored or reviewed.

---

## When This Guidance Is Relevant

This guidance applies when:

- You are preparing a specification for formal publication or your start the development of one a new specification and you want to get it right from the beginning.
- Content is stored in a Git repository and authored in Markdown  
- The document consists of multiple sections or appendices  
- Publishing must align with versioning and release governance  

It is most often applied during candidate or approved release preparation.

---

## When This Guidance Is Not Required

This guidance may not be necessary when:

- Content is exploratory or informal  
- Documents are not intended for external publication  
- Publishing is handled manually and infrequently  

Introducing document assembly too early can add unnecessary structure.

---

## Purpose of the `index.yaml` File

The `index.yaml` file serves as the **entry point for document assembly**.

It defines:

- Document metadata (title, version, status, organization)  
- Output identification (document name, watermark)  
- The ordered list of content files that form the document  

PubHub uses this file to assemble content from the repository into a complete specification.

Each technical document must include one `index.yaml` file located at the root of the document folder.

---

## Example `index.yaml` File

```yaml
---
title: "Lightweight Machine to Machine Technical Specification: Core"
status: "Approved"
version: "1.2"
organizationName: "Open Mobile Alliance (OMA)"
date: "2020-11-10"
copyrightDate: "2023"
logo: "images/oma_logo.png"
documentName: "OMA-TS-LightweightM2M_Core-V1_2-20201110-A"
watermark: "APPROVED"
files:
  - License.md
  - OMA-TS-LightweightM2M_Core.md
  - Appendix_A.md
  - Appendix_B.md
  - Appendix_C.md
  - Appendix_D.md
  - Appendix_E.md
  - Appendix_F.md
  - Appendix_G.md
  - Appendix_H.md
  - Appendix_I.md
  - Appendix_J.md
  - Appendix_K.md
  - Appendix_L.md
  - Appendix_M.md
---
```

## Metadata Properties

The following properties are commonly used in `index.yaml`:

| Property           | Purpose |
|--------------------|---------|
| `title`            | Human-readable document title displayed on the front page |
| `status`           | Publication status (e.g. Draft, Candidate, Approved) |
| `version`          | Document version identifier |
| `organizationName` | Full name of the publishing organization |
| `date`             | Publication date in `YYYY-MM-DD` format |
| `copyrightDate`    | Copyright year |
| `logo`             | Optional path to a logo displayed on the front page |
| `documentName`     | Base filename used for generated outputs |
| `watermark`        | Watermark applied to the PDF output |
| `files`            | Ordered list of Markdown files forming the document |

The `files` list determines the **exact order** in which content appears in the published document.

---

## Managing Content Order

Content files are assembled in the sequence listed under the `files` property.

### Guidance

- Include the main specification content before appendices  
- List appendices in logical order  
- Ensure all referenced files exist in the repository  
- Avoid reordering files between releases unless intentional  

Explicit ordering reduces ambiguity during review and publication.

---

## Handling Legal and License Content

Legal and licensing content must be included **explicitly** in the document assembly.

Please refer to [Managing Legal Disclaimers and Licenses](managing_legal_disclaimers_and_licenses.md) for detailed guidance.    


---

## Common Pitfalls

Avoid the following issues:

- Omitting required content files from the `files` list  
- Relying on implicit ordering instead of explicit sequencing  
- Mixing document metadata with content text  
- Changing document identity fields between releases without intent  

Clear assembly definitions reduce publishing errors and review friction.

---

## Related Guidance

- Publishing Structure — How Specifications Are Assembled  
- Structuring Front Matter and Document Metadata  
- Managing Legal Disclaimers and Licenses  
- Preparing HTML and PDF Outputs  

---

## Summary

The `index.yaml` file defines how a technical specification is assembled and identified at publication time.

PubHub supports publishing outputs; governance and editorial decisions remain with the organization. The `index.yaml` file makes assembly explicit and reproducible from version-controlled sources.

Use this mechanism when publishing needs to be dependable, auditable, and aligned with formal release processes.