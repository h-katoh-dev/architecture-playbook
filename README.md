# Architecture Playbook

A public, practical knowledge base for learning and improving system architecture decision-making.

## Purpose

This repository focuses on **why an architecture should be chosen**, not simply which technology to use.

The goal is to develop the ability to:

- identify system responsibilities and boundaries
- generate multiple architecture options
- compare trade-offs
- reason about security, reliability, scalability, maintainability, and operations
- explain architectural decisions clearly
- review an existing architecture and identify risks

## Learning Loop

```text
Requirement
    ↓
Responsibilities & boundaries
    ↓
Architecture options
    ↓
Trade-off analysis
    ↓
Decision
    ↓
Review / feedback
    ↓
Architecture Decision Record (ADR)
```

## Repository Structure

- `principles/` — fundamental architecture principles
- `patterns/` — architecture patterns and when to use them
- `exercises/` — architecture design exercises
- `case-studies/` — realistic system design case studies
- `architecture-reviews/` — review checklists and review exercises
- `adr/` — documented architecture decisions and trade-offs

## Public Repository Policy

This repository is intentionally public.

Do not commit:

- confidential or proprietary information
- customer or employer-specific information
- personal information
- credentials, secrets, tokens, or private URLs
- unreleased project details

Real-world experiences may be generalized and anonymized so that the underlying architectural lessons remain useful without exposing confidential information.

## Relationship to dev-standard

`architecture-playbook` focuses on **architecture decisions and their reasoning**.

`dev-standard` focuses on **implementation standards and development rules**.

The two repositories may reference each other, but they serve different purposes.
