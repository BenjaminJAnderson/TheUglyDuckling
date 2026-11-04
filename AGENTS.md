# AGENTS.md

## Project

**The Ugly Duckling** is an ambulance being converted into a self-sustaining, off-grid liveaboard.

Current phase: **kitchen, shower and toilet area**, plus the supporting water, waste and electrical systems.

## Current design decisions

- **Toilet:** BOXIO TOILET XL MAX+ separating toilet, portable so it can be moved out of the shower compartment when the shower is in use. 7 L urine / 8 L solids, 40 × 30 cm, 45 cm high with the Solo Up base, 5.8 kg. No water, chemicals or power. Model selected 2026-11-02; stock and lead time TBC.
- **Shower:** Hamwells Loopz Plus recirculating shower. Semi-permanent installation:
  - The Loopz base is the shower-compartment floor.
  - Walls are 3×2 CLS battens at 300 mm centres, fixed to structural ribs, with plywood-backed **2 mm black PVC hygienic cladding**.
  - Three walls, approximately **1970 × 700 mm**, using Hygienic Plastic Supplies SKU `B2104` (3050 × 1220 × 2 mm, £49.99 + VAT per sheet); three sheets minimum.
  - The plywood backing provides stiffness and impact resistance; its thickness and grade are TBC. The cladding is bonded and/or mechanically fixed to the plywood; joints use H-trims and neutral-cure silicone.
  - The Loopz base slides into place and is sealed with a waterproof rubber trim that can be removed for servicing.
  - The unit can be removed for servicing or storage.
  - Design figures: 60 W / 5 A, 10 kg unit plus 6 kg water, 45 °C maximum water temperature, 100 kg maximum deck load.
- **Shower ventilation:** new 12 V roof extractor with humidity sensor/timer. The old black roof extractor is not reused.
- **Diesel heater:** Eberspächer Airtronic D4 12 V Mk1 with 802 controller, already mounted.
  - 89 mm hot-air duct to the shower through a changeover damper, so the heater can supply either the living space or the shower.
  - 76 mm return air from the dry living space, not the shower.
  - 24 mm combustion air and exhaust terminate outside.
  - The main heater outlet must remain open; do not dead-end the heater.
- **Toilet ventilation:** no dedicated toilet vent. The Boxio has no integrated fan or direct vent port; odour control relies on the plug/odour trap, hemp litter and the shower/room extractor.
- **Loopz power:** 12 V socket outside the shower cubicle, in a dry location.
- **Hot water:** no calorifier, hot-water tank or hot-water plumbing. A kettle is used when hot water is wanted.
  - The Loopz Plus does **not** heat water and has a maximum water temperature of **45 °C**.
  - If preheated water is used, mix it down to 45 °C or below.
- **Kitchen:** cold water only. No recirculating tap. The induction hob and kettle are limited to **1.5 kW each** and run from the inverter.
- **Water tanks:** Autocraft underslung **75 L fresh** kit and **60 L waste** tank, selected for planning. Fresh kit uses topfill with a black cap, universal brackets and Shurflo Trail King 7 pump/filter; the 60 L tank is bought with Sprinter/Crafter brackets, no kit and no pump, and the brackets need adapting to the Ducato/WAS chassis. The internal fill point is in the rear upstand behind the kitchen sink, filled from 10 L bottles over the sink. Fitment and service-hatch orientation are unconfirmed; confirm before ordering. Insulation, thermal heating mats and pipework protection are required to prevent freezing. The fresh drain tap, level sensors and waste-tank inlets are still open.
- **Solar:** **800 W** installed as 4 × 200 W panels. No roof decking and no ladder.
- **Electrical:** 12 V leisure system with a Xantrex PROwatt SW 2000i inverter, Sterling Pro Charge Ultra 60 A shore charger, 60 A MPPT and an AGM leisure bank. Final battery chemistry and capacity are still open.

