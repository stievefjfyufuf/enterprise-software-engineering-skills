# 13 Automated Testing Skill Docs

## When To Use

Gunakan saat unit test, integration test, regression test, atau test run perlu ditambahkan/diperbarui.

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