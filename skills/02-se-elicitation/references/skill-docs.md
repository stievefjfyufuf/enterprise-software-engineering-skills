# 02 Elicitation Skill Docs

## When To Use

Gunakan saat perlu menggali kebutuhan dari stakeholder melalui interview, survey, workshop, observasi, atau analisis dokumen.

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
# Elicitation Notes

## Stakeholder

## Technique

## Questions

| Question | Purpose | Answer | Follow-up Needed |
|---|---|---|---|

## Raw Needs

## Pain Points

## Constraints Found

## Ambiguities

## Conflicts
```

## Quality Checklist

- Pertanyaan dikelompokkan per stakeholder atau tujuan.
- Kebutuhan mentah tidak langsung diubah menjadi solusi teknis.
- Ambiguitas dan konflik dicatat.
- Ada follow-up untuk jawaban yang belum jelas.

## Handoff

Bawa raw needs, answers, ambiguity list, dan conflict notes ke 03-se-specification.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.