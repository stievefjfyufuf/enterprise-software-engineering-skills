# 12 Test Planning Skill Docs

## When To Use

Gunakan saat test strategy, scenario, coverage matrix, test data, dan regression checklist perlu dibuat.

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
# Test Plan

## Scope

## Coverage Matrix

| Requirement/AC | Test Type | Scenario | Priority | Automated? |
|---|---|---|---|---|

## Test Data

## Regression Checklist

## Manual Verification Needed

## Risks
```

## Quality Checklist

- Acceptance criteria dipetakan ke skenario test.
- Unit/integration/e2e/manual dibedakan.
- Test data dan edge case dicatat.
- Regression checklist tersedia.

## Handoff

Bawa test plan ke 13-se-automated-testing.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.