# 09 Issue Planning Skill Docs

## When To Use

Gunakan saat requirement dan design perlu diubah menjadi issue/task developer-ready.

## Required Inputs

- Validated requirements and priority order.
- Architecture, ERD, API contract, UI specs, and acceptance criteria.
- Known dependencies, release target, team constraints, and risk notes.

## Step Procedure

1. Create one issue per reviewable outcome, not one issue per vague feature area.
2. Assign `ISSUE-###` IDs and link each issue to `REQ`, `AC`, `API`, `UI`, `DATA`, or `ADR` IDs.
3. Define scope, out-of-scope, acceptance checklist, implementation notes, test expectations, and dependencies.
4. Split work when an issue mixes migration, backend, UI, and testing in a way that cannot be reviewed cleanly.
5. Mark labels, milestone/sprint, owner role, risk, and blocked-by relationships.
6. Sequence issues so enabling schema/API work happens before dependent UI work.
7. Send one selected issue to `10-se-implementation`.

## Output Template

```markdown
# Issue Plan

## Issue Title

## Context

## Scope

## Acceptance Criteria

- [ ]

## Technical Notes

## Dependencies

## Out of Scope

## Test Notes

## Traceability

Requirement ID:
Change Request ID:
```

## Traceability IDs

- Use `ISSUE-###` for implementation tasks.
- Every issue should reference at least one `REQ` and one `AC`.
- Use `DEP-###` for important cross-issue dependencies when needed.

## Mini Example

```markdown
## Issue Title
ISSUE-001: Show overdue equipment dashboard for lab admins

## Acceptance Criteria
- [ ] AC-001 passes for overdue equipment visibility.
- [ ] API-001 errors are handled in the UI.

## Dependencies
- API-001 must exist before UI-001 is implemented.
```

## Quality Checklist

- Satu issue punya satu outcome yang bisa direview.
- Scope dan out-of-scope jelas.
- Acceptance criteria bisa dicek.
- Dependency dan traceability dicatat.

## Handoff

Bawa selected issue ke 10-se-implementation.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.
