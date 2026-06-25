# 09 Issue Planning Skill Docs

## When To Use

Gunakan saat requirement dan design perlu diubah menjadi issue/task developer-ready.

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