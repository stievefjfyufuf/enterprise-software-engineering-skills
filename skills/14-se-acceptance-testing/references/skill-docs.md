# 14 Acceptance Testing Skill Docs

## When To Use

Gunakan saat alur lengkap pengguna perlu divalidasi sebelum deploy atau ketika stakeholder memberi feedback UAT.

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
# Acceptance Testing

## User Flow

## UAT Checklist

- [ ]

## Evidence

## Defects

## Feedback

## Decision

Accepted / Accepted with Notes / Rejected

## Follow-up
```

## Quality Checklist

- Checklist berasal dari acceptance criteria.
- Happy path dan edge case penting diuji.
- Evidence/hasil dicatat.
- Accepted/rejected decision jelas.

## Handoff

Jika accepted, lanjut ke 15-se-deployment. Jika rejected, kirim feedback ke 16-se-change-log-engineering-loop.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.