---
tags: [project, decisions]
status: active
updated: 2026-11-04
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

**Decision:** Use a composting / separating toilet. It should be portable so it can be moved out of the shower compartment when the shower is in use. The model was selected on 2026-11-02 as the **BOXIO TOILET XL MAX+ complete set**; see the entry below.

**Consequences:** No black-water tank is required. A vent, urine container, solids container, cover material and emptying access are required. The final model will determine the vent and footprint.

## 2026-10-21 — Hamwells Loopz Plus shower

**Context:** A recirculating shower greatly reduces fresh-water use, which suits an off-grid build.

**Options considered:**
- Conventional shower draining to the grey tank.
- Loopz Plus recirculating shower.

**Decision:** Use the Hamwells Loopz Plus.

**Consequences:** The Loopz base becomes the shower floor. Walls use 3×2 CLS battens with a removable compression trim sealing the base; the trim was specified on 2026-11-04, see the entry below. The wall finish was revised on 2026-11-02 to plywood-backed 2 mm black PVC cladding. The unit slides in and out. It needs a 12 V supply, a fill method, a drain to the grey tank and ventilation. It does not heat water.

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

**Superseded 2026-11-04:** The grey tank changed to a 60 L Autocraft tank after measuring the underside; see the separate-tank decision below.

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

**Superseded:** 2026-11-02 by the black 2 mm PVC on plywood backing decision below.

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

**Superseded 2026-11-02:** The selected Boxio toilet has no direct vent port, so the dedicated lower-back-wall vent was removed. Odour control now relies on the Boxio plug/odour trap, hemp litter and compartment ventilation. See the Boxio decision below.

## 2026-10-21 — Loopz 12 V socket outside the cubicle

**Context:** The Loopz manual requires the power adapter to be in a dry environment.

**Decision:** Put the 12 V socket outside the shower cubicle.

**Consequences:** Cable and conduit must pass into the cubicle to the Loopz control panel, with a drip loop and a sealed entry.

## 2026-10-29 — Task Gantt scheduling framework

**Context:** The Kanban board held a useful backlog but no dates, effort estimates or dependencies. The Task Gantt plugin shows one note per task, so the existing cards could not appear in a timeline without being converted.

**Options considered:**
- Keep using the Kanban board as the only planning tool.
- Replace the Kanban board with the Gantt.
- Use the Kanban as intake and task notes plus the Gantt for committed work.

**Decision:** Use the Kanban as intake only, create one task note per committed action in `00 - Project/Tasks/`, and use phase milestones as the committed deadlines. The first baseline runs from 2 November 2026 to 21 March 2027, assumes two full build days per week and has no holiday freeze. Task dates are estimates; the phase gates are the checkpoints.

**Consequences:** Scheduled work has a single source of truth and a visible critical path. The Kanban no longer duplicates scheduled cards. Task notes must be kept up to date, Gantt settings must be configured locally because `.obsidian/` is gitignored, and a phase that overruns is re-baselined in this log. See [[Project Plan]].

## 2026-11-02 — Procurement-focused Kanban and budget

**Context:** The Kanban backlog held next-phase work and duplicated design tasks already in `Tasks/`, so it did not support the procurement critical path. Most BOM lines had no price or lead time, and [[Shopping List]] had no budget summary or order batching.

**Options considered:**
- Keep the Kanban as an intake-only board and add only the missing research.
- Use the Kanban as the active procurement pipeline, allowing cards to mirror order tasks.
- Create a separate procurement page and leave the Kanban as an idea intake.

**Decision:** Use the Kanban as the active procurement pipeline with columns for decide, source and price, ready, ordered, received, later phase and complete. Cards may mirror dated order tasks but carry no dates. Add a budget summary and supplier order batches to [[Shopping List]].

**Consequences:** Procurement work is visible and prioritised, while dates remain only in `Tasks/`. The no-duplication rule in [[Project Plan]] and `AGENTS.md` is relaxed to allow one card per order task. The budget stays TBC until the source-and-price cards are complete, so the total is not yet reliable.

## 2026-11-02 — Autocraft 75 L / 45 L underslung tank set (topfill)

**Context:** The underslung fresh and grey tanks needed to be selected and priced. Autocraft offers a matched Ducato set with mounting brackets, a topfill fresh kit, a waste kit and an optional Shurflo pump. The vehicle is a 2019 Ducato with a WAS ambulance box body.

**Options considered:**
- Autocraft complete set, topfill, with pump and filter.
- Autocraft complete set, backfill, with pump and filter; requires an external pressure source.
- Autocraft set without pump; specify the pump separately.
- Individual Fiamma or other tanks.

