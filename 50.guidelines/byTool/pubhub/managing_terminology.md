---
title: Managing Terminology, Definitions, and Abbreviations
category: Guidelines
audience_roles:
  - Editor
  - Program Manager
activities:
  - Writing specifications
  - Publishing releases
tool: PubHub
layout: doc
---

## Context

Clear and consistent terminology is essential in technical specifications.

Standards documents often introduce terms and abbreviations that are reused throughout the text. If these terms are not defined explicitly and used consistently, readers may misinterpret requirements, reviewers may raise repeated clarification questions, and implementations may diverge.

This guidance explains how to define and manage **terminology, definitions, and abbreviations** in specifications published using PubHub (formerly MD2HTML), ensuring clarity and consistent rendering in HTML and PDF outputs.

---

## What This Guidance Enables

Applying this guidance helps you to:

- Define technical terms unambiguously  
- Ensure consistent usage of terms across the document  
- Provide clear expansions for abbreviations  
- Improve readability for both new and experienced readers  
- Render terminology consistently in published HTML and PDF outputs  

---

## When This Guidance Is Relevant

This guidance applies when:

- A specification introduces new technical terms  
- Abbreviations are used throughout the document  
- Definitions need to be referenced consistently in multiple sections  
- The document is prepared for formal review or publication  

It is especially important for normative specifications and long-lived standards.

---

## When This Guidance Is Not Required

This guidance may not be necessary when:

- Content is informal or exploratory  
- Terminology is well known and already defined elsewhere  
- The document is not intended for external publication  

However, introducing terminology structure early often reduces later rework.

---

## Structuring the Terminology Section

Specifications should include a dedicated section titled:

**Terminology and Conventions**

This section typically contains two subsections:

- **Definitions**  
- **Abbreviations**

Keeping definitions and abbreviations separate improves readability and reduces ambiguity.

---

## Defining Terms Using Definition Lists

Definitions are defined using HTML definition list elements to ensure consistent rendering.

### Example Definition Structure

```html
<dl>
  <dt>Git</dt>
  <dd>
    Git is a distributed version control system that tracks changes
    in any set of text files.
  </dd>
  <dt>Firewall</dt>
  <dd>
    A network security system that monitors and controls incoming
    and outgoing network traffic based on predetermined security rules.
  </dd>
</dl>
```

This structure ensures:

- Clear separation between terms and descriptions
- Consistent layout in HTML and PDF outputs
- Predictable rendering across publishing formats

---

## Using Defined Terms in Document Text

Defined terms can be referenced directly within the document text.

### Singular Usage

To reference a defined term in singular form, insert the term inside an anchor element:

```html
<a>firewall</a>
```

### Plural Usage

To reference a defined term in plural form, use the title attribute to specify the singular term:

```html
<a title="firewall">firewalls</a>
```

When readers hover over the term, a tooltip displays the definition. Clicking the term navigates to the definition entry.

## Defining Abbreviations

Abbreviations are defined using the same definition list structure.

### Example Abbreviation Structure
```html
<dl data-caption="Abbreviations"
    data-term-column-title="Term"
    data-description-column-title="Description">
  <dt>TS</dt>
  <dd>Technical Specification</dd>
  <dt>AD</dt>
  <dd>Architecture Document</dd>
</dl>
```

Using a consistent structure for abbreviations ensures uniform presentation across outputs.

## Using Abbreviations in Document Text
### Singular Usage

To reference an abbreviation in singular form:

```html
<abbr>TS</abbr>
```

### Plural Usage

To reference an abbreviation in plural form, specify the singular form in the title attribute:

```html
<abbr title="TS">TSs</abbr>
```

Hovering over the abbreviation displays its expanded form.

## Recommended Practices (DOs)

- Include a dedicated Terminology and Conventions section

- Separate Definitions and Abbreviations into distinct subsections

- Use dl, dt, and dd HTML elements for structured lists

- Reference defined terms consistently throughout the document

- Introduce definitions before first use when possible

## Common Mistakes to Avoid (DON’Ts)

- Do not mix definitions and abbreviations in a single list

- Do not redefine the same term in multiple places

- Do not rely on informal explanations embedded in text

- Do not introduce abbreviations without defining them first

These issues often lead to confusion, inconsistent interpretation, and review delays.

### How PubHub Supports Terminology Handling

PubHub supports publishing outputs; governance and editorial decisions remain with the organization. It does this by:

- Preserves explicit definition structures in source content
- Renders definitions and abbreviations consistently in HTML and PDF
- Enables navigation and tooltips for defined terms
- Maintains stability across published versions


### Related Guidance

- Publishing Structure — How Specifications Are Assembled

- Managing Normative and Informative References

- Defining Document Assembly Using index.yaml

- Preparing HTML and PDF Outputs

## Summary

Terminology, definitions, and abbreviations are foundational to the clarity and consistency of technical specifications.

By defining terms explicitly and using them consistently, standards organizations reduce ambiguity, improve review efficiency, and support reliable implementation.

PubHub supports this process by rendering terminology structures predictably—without imposing editorial or governance decisions on the content.