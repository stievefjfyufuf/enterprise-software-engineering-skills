# 13 Automated Testing Skill Docs

## When To Use

Gunakan saat unit test, integration test, regression test, atau test run perlu ditambahkan/diperbarui.

## Required Inputs

- Test plan with `TEST` IDs and mapped acceptance criteria.
- Implementation diff and current repo test framework.
- Fixtures, mocks, environment requirements, and CI constraints.

## Step Procedure

1. Inspect existing test framework, naming conventions, fixtures, and CI commands.
2. Implement the highest-risk planned tests first, matching the repo's style.
3. Prefer deterministic fixtures and local mocks over external dependencies unless integration behavior is the target.
4. Cover success path, important negative path, permissions, validation, and regression checks.
5. Run focused tests first, then broader relevant suites when feasible.
6. Record commands, pass/fail output, failures fixed, skipped tests, and remaining coverage gaps.
7. If tests pass, send results to `14-se-acceptance-testing`; if tests expose a bug, route back to `10-se-implementation`.

## Output Template

```markdown
# Automated Testing Notes

## Tests Added/Updated

| Test File | Scenario | Requirement/AC |
|---|---|---|

## Test Data/Fixtures

## Commands Run

## Results

## Failures and Fixes

## Coverage Notes
```

## Traceability IDs

- Keep `TEST-###` IDs from the test plan.
- Link test files or test cases to `ISSUE`, `REQ`, and `AC`.

## Mini Example

```markdown
## Tests Added/Updated
| Test ID | File | Purpose |
|---|---|---|
| TEST-001 | tests/equipment-overdue.test.ts | Verifies admin overdue equipment list |

## Commands Run
- npm test -- equipment-overdue

## Results
Pass: 6 tests.
```

## Quality Checklist

- Test mengikuti framework dan pattern repo.
- Test menutup acceptance criteria berisiko.
- Fixture stabil dan tidak bergantung eksternal bila tidak perlu.
- Hasil command test dicatat.

## Handoff

Jika test lolos, lanjut ke 14-se-acceptance-testing. Jika gagal karena bug, kembali ke 10-se-implementation.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.
