# 01 Inception dan Stakeholder Skill Docs

## When To Use

Gunakan saat proyek baru dimulai, ide aplikasi masih kasar, scope belum jelas, atau stakeholder belum dipetakan.

## Required Inputs

- App idea or business problem.
- Target users or customer segment.
- Known constraints such as deadline, budget, platform, compliance, or team size.
- Any existing notes, pitch, assignment brief, or product context.

## Step Procedure

1. Restate the problem without jumping directly to a solution.
2. Identify stakeholder groups and assign stable IDs such as `STK-001`.
3. Separate business goals, user goals, and technical goals with IDs such as `GOAL-001`.
4. Define in-scope, out-of-scope, assumptions, constraints, and success signals.
5. Record unresolved questions that must be answered during elicitation.
6. Call out early enterprise concerns: ownership, compliance, security, data sensitivity, dependencies, and operational risk.
7. Prepare a handoff artifact for `02-se-elicitation`.

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

## Traceability IDs

- Use `STK-###` for stakeholders.
- Use `GOAL-###` for goals.
- Use `ASSUMP-###` for assumptions when they affect scope or risk.

## Mini Example

```markdown
## Primary Problem
Lab staff cannot reliably track who borrowed equipment and when it should be returned.

## Goals
- GOAL-001: Reduce lost equipment by improving borrow/return visibility.

## Stakeholders
| Stakeholder | Role | Needs | Influence | Notes |
|---|---|---|---|---|
| STK-001 Lab Admin | Operational owner | Approve requests and audit inventory | High | Owns daily workflow |
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
