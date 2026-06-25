---
name: 09-se-issue-planning
description: Mengubah requirement menjadi GitHub Issues atau task teknis. Use when breaking validated requirements and designs into implementation issues, tasks, subtasks, labels, dependencies, milestones, sprint backlog, or developer-ready work items.
---

# Issue Planning

## Purpose

Use this skill to mengubah requirement dan design menjadi task implementasi.


## Skill Docs

For detailed step documentation, templates, checklist, and handoff guidance, read references/skill-docs.md after this file when the user asks for full docs or when the step output needs more structure.

## Inputs

Validated requirements, architecture, ERD, API contract, UI specs, priority order.

## Workflow

- Buat satu issue untuk satu outcome yang dapat direview.
- Tuliskan context, scope, acceptance criteria, technical notes, dependencies, and out-of-scope.
- Pecah issue besar menjadi backend, frontend, database, test, and documentation tasks jika perlu.
- Urutkan issue berdasarkan dependency dan prioritas.
- Pastikan setiap issue traceable ke requirement atau change request.

## Output

Issue list, task breakdown, acceptance checklist per issue, dependency map, milestone/sprint grouping.

## Handoff

Kirim satu issue terpilih ke 10-se-implementation.

## Quality Rules

- Keep the work scoped to this skill's single responsibility.
- Preserve traceability to stakeholder goals, requirements, issues, tests, or change requests.
- For enterprise-scale work, call out risk, ownership, dependency, compliance, security, and rollback concerns when relevant.
- Do not overwrite existing baseline artifacts unless the user explicitly asks for replacement and the change is logged.
