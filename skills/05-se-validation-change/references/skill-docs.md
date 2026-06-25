# 05 Validation dan Change Skill Docs

## When To Use

Gunakan saat requirement perlu diperiksa kelengkapan, konsistensi, testability, atau saat ada perubahan requirement awal.

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
# Requirement Validation

| Requirement ID | Clear | Complete | Consistent | Feasible | Testable | Traceable | Notes |
|---|---|---|---|---|---|---|---|

## Issues Found

## Required Changes

## Stakeholder Validation Notes

## Readiness Decision

Ready for design: Yes/No
Reason:
```

## Quality Checklist

- Requirement yang vague atau terlalu besar ditandai.
- Acceptance criteria cocok dengan requirement.
- Konflik belum disembunyikan.
- Keputusan ready/not ready dijelaskan.

## Handoff

Jika valid, lanjut ke 06-se-architecture-design. Jika tidak, kembali ke elicitation/specification.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.