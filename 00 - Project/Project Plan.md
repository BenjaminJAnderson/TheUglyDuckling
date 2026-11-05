---
tags: [project, plan, scheduling]
status: active
updated: 2026-11-05
---

# Project Plan

## Overview

This page is the scheduling framework for the current wet-area phase: kitchen, shower, toilet, water, waste, ventilation and electrical work. It defines how work moves from the Kanban procurement board into dated Gantt notes, how deadlines are set and how the plan is reviewed and re-baselined.

The plan is deliberately provisional. Task dates are estimates; the phase gates are the committed checkpoints.

## Source of truth

| Artefact | Purpose | Scheduled? |
| --- | --- | --- |
| [[Kanban]] | Procurement working board: decisions, sourcing, prices and pre-order states | No; dates stay in `Tasks/` |
| `00 - Project/Tasks/` | Committed work with dates and dependencies | Yes |
| [[Shopping List]] | Purchase reference and BOM status | No |
| [[Decisions]] | Why a choice or re-baseline happened | n/a |
| This page | Framework, baseline, gates and review rules | n/a |

Rules:

- Nothing gets a `start` or `end` date until it is committed.
- Unscheduled work and pre-order procurement states stay on [[Kanban]] without dates, so the Gantt stays clean.
- Scheduled work lives in one dated task note. The Kanban may mirror that action as a procurement state (decide, research, ready, ordered, received); update or close the matching card when the task changes. Do not put dates on Kanban cards.
- Completed tasks are archived at phase close so the active Gantt stays readable.

## Baseline assumptions

- Start date: **Monday 2 November 2026**.
- Availability: **2 full build days per week**, typically at weekends, plus weekday admin.
- No holiday freeze. The Christmas and New Year period is available for work and buffer.
- Procurement lead time: **3 weeks** for long-lead items. Confirm this with suppliers before relying on it.
- Scope: the current wet-area phase only. Exterior, furniture and other conversion work stay on [[Kanban]].
- The Gantt is not resource-levelled. Overlapping bars mean tasks can be interleaved within the window, not that one person can do them simultaneously.

If the build days or lead times change, update this section and re-baseline the phase windows. At one build day per week, expect the baseline to roughly double.

## Phase and milestone baseline

| Phase | Window | Indicative effort | Gate |
| --- | --- | --- | --- |
| 0 Define and decide | 2–20 Nov 2026 | 13 design/admin days | **M01 Design freeze — Fri 20 Nov 2026** |
| 1 Procure | 23 Nov–18 Dec 2026 | 6 procurement days | **M02 Long-lead orders placed — Fri 27 Nov 2026**<br>**M03 Long-lead received and inspected — Fri 18 Dec 2026** |
| 2 Strip-out and first-fix | 19 Dec 2026–10 Jan 2027 | 9 build days | **M04 First-fix complete — Sun 10 Jan 2027** |
| 3 Shower build | 11–31 Jan 2027 | 6 build days | **M05 Shower watertight — Sun 31 Jan 2027** |
| 4 Toilet and kitchen | 1–21 Feb 2027 | 5 build days | **M06 Toilet and kitchen installed — Sun 21 Feb 2027** |
| 5 Commissioning | 22 Feb–7 Mar 2027 | 3 build days | **M07 Systems commissioned — Sun 7 Mar 2027** |
| 6 Snag and handover | 8–21 Mar 2027 | 2 build days | **M08 Phase complete — Sun 21 Mar 2027** |

The final build block of each phase is reserved as buffer. Phase 2 may need one weekday block because it carries nine build days over four weekends. If a gate is at risk, move the downstream window and record the re-baseline in [[Decisions]].

### Effort check

- Phase 2 is the tightest phase: it needs nine build days against eight weekend days. Plan one weekday block, or extend the phase by a weekend. If the tanks, heater branch or electrical first-fix run long, extend Phase 2 rather than compressing the shower build.
- Phase 3 depends on the Loopz arriving by M03. A late Loopz delivery moves the base fit, drain connection and water test week for week.
- Phase 4 can start once first-fix is complete; the toilet and kitchen do not need the shower to be watertight.

## Critical path

1. Confirm Loopz specification and order it → receive → fit base → connect drain → water test.
2. Confirm tank specification and order → receive → mount tanks → drain and vent → leak test.
3. Confirm load schedule and DC-DC wiring → order electrical core → install protection → install DC-DC → install inverter and consumer unit → test circuits.

Procurement lead times are the largest schedule risk. Orders are therefore placed before fabrication starts, with M03 as the receive-and-inspect gate.