**Decision:** Select the Autocraft 75 L fresh / 45 L grey set in topfill configuration with the Shurflo Trail King 7 pump and filter, **£373.40**, for planning. Topfill was chosen over backfill because it can be filled by gravity from a hose, funnel or jug. The cap colour is TBC. Do not order until the 2019/WAS fitment is confirmed. The fill point will be decided after measuring, and the grey-tank inlet will be confirmed with Autocraft.

**Consequences:** The official set listing states 2006–2017, while the individual 75 L listing states 2006–2019 L2/L3/L4; the WAS chassis must be checked before ordering. The dimensions calculate to 67.5 L fresh and 51 L grey, so usable capacity needs confirmation. The supplied 3/4" grey inlet may be too small for a 40 mm sink waste; investigate a drilled 40 mm inlet. A fresh drain tap, level sensors, drinking-water filter, heat shield and thermal heating mats are additional. Payload and axle loads must be checked with both tanks full. See [[Water]].

**Superseded 2026-11-04:** The matched 75/45 set was replaced by separate 75 L fresh and 60 L waste tanks after measuring the underside; see the decision below.

## 2026-11-02 — Shower cladding: black 2 mm PVC on plywood backing

**Context:** The shower walls need a waterproof, wipe-clean surface. The previous design assumed 6 mm solid PVC or compact laminate panels; the selected product is a 2 mm black PVC hygienic cladding sheet, which needs a plywood backing to provide stiffness and impact resistance.

**Options considered:**
- 6 mm solid PVC or compact laminate panels.
- 2 mm black PVC hygienic cladding on a plywood backing.
- Other waterproof wall systems.

**Decision:** Use **2 mm black PVC hygienic cladding** from Hygienic Plastic Supplies, SKU `B2104`, 3050 × 1220 × 2 mm, at **£49.99 + VAT per sheet**, on a plywood backing. Three walls are planned at approximately **1970 × 700 mm**, requiring **three sheets minimum** with substantial offcut. The plywood thickness, grade and fixing method remain TBC.

**Consequences:** The supplier states the cladding is Class 0 fire rated to EN 13501-1 B-s3,d0, solid PVC (not foam-filled) with a satin finish; verify the certificate and keep the cladding clear of the diesel-heater outlet. The 2 mm sheet needs continuous plywood support, sealed edges and a suitable adhesive/fixing detail. Three 3050 × 1220 mm sheets provide 11.16 m² for about 4.14 m² of wall, so expect significant offcut; confirm the final dimensions and consider cut-to-size. The product was out of stock at the time of research. See [[Shower]].

## 2026-11-02 — Boxio XL MAX+ separating toilet and no dedicated toilet vent

**Context:** A portable urine-diverting toilet is needed for the shower compartment. It must avoid a black-water tank, be easy to move for showering and provide enough capacity for two people between emptying. The previous design assumed a fixed lower-back-wall vent with a removable toilet connection.

**Options considered:**
- Boxio TOILET XL MAX+ complete set with Solo Up base.
- Other separating toilets such as Nature's Head, Separett, Kildwick or Air Head.
- Keep the fixed lower-back-wall toilet vent and add a docking hood or hose.
- Rely on the toilet's own odour control and the compartment extractor, with no dedicated toilet vent.

**Decision:** Select the **BOXIO TOILET XL MAX+ complete set** at **£249.99** (regular £269.99, VAT included). Use the included **Solo Up** base, giving a **45 cm** seat height and storage underneath. The toilet alone is 33 cm high. Capacity is **7 L urine / 8 L solids**, weight **5.8 kg**, footprint **40 × 30 cm** and maximum load **150 kg**. Remove the dedicated toilet vent: the Boxio has no integrated fan or direct vent port. Odour control relies on the separator, plug/odour trap, hemp litter and the shower/room extractor.

**Consequences:** No lower-back-wall penetration, vent hose, docking hood, carbon filter or 12 V toilet fan is required. The toilet uses no water, chemicals or power. Urine can be emptied into a normal toilet; solids go into general waste in a Bio-Bag, subject to local rules. The 45 cm height, use/storage positions and retention for travel still need checking in [[T02 Design toilet use, storage and retention]]. The product page showed both SOLD OUT and in stock with 4–6 working days delivery, so availability must be confirmed before ordering. The linked manual covers the standard TOILET MAX and lists 5 L / 5.7 L; confirm the XL's 7 L / 8 L figures with Boxio. See [[Toilet]] and [[Shopping List]].

