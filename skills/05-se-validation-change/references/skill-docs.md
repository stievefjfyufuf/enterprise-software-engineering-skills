# 05 Validation dan Change Skill Docs

## When To Use

Gunakan saat requirement perlu diperiksa kelengkapan, konsistensi, testability, atau saat ada perubahan requirement awal.

## Required Inputs

- Prioritized requirements, acceptance criteria, and conflict log.
- Stakeholder feedback or approval notes.
- Open questions, constraints, and readiness concerns.

## Step Procedure

1. Validate each requirement for clarity, completeness, consistency, feasibility, testability, and traceability.
2. Check that each `AC` can be verified manually or automatically.
3. Mark each requirement as ready, needs clarification, changed, rejected, or deferred.
4. Record stakeholder validation notes and decision owner.
5. If the change is material, create an early change note and route back to elicitation/specification as needed.
6. Publish a readiness decision before design starts.
7. Send ready requirements to `06-se-architecture-design`; send unclear items back to `02` or `03`.

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

## Traceability IDs

- Keep `REQ`, `NFR`, and `AC` IDs stable.
- Use `VAL-###` for validation findings.
- Use `DEC-###` for stakeholder readiness decisions.

## Mini Example

```markdown
## Issues Found
- VAL-001: REQ-003 has no measurable acceptance criteria.

## Readiness Decision
Ready for design: No
Reason: REQ-003 returns to 03-se-specification; all other MVP requirements are ready.
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
