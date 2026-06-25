# 01 Inception dan Stakeholder Skill Docs

## When To Use

Gunakan saat proyek baru dimulai, ide aplikasi masih kasar, scope belum jelas, atau stakeholder belum dipetakan.

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
# Problem Statement

## Background

## Primary Problem

## Goals

## Stakeholders

| Stakeholder | Role | Needs | Influence | Notes |
|---|---|---|---|---|

## Scope

### In Scope

### Out of Scope

## Assumptions

## Constraints

## Open Questions
```

## Quality Checklist

- Masalah utama jelas dan tidak langsung loncat ke solusi.
- Stakeholder primer dan sekunder teridentifikasi.
- Scope awal punya batas in-scope dan out-of-scope.
- Asumsi dan pertanyaan terbuka dicatat.

## Handoff

Bawa stakeholder map dan open questions ke 02-se-elicitation.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.