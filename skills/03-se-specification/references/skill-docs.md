# 03 Specification Skill Docs

## When To Use

Gunakan saat kebutuhan mentah perlu diubah menjadi requirement, user story, non-functional requirement, dan acceptance criteria.

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