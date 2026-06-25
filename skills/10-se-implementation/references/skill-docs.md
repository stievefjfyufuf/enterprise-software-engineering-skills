# 10 Implementation Skill Docs

## When To Use

Gunakan saat satu issue siap dikerjakan menjadi perubahan code yang scoped.

## Required Inputs

- Selected issue with acceptance checklist and traceability IDs.
- Repo context, local patterns, architecture/design/API/UI specs.
- Migration/config expectations and test expectations.

## Step Procedure

1. Read the relevant repo structure, existing patterns, tests, and ownership boundaries before editing.
2. Confirm the issue scope and list explicit out-of-scope behavior.
3. Make the smallest cohesive code change that satisfies the acceptance checklist.
4. Preserve existing behavior unless the issue or change request explicitly approves the change.
5. Add migrations/config changes only when required and document rollback or compatibility impact.
6. Run focused verification where possible and record commands/results.
7. Send diff and implementation notes to `11-se-code-review`.

## Output Template

```markdown
# Implementation Notes

## Issue

## Files Changed

| File | Reason |
|---|---|

## Approach

## Behavior Implemented

## Migration/Config Changes

## Manual Verification

## Risks
```

## Traceability IDs

- Keep the selected `ISSUE` ID in implementation notes.
- Reference changed behavior back to `REQ`, `AC`, and `CR` when applicable.

## Mini Example

```markdown
## Issue
ISSUE-001 linked to REQ-001 and AC-001.

## Files Changed
| File | Reason |
|---|---|
| src/features/equipment/overdue.ts | Implements overdue filtering for API-001 |

## Manual Verification
Command: npm test -- overdue
Result: Pass
```

## Quality Checklist

- Repo dan pattern lokal dibaca dulu.
- Perubahan hanya sesuai issue atau approved scope.
- Behavior memenuhi acceptance criteria.
- Tidak mengubah baseline di luar scope.

## Handoff

Bawa diff dan implementation notes ke 11-se-code-review.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.