## Task note format

Create task notes from [[Task Template]]. One note is one actionable task.

```yaml
---
tags: [task, area/shower, phase/build]
status: todo
start: 2027-01-11
end: 2027-01-17
effort_days: 2
progress: 0
after:
  - "FS:[[S05 Install wall frame, noggins and insulation]]"
updated: 2026-10-29
---
```

| Field | Meaning |
| --- | --- |
| `start` | First calendar day of the task window, `YYYY-MM-DD` |
| `end` | Last calendar day, inclusive |
| `effort_days` | Focused work days required; a custom Gantt column |
| `status` | `todo`, `in-progress`, `blocked`, `done`; optional `cancelled` |
| `progress` | Percentage complete, 0–100 |
| `after` | Dependency list; default FS, or `SS:` / `FF:` |
| `milestone` | `true` on end-only milestone notes |
| `parent` | Optional; not used in version one |

Rules:

- Use `FS` for normal handoffs, `SS` when two tasks start together after a shared prerequisite, and `FF` when they must finish together.
- `SF` is not supported by the plugin.
- Keep dependencies limited to real handoffs. A shallow graph is easier to maintain.
- Milestones use `end` only and `milestone: true`; they render as diamonds.
- Do not use the `due` key. The plugin reads `end` and displays it as Due.
- Do not add dates to tasks that are not committed.

## Gantt setup

The plugin settings live in `.obsidian/`, which is gitignored. Configure them on each machine:

| Setting | Value |
| --- | --- |
| Default folder | `00 - Project/Tasks` |
| Recurse | On |
| Group by | Folder (area) |
| Date format | `YYYY/MM/DD` for display; frontmatter stays ISO |
| Default zoom | Week |
| Non-working days | None while using calendar windows |
| Statuses | `todo`, `in-progress`, `blocked`, `done`, optional `cancelled` |
| Visible columns | start, end, status, progress, `effort_days`, tags |
| Colour by | Status |
| Progress line | On |
| Auto-schedule FS | Off until the baseline is stable |

Open the view from the ribbon and select `00 - Project/Tasks`. Because the plugin is note-per-task, it does not read Kanban cards.

## Folder structure

```text
00 - Project/
├── Project Plan.md
├── Task Template.md
├── Tasks/
│   ├── 00 Milestones/
│   ├── 10 Shower/
│   ├── 20 Toilet/
│   ├── 30 Water/
│   ├── 40 Electrics/
│   ├── 50 Ventilation & Heating/
│   ├── 60 Kitchen/
│   └── 90 Cross-cutting/
├── Kanban.md
├── Decisions.md
└── Shopping List.md
```

`Task Template.md` sits outside `Tasks/` so it never appears in the Gantt. Archived tasks move to `00 - Project/Archive/Tasks/`, outside the Gantt folder.

## Workflow

1. Capture an idea, research question or buy-now item on [[Kanban]].
2. When it is ready to schedule, create a task note from [[Task Template]].
3. Give it an outcome, done criteria, `effort_days` and dependencies.
4. Place `start` and `end` inside the relevant phase window.
5. Update or complete the matching Kanban card; dates remain only in the task note.
6. Update `status` and `progress` at the weekly review.
7. At phase close, archive completed tasks and update the as-built documentation.

## Review cadence

### Weekly review

- Update `status` and `progress` on every active task.
- Confirm the next two weeks are realistic.
- Check blocked tasks and name the blocker in the task body.
- Check outstanding orders and expected delivery dates.
- Check whether the next gate is at risk.

### Monthly review

- Re-baseline phase windows if a gate has slipped.
- Review the critical path and the procurement chain.
- Archive completed tasks from the previous phase.
- Record significant scope or date changes in [[Decisions]].

### Gate review

- Confirm the gate criteria in the milestone note.
- Record evidence and photo links in the milestone body.
- Mark the milestone `done` only when the criteria are met.
- Re-baseline downstream tasks before starting the next phase.

## Milestones

- [[M01 Design freeze]]
- [[M02 Long-lead orders placed]]
- [[M03 Long-lead received and inspected]]
- [[M04 First-fix complete]]
- [[M05 Shower watertight]]
- [[M06 Toilet and kitchen installed]]
- [[M07 Systems commissioned]]
- [[M08 Phase complete]]

## Related

- [[Dashboard]]
- [[Kanban]]
- [[Decisions]]
- [[Shopping List]]
- [[Task Template]]
- [[Kitchen, Shower & Toilet]]
