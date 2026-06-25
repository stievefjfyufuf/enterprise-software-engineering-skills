# 11 Code Review Skill Docs

## When To Use

Gunakan saat diff, PR, code change, migration, atau test perlu direview untuk bug, risiko, regresi, dan missing coverage.

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
# Code Review

## Findings

| Severity | File/Line | Finding | Impact | Suggested Fix |
|---|---|---|---|---|

## Missing Tests

## Regression Risks

## Security/Data Risks

## Decision

Approve / Request Changes / Block

## Notes
```

## Quality Checklist

- Findings disusun berdasarkan severity.
- Temuan punya file/line jika tersedia.
- Review fokus pada bug, regression, security, data loss, dan missing tests.
- Keputusan review jelas.

## Handoff

Jika approve, lanjut ke 12-se-test-planning. Jika request changes/block, kembali ke 10-se-implementation.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.