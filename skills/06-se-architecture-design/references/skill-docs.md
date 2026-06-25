# 06 Architecture Design Skill Docs

## When To Use

Gunakan saat struktur aplikasi, component boundary, integration, deployment shape, dan keputusan arsitektur perlu dibuat.

## Required Inputs

- Validated requirements and NFRs.
- Expected scale, security/compliance constraints, integration needs, and deployment target.
- Existing repo/platform constraints if the project already has code.

## Step Procedure

1. Choose the simplest architecture style that satisfies requirements and NFRs; justify microservices only when the tradeoff is necessary.
2. Define components, responsibilities, ownership, boundaries, and communication patterns.
3. Map critical flows from user action to data storage and external integrations.
4. Record architecture decisions as `ADR-###` with context, decision, options considered, consequences, and rollback/migration impact.
5. Identify security, data integrity, observability, scalability, maintainability, and deployment risks.
6. Link each major component or decision to driving `REQ` or `NFR`.
7. Send component map and data flow to `07-se-database-api-design`.

## Output Template

```markdown
# Architecture Design

## Architecture Style

## Components

| Component | Responsibility | Depends On | Owner/Boundary |
|---|---|---|---|

## Data Flow

## External Integrations

## Architecture Decision Records

### ADR-001: [Decision]

Context:
Decision:
Consequences:
Tradeoffs:

## Risks
```

## Traceability IDs

- Use `ADR-###` for architecture decisions.
- Use `COMP-###` for components when the system has more than a few modules.
- Link every `ADR` to relevant `REQ` or `NFR`.

## Mini Example

```markdown
### ADR-001: Use modular monolith for MVP
Context: REQ-001 to REQ-006 need shared data and small-team delivery.
Decision: Build one deployable app with separated inventory, request, and admin modules.
Consequences: Lower deployment complexity now; revisit service split after clear scaling pressure.
```

## Quality Checklist

- Arsitektur traceable ke requirement dan NFR.
- Component punya responsibility jelas.
- Tradeoff dicatat.
- Security, scalability, maintainability, dan deployment dipertimbangkan.

## Handoff

Bawa component map dan data flow ke 07-se-database-api-design.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.
