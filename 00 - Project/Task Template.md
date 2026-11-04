---
tags: [template, task]
status: template
updated: 2026-10-29
---

# Task Template

Copy this note into the relevant `Tasks/` area folder and rename it with an ID, for example `S06 Fit waterproof panels.md`.

Do **not** add `start` or `end` to this template. The Gantt only picks up dated notes, and the template must stay out of the view.

## Frontmatter

```yaml
---
tags: [task, area/shower, phase/build]
status: todo
start: YYYY-MM-DD
end: YYYY-MM-DD
effort_days: 1
progress: 0
after:
  - "FS:[[PREDECESSOR TASK]]"
updated: YYYY-MM-DD
---
```

## Body

```markdown
# S06 Fit waterproof panels

## Outcome

One sentence describing what is true when this task is finished.

## Done when

- [ ] Acceptance criterion 1
- [ ] Acceptance criterion 2
- [ ] Notes and photos added to the relevant area page

## Notes

- Relevant page: [[Shower]]
- Purchase reference: [[Shopping List]]
- Blocker or dependency, if any.

## Links

- [[Project Plan]]
- [[Dashboard]]
```

## Milestone template

```yaml
---
tags: [task, milestone]
status: todo
end: YYYY-MM-DD
milestone: true
updated: YYYY-MM-DD
---

# M0X Gate name

## Gate criteria

- [ ] Criterion 1
- [ ] Criterion 2

## Evidence

- Link or note the evidence.

## Related

- [[Project Plan]]
```
