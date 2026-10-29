---
tags: [project, decisions]
status: active
updated: 2026-10-21
---

# Decisions

A running log of significant build and documentation decisions.

## Format

```text
## YYYY-MM-DD — Title

**Context:** Why the decision was needed.

**Options considered:**
- Option A
- Option B

**Decision:** What was chosen.

**Consequences:** What this means for the build and documentation.
```

## 2026-10-21 — Split kitchen, shower and toilet documentation

**Context:** The combined page mixed requirements, BOM items and shopping links, and the toilet was not documented at all.

**Options considered:**
- Keep one combined page.
- Split into an overview page plus `Kitchen`, `Shower` and `Toilet`.

**Decision:** Split into an overview page plus three focused pages.

**Consequences:** Each area can have its own requirements, BOM and open questions. The overview page remains the entry point.

## 2026-10-21 — Composting / separating toilet

**Context:** The build is intended to be self-sustaining and should avoid a black-water tank if possible.

**Options considered:**
- Cassette toilet.
- Composting / separating toilet.
- Incinerating toilet.
- Porta potti.

**Decision:** Use a composting / separating toilet. It should be portable so it can be moved out of the shower compartment when the shower is in use. The model is still open.

**Consequences:** No black-water tank is required. A vent, urine container, solids container, cover material and emptying access are required. The final model will determine the vent and footprint.

## 2026-10-21 — Hamwells Loopz Plus shower

**Context:** A recirculating shower greatly reduces fresh-water use, which suits an off-grid build.

**Options considered:**
- Conventional shower draining to the grey tank.
- Loopz Plus recirculating shower.

**Decision:** Use the Hamwells Loopz Plus.

**Consequences:** The Loopz base becomes the shower floor. Walls use 3×2 CLS battens with 6 mm PVC/compact laminate panels and a rubber trim sealing the base. The unit slides in and out. It needs a 12 V supply, a fill method, a drain to the grey tank and ventilation. It does not heat water.

## 2026-10-21 — Kettle-only hot water

**Context:** A calorifier or hot-water tank adds plumbing, weight, winter-freezing risk and cost.

**Decision:** Do not install a hot-water system. Use a kettle when hot water is needed.

**Consequences:** The kitchen sink is cold-water only. The shower must use ambient or preheated water. Loopz water must not exceed 45 °C. The kettle must be inverter-compatible.

## 2026-10-21 — 1.5 kW appliance limit

**Context:** The planned inverter is 2000 W and the AGM battery bank is relatively small.

**Decision:** Limit the induction hob and kettle to 1.5 kW each and run them from the inverter.

**Consequences:** Do not run the hob and kettle simultaneously. Check inverter surge, cable size, fuse rating and battery capacity. A low-wattage kettle is required.

## 2026-10-21 — Underslung 75 L fresh / 45 L grey tanks

**Context:** Interior space is limited, so the tanks will be mounted underneath the ambulance.

**Decision:** Use a 75 L fresh tank and a 45 L grey tank, both underslung.

**Consequences:** The tanks and pipework need insulation and heating to prevent freezing. Mounting, protection from road debris, fill and drain access, and level sensing must be designed.

## 2026-10-21 — Cancel roof decking and ladder; keep 800 W solar

**Context:** The metal decking and ladder were no longer required.

**Decision:** Cancel the roof decking and ladder. Keep the installed 800 W solar array.

**Consequences:** The roof is used for solar and service penetrations only. The roof page records measurements and penetrations for future work. The ladder page is retained as a cancelled reference.

## 2026-10-21 — Shower wall build: plastic panels

**Context:** Plastic waterproof panels simplify the wall finish and avoid tanking plywood.

**Options considered:**
- 6 mm plywood plus waterproof tanking.
- 6 mm solid PVC or compact laminate panels on 3×2 CLS battens.

**Decision:** Use Option B: 6 mm solid PVC or compact laminate panels on 3×2 CLS battens at 300 mm centres, mechanically fixed with stainless screws and sealing washers.

**Consequences:** The panels need a rigid frame, expansion gaps, flexible sealant and H-trims. Battens must fix into the van's structural ribs. The panel fire rating must be checked, especially near the diesel-heater outlet. Plastic panels are not automatically lighter than 6 mm ply.

## 2026-10-21 — New shower roof extractor

**Context:** The existing black roof extractor is not being reused.

**Decision:** Install a new 12 V shower extractor with humidity sensor/timer and a new roof vent.

**Consequences:** A new roof penetration, duct, cowl, insect mesh and backdraught shutter are required. The roof layout must avoid the solar panels and existing penetrations.

## 2026-10-21 — Diesel heater drying branch with changeover

**Context:** The Eberspächer Airtronic D4 is already mounted and can supply dry heat to the shower.

**Decision:** Duct 89 mm hot air to the shower through a changeover damper, so the heater can supply either the living space or the shower. The 76 mm return draws from the dry living space. The 24 mm combustion air and exhaust terminate outside.

**Consequences:** The main heater outlet must remain open; the shower branch must not dead-end the heater. A high-temperature diffuser, heat shield, CO alarm and Eberspächer 802 controller are required. See [[Diesel Heater]].

## 2026-10-21 — Loopz conservative design figures

**Context:** The Loopz manuals and web page disagree on power, weight and maximum water temperature.

**Decision:** Design to 60 W / 5 A, 10 kg unit weight plus 6 kg water, 45 °C maximum water temperature and 100 kg maximum deck load until Hamwells confirms otherwise.

**Consequences:** Wiring and fusing use the 60 W figure. The floor supports 16 kg. Preheated water must be mixed to 45 °C or below. Users close to 100 kg should check the deck limit with Hamwells.

## 2026-10-21 — Toilet vent at lower back wall

**Context:** The composting toilet is portable but needs a fixed vent.

**Decision:** Provide a fixed vent at the lower section of the back wall of the shower compartment, with a removable connection to the toilet.

**Consequences:** The toilet must dock or connect to the vent when in use. The final toilet model determines whether it uses an integrated fan, flexible hose or docking hood.

## 2026-10-21 — Loopz 12 V socket outside the cubicle

**Context:** The Loopz manual requires the power adapter to be in a dry environment.

**Decision:** Put the 12 V socket outside the shower cubicle.

**Consequences:** Cable and conduit must pass into the cubicle to the Loopz control panel, with a drip loop and a sealed entry.

## Related

- [[Dashboard]]
- [[Kanban]]
- [[Shopping List]]
- [[Kitchen, Shower & Toilet]]
- [[Shower]]
- [[Toilet]]
- [[Water]]
- [[Ventilation & Moisture]]
- [[Diesel Heater]]
- [[Electrics Overview]]
