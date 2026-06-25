# Enterprise Software Engineering Skills

This repository contains 16 Codex skills for an end-to-end software engineering workflow, from inception to deployment, with an engineering loop for controlled changes.

Use these skills when you want Codex to work like a disciplined software engineering partner: clarify the problem first, keep requirements traceable, design before coding, implement in small scoped changes, verify behavior, deploy with rollback awareness, and route future changes through a controlled baseline loop.

## Skills

01. 01-se-inception-stakeholder
02. 02-se-elicitation
03. 03-se-specification
04. 04-se-prioritization
05. 05-se-validation-change
06. 06-se-architecture-design
07. 07-se-database-api-design
08. 08-se-ui-design
09. 09-se-issue-planning
10. 10-se-implementation
11. 11-se-code-review
12. 12-se-test-planning
13. 13-se-automated-testing
14. 14-se-acceptance-testing
15. 15-se-deployment
16. 16-se-change-log-engineering-loop

## Workflow

Requirement discovery -> specification -> prioritization -> validation -> architecture -> database/API -> UI -> issues -> implementation -> review -> testing -> acceptance -> deployment -> baseline -> controlled change loop.

Recommended sequence:

1. Start with `01-se-inception-stakeholder` when the project idea is still rough.
2. Use `02-se-elicitation` and `03-se-specification` to turn stakeholder needs into testable requirements.
3. Use `04-se-prioritization` and `05-se-validation-change` to decide MVP scope and readiness.
4. Use `06-se-architecture-design`, `07-se-database-api-design`, and `08-se-ui-design` before writing implementation issues.
5. Use `09-se-issue-planning` to create developer-ready tasks.
6. Use `10-se-implementation` through `14-se-acceptance-testing` to implement, review, test, and validate.
7. Use `15-se-deployment` to release and mark the new baseline.
8. Use `16-se-change-log-engineering-loop` for every later bug fix, feature addition, refactor, or correction that affects an existing baseline.

You can skip a step only when its artifact already exists and is current. When skipping, note the artifact used as the source of truth.

## Traceability ID Standard

Use stable IDs across all artifacts so Codex can connect goals, requirements, issues, code, tests, releases, and changes:

| Prefix | Meaning | Example |
|---|---|---|
| `GOAL` | Business, user, or technical goal | `GOAL-001` |
| `STK` | Stakeholder or stakeholder group | `STK-001` |
| `NEED` | Raw elicited need | `NEED-001` |
| `REQ` | Functional requirement | `REQ-001` |
| `NFR` | Non-functional requirement | `NFR-001` |
| `AC` | Acceptance criteria | `AC-001` |
| `ADR` | Architecture decision record | `ADR-001` |
| `API` | API contract item | `API-001` |
| `UI` | Screen, flow, or UI state | `UI-001` |
| `ISSUE` | Implementation issue/task | `ISSUE-001` |
| `TEST` | Test scenario or automated test | `TEST-001` |
| `UAT` | Acceptance/UAT checklist item | `UAT-001` |
| `REL` | Release or deployment marker | `REL-001` |
| `CR` | Change request | `CR-001` |

Every downstream artifact should reference the upstream ID that justified it. For example: `ISSUE-004` should link to `REQ-002`, `AC-006`, `API-003`, and any relevant `UI-002`.

## Example Prompts

```text
Use 01-se-inception-stakeholder for this app idea: a campus inventory system for lab equipment.
```

```text
Use 03-se-specification to convert these elicitation notes into requirements, user stories, NFRs, acceptance criteria, and traceability IDs.
```

```text
Use 09-se-issue-planning to break this validated requirement set and UI/API design into GitHub-ready implementation issues.
```

```text
Use 16-se-change-log-engineering-loop. Baseline REL-002 exists, and I want to add role-based approval for equipment requests.
```

## Skill Docs

Each numbered skill includes references/skill-docs.md with detailed usage docs, output templates, quality checklist, and handoff guidance for that step.

## Install

Copy the folders inside `skills/` into your Codex skills directory, for example `~/.codex/skills`.

After copying, restart Codex or reload skills if your environment requires it. The skill folder name and the `name:` field inside each `SKILL.md` are intentionally the same.

## Quality Bar

- Keep each step scoped to its responsibility.
- Prefer explicit assumptions over hidden guesses.
- Preserve traceability IDs from step to step.
- Record conflicts, risks, ownership, dependencies, security/compliance concerns, migration impact, rollback needs, and verification evidence when relevant.
- Do not rewrite a baseline artifact outside an approved change request.
