# 08 UI Design Skill Docs

## When To Use

Gunakan saat halaman, navigasi, form, state UI, wireframe, dan user flow perlu dirancang.

## Required Inputs

- User stories, acceptance criteria, and priority order.
- API contract, domain workflow, target users, and device/platform expectations.
- Brand/design system constraints if they exist.

## Step Procedure

1. Derive screens and flows from user goals and acceptance criteria.
2. Assign screen/flow IDs such as `UI-001` and link them to `REQ`, `AC`, and `API` IDs.
3. Define navigation, primary actions, secondary actions, form fields, validation messages, and permissions.
4. Specify loading, empty, error, success, disabled, unauthorized, and destructive-action states.
5. Include accessibility and responsive behavior notes when UI is user-facing.
6. Call out data displayed, data submitted, and API dependency for each screen.
7. Send screen specs and UI flow to `09-se-issue-planning`.

## Output Template

```markdown
# UI Design

## Screen List

| Screen | User Goal | Main Actions | Data Needed |
|---|---|---|---|

## Navigation Flow

## Forms

| Form | Field | Type | Validation | Error Message |
|---|---|---|---|---|

## UI States

- Loading:
- Empty:
- Error:
- Success:

## Wireframe Notes
```

## Traceability IDs

- Use `UI-###` for screens, flows, or major UI states.
- Link each `UI` item to `REQ`, `AC`, and relevant `API`.

## Mini Example

```markdown
## Screen List
| Screen | User Goal | Key Data | Linked IDs |
|---|---|---|---|
| UI-001 Overdue Equipment Dashboard | Admin reviews overdue items | equipment, borrower, dueDate | REQ-001, AC-001, API-001 |

## UI States
- Empty: show "No overdue equipment" and last updated time.
- Error: show retry action and preserve filters.
```

## Quality Checklist

- Setiap screen punya user goal.
- Navigasi mendukung alur utama.
- Form field dan validasi jelas.
- Loading, empty, error, dan success state dicatat.

## Handoff

Bawa screen specs dan UI flow ke 09-se-issue-planning.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.
