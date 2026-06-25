# 02 Elicitation Skill Docs

## When To Use

Gunakan saat perlu menggali kebutuhan dari stakeholder melalui interview, survey, workshop, observasi, atau analisis dokumen.

## Required Inputs

- Stakeholder map from step 01.
- Goals, assumptions, constraints, and open questions.
- Domain context, existing process notes, or current system screenshots/docs if available.

## Step Procedure

1. Group questions by stakeholder ID and goal ID.
2. Choose elicitation techniques: interview for tacit knowledge, survey for broad preference, workshop for conflict resolution, observation for workflow gaps, document analysis for rules.
3. Capture raw needs with IDs such as `NEED-001`; do not convert them into technical solutions yet.
4. Mark each need as explicit, inferred, constraint, pain point, policy/rule, or unresolved.
5. Record ambiguity, conflicts, missing data, and follow-up questions.
6. Preserve source traceability from stakeholder or document to each need.
7. Prepare raw needs and ambiguity/conflict notes for `03-se-specification`.

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

## Traceability IDs

- Use `NEED-###` for raw stakeholder needs.
- Link every `NEED` to `STK`, `GOAL`, or source document.
- Use `Q-###` for follow-up questions when a decision is blocked.

## Mini Example

```markdown
## Questions
- Q-001 for STK-001: Who is allowed to approve an equipment request?

## Raw Needs
- NEED-001: Lab admin needs to see overdue borrowed equipment. Source: STK-001. Goal: GOAL-001.

## Ambiguities
- Q-002: Define whether overdue means same day, 24 hours, or scheduled return date.
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
