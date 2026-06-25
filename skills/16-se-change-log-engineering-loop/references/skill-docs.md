# 16 Change Log dan Engineering Loop Skill Docs

## When To Use

Gunakan saat PRD, design, code, test, atau app sudah punya baseline lalu user meminta perubahan, bug fix, tambahan fitur, refactor, atau koreksi release.

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
# Change Request

## Change ID

CR-000

## Request

## Reason

## Type

Feature addition / Behavior change / Bug fix / Removal / Refactor / Breaking change

## Impact Analysis

| Artifact | Affected? | Change Needed | Risk |
|---|---|---|---|

## Approved Scope

## Not In Scope

## Before

## After

## Verification Needed

## Routing Decision

Send to skill(s):
```

## Quality Checklist

- Perubahan masuk sebagai Change Request.
- Baseline dibandingkan sebelum edit.
- Affected dan unaffected artifacts jelas.
- Approved scope membatasi perubahan.
- Before/After dan verification needed dicatat.

## Handoff

Route hanya ke skill terdampak, lalu setelah lolos review/test/acceptance update baseline.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.