# ADR-001: Authentication responsibility for a CMS-centered member system

## Context

A content-oriented website needs member authentication and application data.
The system may include a CMS such as Drupal and a separate application layer.

The key question is where authentication responsibility should live.

## Options

### Option A: Build custom authentication in a separate application

The application owns login, session handling, password management, and member authentication.

### Option B: Use a managed authentication service from the existing CMS/application boundary

A managed authentication service handles authentication while the CMS remains focused on content and site responsibilities.

## Decision

Prefer **separating authentication responsibility from content management** when the system already has a suitable managed authentication boundary.

The exact service is not prescribed by this ADR. The decision depends on security requirements, existing platform capabilities, operational ownership, and integration constraints.

## Trade-offs

### Benefits

- Reduces custom security-sensitive implementation.
- Keeps content management and authentication responsibilities more clearly separated.
- Allows application features to evolve without making the CMS responsible for every authentication concern.

### Costs

- Introduces an external service dependency.
- Requires careful session, authorization, and account-linking design.
- Operational ownership becomes an important architectural concern.

## Consequences

The architecture should explicitly define:

- authentication responsibility
- authorization responsibility
- user/account identity mapping
- session/token boundaries
- failure and recovery behavior
- operational ownership

This decision is a learning example, not a universal recommendation. The correct choice depends on the system's requirements and constraints.
