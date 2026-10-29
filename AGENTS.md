# AGENTS.md

## Project

**The Ugly Duckling** is an ambulance being converted into a self-sustaining, off-grid liveaboard.

Current phase: **kitchen, shower and toilet area**, plus the supporting water, waste and electrical systems.

## Current design decisions

- **Toilet:** composting / separating toilet. It should be portable so it can be moved out of the shower compartment when the shower is in use. Model still to be chosen.
- **Shower:** Hamwells Loopz Plus recirculating shower. Semi-permanent installation:
  - The Loopz base is the shower-compartment floor.
  - Walls are 3×2 CLS battens at 300 mm centres, fixed to structural ribs, with 6 mm solid PVC or compact laminate waterproof panels.
  - Panels are mechanically fixed with stainless screws and sealing washers; joints use H-trims and neutral-cure silicone.
  - The Loopz base slides into place and is sealed with a waterproof rubber trim that can be removed for servicing.
  - The unit can be removed for servicing or storage.
  - Design figures: 60 W / 5 A, 10 kg unit plus 6 kg water, 45 °C maximum water temperature, 100 kg maximum deck load.
- **Shower ventilation:** new 12 V roof extractor with humidity sensor/timer. The old black roof extractor is not reused.
- **Diesel heater:** Eberspächer Airtronic D4 12 V Mk1 with 802 controller, already mounted.
  - 89 mm hot-air duct to the shower through a changeover damper, so the heater can supply either the living space or the shower.
  - 76 mm return air from the dry living space, not the shower.
  - 24 mm combustion air and exhaust terminate outside.
  - The main heater outlet must remain open; do not dead-end the heater.
- **Toilet vent:** fixed vent at the lower section of the back wall of the shower compartment, with a removable connection to the portable composting toilet.
- **Loopz power:** 12 V socket outside the shower cubicle, in a dry location.
- **Hot water:** no calorifier, hot-water tank or hot-water plumbing. A kettle is used when hot water is wanted.
  - The Loopz Plus does **not** heat water and has a maximum water temperature of **45 °C**.
  - If preheated water is used, mix it down to 45 °C or below.
- **Kitchen:** cold water only. No recirculating tap. The induction hob and kettle are limited to **1.5 kW each** and run from the inverter.
- **Water tanks:** underslung. **75 L fresh** and **45 L grey**. Insulation and heating are required to prevent freezing.
- **Solar:** **800 W** installed as 4 × 200 W panels. No roof decking and no ladder.
- **Electrical:** 12 V leisure system with a Xantrex PROwatt SW 2000i inverter, Sterling Pro Charge Ultra 60 A shore charger, 60 A MPPT and an AGM leisure bank. Final battery chemistry and capacity are still open.

## Repository map

```text
00 - Project/          Dashboard, Kanban, decisions, shopping list, page template
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

- Status values: `idea`, `research`, `shortlisted`, `ordered`, `received`, `installed`, `cancelled`.
- Record significant choices in `[[Decisions]]` with the date, context, options and consequences.
- Mark assumptions and open questions explicitly. Do not invent specifications.
- Link each page back to `[[Dashboard]]` and to the relevant system page.
- Use tags in frontmatter, not inline code tags.

## Safety and build notes

- Keep 230 V AC and water separated; use RCD/RCBO protection and drip loops.
- Fuse DC circuits close to the source.
- The 2 kW inverter and 1.5 kW loads are demanding on the planned AGM bank. Check battery capacity, cable size and fuse ratings before installation.
- Ventilation is critical: kitchen extractor, shower extractor and composting-toilet vent.
- Insulate and heat the underslung tanks and pipework for winter use.
- Do not edit CAD, GCODE, STL, DXF or KiCad files unless explicitly asked.
- Never commit secrets, keys or personal credentials.

## Workflow

1. Update the relevant page and its BOM.
2. Update `[[Shopping List]]` when an item becomes shortlisted or ordered.
3. Record the reason for a change in `[[Decisions]]`.
4. Update `[[Kanban]]` with the next physical task.
