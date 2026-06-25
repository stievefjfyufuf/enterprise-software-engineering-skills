# 04 Prioritization Skill Docs

## When To Use

Gunakan saat backlog requirement perlu diurutkan, MVP ditentukan, atau konflik kebutuhan diselesaikan.

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
# Prioritization Matrix

| Requirement ID | Value | Risk | Effort | Dependency | Priority | Rationale |
|---|---:|---:|---:|---|---|---|

## MVP Scope

## Next Release

## Deferred

## Conflict Log

| Conflict | Stakeholders | Decision | Rationale |
|---|---|---|---|
```

## Quality Checklist

- Prioritas punya alasan, bukan hanya angka.
- MVP jelas dan realistis.
- Dependency dipertimbangkan.
- Konflik requirement dicatat bersama keputusan.

## Handoff

Bawa prioritized backlog dan conflict log ke 05-se-validation-change.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.