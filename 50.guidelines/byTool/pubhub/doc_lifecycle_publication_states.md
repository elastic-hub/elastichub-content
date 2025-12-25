---
title: Managing Document Lifecycle and Publication States
category: Guidelines
audience_roles:
  - Editor
  - Program Manager
  - Chair
activities:
  - Publishing specifications
  - Managing releases
tool: PubHub
---

## Context

Technical specifications are not static artifacts. They evolve over time as requirements mature, feedback is incorporated, and implementations are validated.

To manage this evolution responsibly, standards organizations distinguish between **publication states** such as *Draft*, *Candidate*, *Approved*, and *Deprecated* (or *Historic*). These states communicate the current standing of a document to readers, implementers, and stakeholders.

This guidance explains how to think about **document lifecycle and publication states** when publishing specifications using PubHub, without defining governance rules or approval processes.

---

## What This Guidance Enables

Applying this guidance helps you to:

- Communicate the maturity and intent of a specification clearly  
- Maintain continuity across document versions  
- Avoid confusion between working drafts and stable releases  
- Support long-lived specifications, including deprecation and historical reference  
- Align document metadata with publication intent  

---

## What This Guidance Does *Not* Define

This guidance does **not** define:

- Specification lifecycle phases (e.g. scope, development, review, approval)  
- Voting, approval, or decision-making processes  
- Authority or responsibility for state transitions  
- Review or testing workflows  

Those topics belong in organizational process documentation and governance rules.

---

## Publication States vs Specification Lifecycle

It is important to distinguish between:

- **Specification lifecycle phases**  
  (how a specification is developed and approved), and

- **Publication states**  
  (how the resulting document is labeled and communicated once published).

This guidance focuses **only on publication states** — how a document is presented and understood by its audience after it is published.

---

## Common Publication States

Standards organizations commonly use the following publication states. These are **examples**, not mandates.

### Draft

A *Draft* specification:

- Is under active development  
- May change without notice  
- Is shared for review and feedback  

Drafts communicate intent but should not be relied on for stable implementations.

---

### Candidate

A *Candidate* specification is typically used **only when testing or validation is required**.

It indicates that:

- The document is considered technically complete  
- Feedback is focused on validation rather than design  
- Implementations may be developed to test interoperability or correctness  

Not all specifications require a Candidate state.

---

### Approved

An *Approved* specification:

- Has completed the organization’s approval process  
- Represents a stable and authoritative version  
- Is intended for implementation and long-term reference  

Approved documents should be clearly distinguishable from drafts and candidates.

---

### Deprecated / Historic

A *Deprecated* or *Historic* specification:

- Is no longer recommended for new implementations  
- May be superseded by a newer version  
- Is retained for reference, traceability, or historical reasons  

Deprecation does not imply deletion. Historical documents remain part of the organization’s published record.

---

## Relationship Between Lifecycle and Metadata

Publication states are typically expressed through **document metadata**, not through content changes alone.

Common metadata fields used to reflect lifecycle include:

- Publication status  
- Version identifier  
- Publication date  
- Watermarks or visual indicators  

By updating metadata intentionally, organizations can signal lifecycle changes without rewriting the document body.

---

## What Changes Between States (and What Should Not)

When a document moves between publication states:

- Metadata is often updated  
- Visual indicators (such as watermarks) may change  
- Release notes or changelogs may be updated  

What should **not** change unintentionally:

- Document identity  
- Scope and intent (unless explicitly revised)  
- Historical versions and references  

Clear separation between content evolution and state signaling improves trust and traceability.

---

## How PubHub Supports Document Lifecycle

PubHub does not manage or enforce lifecycle decisions. Instead, it:

- Renders publication metadata consistently in HTML and PDF outputs  
- Preserves historical versions as published artifacts  
- Supports clear visual signaling of document state  
- Enables reproducible publication from specific repository states  

Responsibility for lifecycle decisions remains with the standards organization.

---

## Recommended Practices (DOs)

- Use publication states consistently across documents  
- Reflect lifecycle state through metadata, not informal text  
- Preserve access to deprecated or historic specifications  
- Review publication state at each formal release  

---

## Common Pitfalls to Avoid (DON’Ts)

- Do not conflate development phases with publication states  
- Do not change document identity when updating status  
- Do not remove historical specifications without traceability  
- Do not rely on ambiguous language to signal document maturity  

These issues frequently lead to confusion for implementers and reviewers.

---

## Related Guidance

- Publishing Structure — How Specifications Are Assembled  
- Structuring Front Matter and Document Metadata  
- Defining Document Assembly Using `index.yaml`  
- Managing Legal Disclaimers and Licenses  

---

## Summary

Publication states communicate the maturity and intent of a technical specification.

By managing document lifecycle explicitly and signaling state through metadata, standards organizations provide clarity, stability, and long-term value to their communities.

PubHub supports this approach by rendering lifecycle information predictably—without defining governance rules or approval authority.