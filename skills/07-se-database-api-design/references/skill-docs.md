# 07 Database dan API Design Skill Docs

## When To Use

Gunakan saat ERD, tabel, relasi, constraint, migration, endpoint, dan API contract perlu dibuat.

## Required Inputs

- Architecture component map and data flow.
- Validated requirements, user stories, NFRs, and acceptance criteria.
- Security, tenancy, data retention, audit, and integration constraints.

## Step Procedure

1. Derive entities from domain nouns and user workflows; avoid tables that exist only because an interface screen exists.
2. Define tables, primary keys, foreign keys, cardinality, uniqueness, indexes, audit fields, and retention needs.
3. Normalize for integrity, then denormalize only with a stated performance reason.
4. Design API endpoints from use cases, not just CRUD tables.
5. Specify auth/authorization, request schema, response schema, validation rules, error responses, pagination/filtering/sorting, and idempotency where relevant.
6. Record migration, seed data, backward compatibility, and rollback notes.
7. Send ERD/API contract to `08-se-ui-design` and `09-se-issue-planning`.

## Output Template

```markdown
# Database and API Design

## ERD Summary

## Tables

| Table | Purpose | Key Fields | Relationships |
|---|---|---|---|

## API Endpoints

| Method | Path | Purpose | Auth | Request | Response |
|---|---|---|---|---|---|

## Validation Rules

## Error Responses

## Migration Notes

## Security and Data Notes
```

## Traceability IDs

- Use `DATA-###` for tables/entities.
- Use `API-###` for API contract entries.
- Link each `DATA` and `API` item to `REQ`, `NFR`, or `AC`.

## Mini Example

```markdown
| Method | Path | Purpose | Auth | Request | Response |
|---|---|---|---|---|---|
| GET | /api/equipment/overdue | API-001: List overdue equipment for admins | Admin | query: page, status | items, borrower, dueDate |

## Error Responses
- 403 when user lacks admin role.
- 422 when pagination params are invalid.
```

## Quality Checklist

- Entity berasal dari domain dan requirement.
- Relasi dan cardinality jelas.
- Endpoint berbasis use case, bukan hanya CRUD tabel.
- Auth, validation, error, dan migration dicatat.

## Handoff

Bawa ERD/API contract ke 08-se-ui-design dan 09-se-issue-planning.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.
