# 06 Architecture Design Skill Docs

## When To Use

Gunakan saat struktur aplikasi, component boundary, integration, deployment shape, dan keputusan arsitektur perlu dibuat.

## Required Inputs

Read the parent SKILL.md first, then confirm the available inputs match the skill purpose. If an input is missing, infer conservatively from project context or list it as an open question.

## Step Procedure

1. Review the current project artifact from the previous step.
2. Identify the smallest useful output this step must produce.
3. Preserve traceability to stakeholder goals, requirements, issues, tests, or change requests.
4. Call out enterprise concerns when relevant: risk, ownership, dependency, security, compliance, data integrity, observability, migration, rollback, and maintainability.
5. Prepare a handoff artifact for the next numbered skill.

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