# 08 UI Design Skill Docs

## When To Use

Gunakan saat halaman, navigasi, form, state UI, wireframe, dan user flow perlu dirancang.

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
# UI Design

## Screen List

| Screen | User Goal | Main Actions | Data Needed |
|---|---|---|---|

## Navigation Flow

## Forms

| Form | Field | Type | Validation | Error Message |
|---|---|---|---|---|

## UI States

- Loading:
- Empty:
- Error:
- Success:

## Wireframe Notes
```

## Quality Checklist

- Setiap screen punya user goal.
- Navigasi mendukung alur utama.
- Form field dan validasi jelas.
- Loading, empty, error, dan success state dicatat.

## Handoff

Bawa screen specs dan UI flow ke 09-se-issue-planning.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.