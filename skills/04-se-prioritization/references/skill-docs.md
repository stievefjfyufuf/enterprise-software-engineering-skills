# 04 Prioritization Skill Docs

## When To Use

Gunakan saat backlog requirement perlu diurutkan, MVP ditentukan, atau konflik kebutuhan diselesaikan.

## Required Inputs

- Requirement set with `REQ`, `NFR`, and `AC` IDs.
- Stakeholder goals and influence.
- Constraints, deadlines, dependencies, risk notes, and compliance drivers.

## Step Procedure

1. Score each requirement by value, risk reduction, urgency, compliance impact, effort, and dependency.
2. Use MoSCoW or a simple value/risk/effort matrix; state which method is used.
3. Identify MVP items, next-release items, deferred items, and rejected items.
4. Resolve or document stakeholder conflicts with rationale and decision owner.
5. Keep dependency order explicit so implementation does not start before enabling work.
6. Preserve requirement and acceptance criteria IDs.
7. Prepare prioritized backlog and conflict log for `05-se-validation-change`.

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

## Traceability IDs

- Keep original `REQ`, `NFR`, and `AC` IDs.
- Use `DEC-###` for prioritization decisions when a tradeoff or conflict is resolved.

## Mini Example

```markdown
| Requirement ID | Value | Risk | Effort | Dependency | Priority | Rationale |
|---|---:|---:|---:|---|---|---|
| REQ-001 | 5 | 3 | 2 | None | Must | Directly supports GOAL-001 and daily admin workflow |

## Conflict Log
- DEC-001: Reporting dashboard deferred because approval flow is needed first.
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
