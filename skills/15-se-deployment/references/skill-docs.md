# 15 Deployment Skill Docs

## When To Use

Gunakan saat release, deployment checklist, migration rollout, smoke test, rollback, dan post-deploy verification perlu dilakukan.

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
# Deployment Plan

## Release Scope

## Pre-Deployment Checklist

- [ ] Build ready
- [ ] Tests passed
- [ ] Environment configured
- [ ] Migration reviewed

## Deployment Steps

## Smoke Tests

## Rollback Plan

## Release Notes

## Post-Deployment Result

## New Baseline
```

## Quality Checklist

- Build, tests, env, secret, dan migration readiness jelas.
- Rollback plan tersedia.
- Smoke test dilakukan.
- Baseline baru ditandai setelah deployment berhasil.

## Handoff

Jika ada incident atau feedback produksi, kirim ke 16-se-change-log-engineering-loop.

## Common Mistakes To Avoid

- Do not skip traceability.
- Do not rewrite a baseline artifact outside the approved scope.
- Do not mix this step with unrelated downstream implementation work.
- Do not hide conflicts, assumptions, or unresolved questions.