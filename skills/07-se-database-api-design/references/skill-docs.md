# 07 Database dan API Design Skill Docs

## When To Use

Gunakan saat ERD, tabel, relasi, constraint, migration, endpoint, dan API contract perlu dibuat.

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