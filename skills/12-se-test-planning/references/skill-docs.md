# 12 Test Planning Skill Docs

## When To Use

Gunakan saat test strategy, scenario, coverage matrix, test data, dan regression checklist perlu dibuat.

## Required Inputs

- Requirements, acceptance criteria, selected issue, implementation notes, and review findings.
- Architecture/API/UI/data risk notes.
- Existing test pyramid, framework, fixtures, and CI constraints.

## Step Procedure

1. Map every acceptance criterion to at least one scenario.
2. Classify tests as unit, integration, API, UI/e2e, manual, regression, security, or migration checks.
3. Prioritize high-risk behavior, permissions, data boundaries, error handling, and rollback-sensitive paths.
4. Define test data, fixtures, setup/teardown, and external service handling.
5. Include negative cases, edge cases, and regression checks for nearby behavior.
6. Identify what cannot be automated yet and why.
7. Send test plan to `13-se-automated-testing`.

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

## Traceability IDs

- Use `TEST-###` for planned test scenarios.
- Map each `TEST` to `AC`, `REQ`, and `ISSUE`.

## Mini Example

```markdown
| Test ID | Acceptance Criteria | Type | Scenario | Data Needed |
|---|---|---|---|---|
| TEST-001 | AC-001 | Integration | Admin sees overdue equipment only | overdue item, active borrower |
| TEST-002 | AC-001 | Security | Non-admin cannot access overdue endpoint | non-admin user |
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
