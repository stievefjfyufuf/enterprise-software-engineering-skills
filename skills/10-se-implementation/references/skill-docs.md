# 10 Implementation Skill Docs

## When To Use

Gunakan saat satu issue siap dikerjakan menjadi perubahan code yang scoped.

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
# Implementation Notes

## Issue

## Files Changed

| File | Reason |
|---|---|

## Approach

## Behavior Implemented

## Migration/Config Changes

## Manual Verification

## Risks
```

## Quality Checklist

- Repo dan pattern lokal dibaca dulu.
- Perubahan hanya sesuai issue atau approved scope.
- Behavior memenuhi acceptance criteria.
- Tidak mengubah baseline di luar scope.

## Handoff

Bawa diff dan implementation notes ke 11-se-code-review.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.