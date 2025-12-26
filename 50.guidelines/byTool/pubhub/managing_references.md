---
title: Managing Normative and Informative References
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

References are a critical part of technical specifications.

In standards work, references establish the external documents that define requirements, terminology, or background context. They must be clear, stable, and unambiguous so that readers can understand what is required to implement a specification and what material is provided for additional context.

This guidance explains how to manage **Normative** and **Informative** references when publishing specifications using PubHub (formerly MD2HTML), ensuring that references render correctly and remain reliable across HTML and PDF outputs.

---

## What This Guidance Enables

Applying this guidance helps you to:

- Clearly distinguish mandatory and non-mandatory references  
- Ensure references are rendered consistently in HTML and PDF  
- Avoid broken links or ambiguous citations  
- Support long-term stability of published specifications  
- Align reference handling with common standards practices  

---

## When This Guidance Is Relevant

This guidance applies when:

- You are preparing a technical specification for publication or you start developing the specifications and want to get it right from the beginning. 
- The document includes external standards, specifications, or references  
- References must be reviewed, approved, and maintained over time  
- HTML and PDF outputs must be consistent and reliable  

It is especially important during candidate and approved release stages.

---

## When This Guidance Is Not Required

This guidance may not be necessary when:

- Content is informal or exploratory  
- External references are not yet agreed  
- The document is not intended for formal publication  

However, introducing reference structure early can reduce rework later.

---

## Normative vs Informative References

### Normative References

Normative references define **mandatory dependencies**.

They are documents that:
- Contain requirements used by the specification
- Must be implemented or complied with to conform

If a reference is normative, it must be available and applicable for correct implementation.

---

### Informative References

Informative references provide **additional context**.

They may:
- Explain background concepts
- Offer examples or guidance
- Provide historical or explanatory material

Informative references are not required to implement the specification.

---

## Structuring the References Section

A specification must include **two separate subsections**:

- **Normative References**
- **Informative References**

Each subsection should contain a reference list structured explicitly so that it renders correctly in published outputs.

---

## Defining References Using HTML Structures

To ensure reliable rendering, references are defined using HTML definition list elements.

### Example Reference Structure

```html
<dl>
  <dt>[OMADICT]</dt>
  <dd>
    "Dictionary for OMA Specifications",
    Open Mobile Alliance™,
    OMA-ORG-Dictionary-V2_9,
    URL: http://www.openmobilealliance.org/
  </dd>
</dl>
```

This structure ensures:

- Clear separation of reference identifiers and descriptions  
- Consistent layout in HTML and PDF outputs  
- Predictable rendering across publishing formats  

---

## Recommended Practices (DOs)

- Use `dl`, `dt`, and `dd` HTML elements for reference lists  
- Use square brackets for reference identifiers (e.g. `[ABC]`)  
- Include complete citation details:
  - Title  
  - Author or organization  
  - Version or identifier  
  - Publication date (if applicable)  
  - URL  
- Separate Normative and Informative references into distinct sections  

---

## Common Mistakes to Avoid (DON’Ts)

- Do not use Markdown lists or tables for references  
- Do not mix Normative and Informative references in one list  
- Do not use inline Markdown links as the primary reference definition  
- Do not omit reference identifiers or rely on implicit citations  

These issues frequently lead to broken layouts or ambiguous references in published documents.

---

## How PubHub Supports Reference Handling

PubHub supports publishing outputs; governance and editorial decisions remain with the organization. It does this by:

- Preserves the explicit structure defined in the source content  
- Renders references consistently in HTML and PDF outputs  
- Ensures reference tables remain stable across versions  

This preserves stable rendering across published versions.

---

## Related Guidance

- Publishing Structure — How Specifications Are Assembled  
- Defining Document Assembly Using `index.yaml`  
- Terminology, Definitions, and Abbreviations  
- Preparing HTML and PDF Outputs  

---

## Summary

Normative and Informative references play a central role in the clarity and integrity of technical specifications.

By defining references explicitly and structuring them consistently, standards organizations can ensure that published documents remain clear, reviewable, and dependable over time.

PubHub supports this process by rendering references reliably—without imposing editorial or governance decisions on the content.