## 2026-11-04 — Separate 75 L fresh and 60 L waste tanks, internal topfill

**Context:** The underside was measured to confirm the tank envelopes. There is enough space for the 75 L fresh tank. The waste-tank position is awkward: an electrical cable can be removed to free space, but a 400 mm-wide tank still fouls brake-cable and other protrusions. The previous matched set used a 45 L tank measuring 400 × 500 × 255 mm.

**Options considered:**
- Keep the Autocraft 75/45 set and accept the 400 mm waste-tank width.
- Remove the cable and force the 45 L tank into the space, accepting poor clearance.
- Use a narrower 60 L tank and adapt its mounting brackets.
- Relocate the waste tank or commission a custom tank.

**Decision:** Buy the tanks separately: the **Autocraft 75 L fresh kit** with topfill black cap, universal brackets and Shurflo pump/filter, SKU `75KT-TFB-PU-UB-WOO`, **£252.40**; and the **Autocraft 60 L Sprinter/Crafter tank** with its bracket set, no fresh kit and no pump, SKU `60SPCRKT-00-00-60MB-WOO`, **£205.00**. The 60 L tank is **350 × 800 × 250 mm**, so its width should clear the brake-cable protrusions once the cable is removed and confirmed to be no longer required. Use it as the waste tank. Combined price is **£457.40** before waste fittings.

The fresh tank keeps a **topfill** design. The fill point moves **inside**, to a black lockable cap in the rear upstand directly behind the kitchen sink. Ten-litre bottles rest on the counter and are poured over the sink, so spills drain to the grey tank. The 40 mm fill hose must fall continuously to the tank. The waste tank is drilled for a 40 mm sink inlet, a 3/4" Loopz inlet, a 3/8" breather and a 3/4" drain tap.

**Consequences:** The tanks cost £84 more than the previous set before the separately sourced waste fittings, but the waste tank is 15 L larger and should fit the measured space. The Sprinter/Crafter brackets must be adapted or redrilled for the Ducato/WAS chassis and checked for strength. The service-hatch orientation and drill positions need Autocraft confirmation. The 60 L tank is 800 mm long, so length and cleaning access still need checking. The internal filler removes the need for an external fill point but introduces a 40 mm hose route, a breather/overflow path that must terminate outside, and a spill path into the sink. The 75 L nominal capacity still conflicts with its 67.5 L external envelope. See [[Water]] and [[Shopping List]].

## 2026-11-04 — JA Seals Multi Seal for the Loopz base perimeter

**Context:** The Loopz base must be sealed to the shower walls while remaining removable for servicing. The previous design called for a generic waterproof rubber trim, but no product was selected. The proposed product is the JA Seals Multi Seal 2.5 m, a garage-door compression seal for gaps up to 25 mm supplied with double-sided tape and self-tapping screws.

**Options considered:**
- JA Seals Multi Seal as the primary mechanical compression seal, fixed to the walls only.
- Neutral-cure silicone or a butyl/MS-polymer seal as the primary barrier, with the Multi Seal as a removable cover trim.
- A shower-specific seal such as Sealux Aquastrap EPDM/butyl.

**Decision:** Use one **JA Seals Multi Seal 2.5 m**, **£24 inc VAT**, as the **primary mechanical compression seal** around the three walls. Fix it to the walls only, through the PVC cladding into the plywood backing and, where possible, the battens, using the supplied self-tapping screws; use the tape for location only. Do not screw or bond it to the Loopz base, so the unit can still slide out. Seal screw heads and corner joints with neutral-cure silicone.

**Consequences:** The trim is a garage-door product, not a waterproof sealant. Its material, mould resistance and suitability for intermittent wet use are not stated and must be confirmed with JA Seals before ordering. The base-to-wall gap must be measured and fall within the trim's rated gap of up to 25 mm with slight compression; the 2.5 m length covers the three 700 mm walls but leaves only about 0.4 m for corners. Dry-fit the base and trim, test removal, and prove the joint in [[S09 Shower watertightness test]]. If it fails, revert to a neutral-cure silicone/MS-polymer primary seal with a removable trim, or a shower-specific product. See [[Shower]] and [[Shopping List]].

## Related

- [[Dashboard]]
- [[Project Plan]]
- [[Kanban]]
- [[Shopping List]]
- [[Kitchen, Shower & Toilet]]
- [[Shower]]
- [[Toilet]]
- [[Water]]
- [[Ventilation & Moisture]]
- [[Diesel Heater]]
- [[Electrics Overview]]
