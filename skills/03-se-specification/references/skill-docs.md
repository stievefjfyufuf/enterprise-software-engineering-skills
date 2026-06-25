# 03 Specification Skill Docs

## When To Use

Gunakan saat kebutuhan mentah perlu diubah menjadi requirement, user story, non-functional requirement, dan acceptance criteria.

## Required Inputs

- Raw needs, stakeholder answers, ambiguity list, and conflict notes.
- Goals and constraints from earlier steps.
- Domain rules, policies, compliance requirements, and known NFRs.

## Step Procedure

1. Convert each valid raw need into one or more testable requirements.
2. Assign IDs: `REQ-###` for functional requirements, `NFR-###` for non-functional requirements, and `AC-###` for acceptance criteria.
3. Write requirements with measurable behavior, actor, condition, and expected outcome.
4. Write NFRs with evaluation method or threshold.
5. Map each requirement to source `NEED`, `GOAL`, and stakeholder.
6. Keep unresolved items as open questions instead of inventing certainty.
7. Prepare the requirement set for `04-se-prioritization`.

## Output Template

```markdown
# Requirements Specification

## Functional Requirements

| ID | Requirement | Source | Priority | Acceptance Criteria ID |
|---|---|---|---|---|

## Non-Functional Requirements

| ID | Attribute | Requirement | Measurement |
|---|---|---|---|

## User Stories

As a [actor], I want [action], so that [value].

## Acceptance Criteria

Given [context]
When [action]
Then [expected result]

## Traceability

| Requirement ID | Goal | Stakeholder | Design/Test Link |
|---|---|---|---|
```

## Traceability IDs

- Use `REQ-###` for functional requirements.
- Use `NFR-###` for measurable quality attributes.
- Use `AC-###` for acceptance criteria.
- Every `REQ` should map to at least one `NEED` or `GOAL`.

## Mini Example

```markdown
| ID | Requirement | Source | Priority | Acceptance Criteria ID |
|---|---|---|---|---|
| REQ-001 | The system shall show overdue borrowed equipment to lab admins. | NEED-001, GOAL-001 | TBD | AC-001 |

Given STK-001 opens the inventory dashboard
When equipment is past its return date
Then the item appears in an overdue list with borrower and due date.
```

## Quality Checklist

- Requirement spesifik, feasible, dan testable.
- NFR punya ukuran atau kondisi evaluasi.
- User story punya actor, action, dan value.
- Acceptance criteria bisa diuji.
- Traceability ke goal atau stakeholder tersedia.

## Handoff

Bawa requirement set ke 04-se-prioritization.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.
