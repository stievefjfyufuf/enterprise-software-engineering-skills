# 11 Code Review Skill Docs

## When To Use

Gunakan saat diff, PR, code change, migration, atau test perlu direview untuk bug, risiko, regresi, dan missing coverage.

## Required Inputs

- Code diff or changed files.
- Selected issue, acceptance criteria, implementation notes, tests, and architecture/design constraints.
- Risk notes for data, security, migration, performance, or compatibility.

## Step Procedure

1. Review the diff against the issue scope and acceptance criteria first.
2. Prioritize behavioral regressions, security flaws, data loss, migration risk, missing tests, and maintainability problems.
3. Reference file/line when available and assign severity such as `P0`, `P1`, `P2`, or `P3`.
4. Check whether implementation changed unrelated baseline behavior.
5. Identify missing tests and residual risk even when approving.
6. Decide: approve, approve with notes, request changes, or block.
7. If approved, send to `12-se-test-planning`; if blocked, route back to `10-se-implementation`.

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

## Traceability IDs

- Keep `ISSUE`, `REQ`, `AC`, and `CR` references in review notes.
- Use `FINDING-###` for actionable review findings.

## Mini Example

```markdown
## Findings
- FINDING-001 [P1] src/api/equipment.ts:42 allows non-admin users to query overdue equipment.

## Decision
Request changes; security issue blocks testing.
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