## Repository map

```text
00 - Project/          Dashboard, project plan, tasks, Kanban, decisions, shopping list, templates
01 - INTERIOR/         Kitchen, shower, toilet, bed, furniture, lining
02 - SYSTEMS/          Water, ventilation, diesel heating, electrical overview and component notes
03 - EXTERIOR/         Solar, roof, caulking, lights, paint, antenna, ladder
CAD Files/             FreeCAD, STL, DXF and GCODE files
Electric Wiring Guide/ KiCad electrical design
```

## Documentation conventions

- Use **Obsidian wikilinks** for internal links: `[[Kitchen]]`, `[[Water]]`.
- Use **standard Markdown links** for external links: `[Supplier](https://example.com)`.
- Every content page starts with one `#` heading and uses `##` for sections. The Kanban page is plugin-managed and uses `##` columns.
- Add frontmatter where useful:

```yaml
---
tags: [interior, kitchen]
status: planning
updated: 2026-10-21
---
```

- Use the page template at `[[Page Template]]`.
- Keep BOMs in a consistent table:

| Item | Qty | Spec / Model | Supplier / Link | Price | Status | Notes |
| --- | --- | --- | --- | --- | --- | --- |

- Page and BOM status values: `idea`, `research`, `shortlisted`, `ordered`, `received`, `installed`, `cancelled`.
- Record significant choices in `[[Decisions]]` with the date, context, options and consequences.
- Mark assumptions and open questions explicitly. Do not invent specifications.
- Link each page back to `[[Dashboard]]` and to the relevant system page.
- Use tags in frontmatter, not inline code tags.

## Planning and scheduling

- [[Project Plan]] is the scheduling framework and baseline. Read it before adding dated work.
- [[Kanban]] is the procurement working board for ideas, research, prices and pre-order states. Dated work stays in `Tasks/`; a Kanban card may mirror an order task but must not carry dates.
- Committed work lives as one note per task under `00 - Project/Tasks/`, grouped by area.
- Task notes use `start`, `end`, `effort_days`, `status`, `progress` and `after`. Dates are ISO `YYYY-MM-DD`.
- Task statuses are `todo`, `in-progress`, `blocked` and `done`; optional `cancelled`. These are separate from page and BOM statuses.
- Dependencies use `"[[Task]]"` for finish-to-start, or `"SS:[[Task]]"` and `"FF:[[Task]]"`. `SF` is not supported.
- Milestones use `end` only plus `milestone: true` and represent the committed phase gates.
- Create tasks from [[Task Template]]. The template must not contain `start` or `end`, so it stays out of the Gantt.
- Do not put dates on Kanban cards, unscheduled ideas or individual BOM lines.
- Gantt settings live in `.obsidian/` and are not committed; the setup is documented in [[Project Plan]].

## Safety and build notes

- Keep 230 V AC and water separated; use RCD/RCBO protection and drip loops.
- Fuse DC circuits close to the source.
- The 2 kW inverter and 1.5 kW loads are demanding on the planned AGM bank. Check battery capacity, cable size and fuse ratings before installation.
- Ventilation is critical: kitchen extractor, shower extractor and toilet compartment ventilation. The Boxio has no dedicated toilet vent.
- Insulate and heat the underslung tanks and pipework for winter use.
- Do not edit CAD, GCODE, STL, DXF or KiCad files unless explicitly asked.
- Never commit secrets, keys or personal credentials.

## Workflow

1. Update the relevant page and its BOM.
2. Update `[[Shopping List]]` when an item becomes shortlisted or ordered.
3. Record the reason for a change in `[[Decisions]]`.
4. Update the relevant task note's `status` and `progress`, or create one from [[Task Template]].
5. Update or close the matching `[[Kanban]]` card as procurement progresses; dates stay only in `Tasks/`.
6. At a phase gate, review the milestone criteria and re-baseline downstream tasks if needed.
