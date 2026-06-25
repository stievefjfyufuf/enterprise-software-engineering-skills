# 16 Change Log dan Engineering Loop Skill Docs

## When To Use

Gunakan saat PRD, design, code, test, atau app sudah punya baseline lalu user meminta perubahan, bug fix, tambahan fitur, refactor, atau koreksi release.

## Required Inputs

- User change request, defect report, stakeholder feedback, or production issue.
- Current baseline artifacts: PRD/spec, design, code, tests, release/deployment notes.
- Known affected IDs such as `REL`, `REQ`, `ISSUE`, `TEST`, or `UAT`.

## Step Procedure

1. Assign `CR-###` and capture requester, request, reason, type, urgency, and baseline affected.
2. Compare before/after behavior against the current baseline before proposing edits.
3. Perform impact analysis across requirements, design, database/API, UI, issues, code, tests, acceptance, deployment, docs, and operations.
4. Define approved scope and explicit not-in-scope items.
5. Decide routing: specification/design issue, implementation-only bug fix, testing-only gap, deployment correction, or full loop.
6. Define verification needed and rollback/compatibility concerns.
7. Route only to affected skills, then update baseline after review/test/acceptance/deployment succeeds.

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

## Traceability IDs

- Use `CR-###` for every baseline-affecting change request.
- Link `CR` to affected `REL`, `REQ`, `AC`, `ISSUE`, `TEST`, `UAT`, `API`, `UI`, or `DATA` IDs.

## Mini Example

```markdown
## Change ID
CR-001

## Request
Add role-based approval before equipment can be borrowed.

## Routing Decision
Send to skill(s): 03-se-specification, 07-se-database-api-design, 08-se-ui-design, 09-se-issue-planning.
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
