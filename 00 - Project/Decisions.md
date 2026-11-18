---
tags: [project, decisions]
status: active
updated: 2026-11-18
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

**Superseded (partially) 2026-11-16:** The humidity sensor/timer requirement was relaxed to manual control. The MaxxFan Dome Plus `00-03810B` is shortlisted as a direct roof-mounted extractor/light; see the entry below.

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

## 2026-11-05 — Record installed 314 Ah LiFePO4 leisure bank

**Context:** The documentation still described the leisure bank as undecided and compared AGM candidates. A 12 V LiFePO4 battery is now installed, and the DC-DC choice depends on its charge profile and low-temperature behaviour.

**Options considered:**
- Keep the AGM research as the current design.
- Record the installed Eco-Worthy battery as the leisure bank.
- Replace it with a different chemistry or capacity.

**Decision:** Record the installed **Eco-Worthy EnergyTrek 12 V 314 Ah LiFePO4 battery** as the leisure bank. Its published figures are 12.8 V, 314 Ah, 4,019 Wh, a 200 A BMS, 200 A maximum charge and discharge, 0–55 °C charging, low-temperature charging protection below approximately -7 °C, Bluetooth monitoring, SOC LEDs, M8 terminals, 414 × 215 × 260 mm and 27.4 kg. The product URL says 300 Ah, but the product page and specification table state 314 Ah; the listing discrepancy is recorded rather than resolved by assumption.

**Consequences:** The MPPT, Pro Charge Ultra and DC-DC must all use a LiFePO4 profile. The 60 A MPPT remains the bulk charger. The old lead-acid auxiliary system and split-charge relays have been removed, so the DC-DC is the only alternator-to-leisure path. The BB1225 25 A DC-DC is a maintenance and trickle source at about 0.080C for this bank. Its 0 °C low-temperature trip is more conservative than the battery BMS cutoff and is acceptable. The Xantrex 2000 W inverter's 3000 W surge is about 278 A at 12 V, above the battery's 240 A/10 s peak, so the inverter surge and 1.5 kW appliance limit must be tested and recorded in [[E02 Complete load schedule and cable-fuse sizing]]. The AGM component pages remain as research history. See [[Eco-Worthy EnergyTrek 12V 314Ah LiFePO4 Battery]], [[Electrics Overview]] and [[Shopping List]].

## 2026-11-05 — Replace the installed 60 A DC-DC with a 15 A bidirectional BaBy (superseded 2026-11-13)

**Superseded 2026-11-13:** the BB1215 was not ordered; see the BB1225 decision below.

**Context:** A Voltanic 60 A DC-DC is installed and connects the alternator to the LiFePO4 leisure bank. The vehicle spends most of its time stationary, the 800 W solar array is the primary charge source, and the 60 A alternator load, cable size and fusing are unnecessary for the actual travel pattern. The installed unit cannot maintain the starter battery from surplus leisure-bank charge when parked. Separate trickle chargers were considered but add cost and cabling.

**Options considered:**
- Keep the installed Voltanic 60 A DC-DC.
- Fit the Sterling Power BaBy 15 A bidirectional DC-DC and maintainer.
- Fit a Sterling Saturn 25 A or 40 A bidirectional unit.
- Keep the 60 A unit and add a separate trickle or echo charger.

**Decision:** Replace the installed Voltanic 60 A DC-DC with the **Sterling Power BaBy 15 A bidirectional DC-DC** (BB1215, SKU `BABY`), **£149 inc VAT**. Remove the 60 A unit and sell or retain it; do not run both. Use the BaBy's ignition-feed mode, a direct common negative, 4–6 mm² cable and 25 A fuses at both batteries. Mount it in the confirmed dry location and fit the included temperature sensor to the leisure battery negative.

**Consequences:** Alternator charging drops to about 15 A nominal, or 19 A maximum per the manual. On the 314 Ah bank this is about 0.048C: roughly 10.5 hours for 50% depth of discharge and 16.7 hours for 80%. The BaBy is therefore a maintenance and trickle source, not the bulk charger; solar remains primary. Reverse charging maintains the starter battery when the leisure bank is above 13.5 V, so a full LiFePO4 bank at rest may not maintain it overnight. Use ignition-feed mode to stop the Pro Charge Ultra's starter output from triggering forward charging. Connect the BaBy output and reverse-charge path to the battery busbar or main fuse side. Replace the 60 A fuses with 25 A fuses and check whether the existing lugs fit the BaBy's 6.1 mm terminals. Confirm the 15 A versus 19 A rating, the 5-year versus 2-year warranty and the reverse-charge current with Sterling. See [[Sterling Power BB1225 25A DC-DC Charger]], [[Eco-Worthy EnergyTrek 12V 314Ah LiFePO4 Battery]], [[E05 Install charger, inverter, consumer unit and circuits]] and [[Shopping List]].

## 2026-11-13 — Use the Sterling BB1225 25 A DC-DC instead of the BB1215

**Context:** The BB1215 BaBy was selected on 2026-11-05 but not ordered. The supplied BB1225 manual covers a 25 A unit (26 A input) with reverse charging and jump-start assist. It is closer to the capacity of the installed 60 A unit than the BB1215 while still simplifying the alternator, cable and fuse requirements, and it retains starter battery maintenance from surplus leisure charge.

**Options considered:**
- Keep the BB1215 selection.
- Fit the Sterling Power BB1225 25 A battery-to-battery charger.
- Keep the installed Voltanic 60 A DC-DC.

**Decision:** Use the **Sterling Power BB1225 25 A 12 V–12 V battery-to-battery charger** (BB1225), **£190.80 inc VAT** on the Sterling listing. Remove the installed Voltanic 60 A unit and sell or retain it; do not run both. Use ignition-feed mode, a direct common negative, 6 mm² / 10 AWG cable and about 30 A fuses at both batteries. Mount it in the confirmed dry location and fit the included temperature sensor to the leisure battery negative.

**Consequences:** At 25 A on the 314 Ah bank the charge rate is about 0.080C: roughly 6.3 hours for 50% depth of discharge and 10 hours for 80%. The BB1225 is therefore a maintenance and trickle source, not the bulk charger; solar remains primary. Select the Lithium I profile, which uses 14.4 V absorption and lists 13.8 V float, but the manual also states that lithium profiles use live output voltage, so confirm the float behaviour. The 0 °C lithium trip is conservative and matches the battery's stated charging range. Reverse charging maintains the starter battery at about 13.4 V and engages at 13.5 V on lithium, so a full LiFePO4 bank at rest may not maintain it overnight. Use ignition-feed mode to stop the Pro Charge Ultra's starter output from triggering forward charging. Replace the 60 A fuses with about 30 A fuses; the manual's connector page says 30 A while some mode diagrams show 50 A. The manual does not state the terminal diameter, so check whether the existing lugs fit before reusing the heavy cable. The supplied 2023 manual states a 2-year warranty while current Sterling Saturn listings state 5 years, so confirm with the supplier. See [[Sterling Power BB1225 25A DC-DC Charger]], [[Eco-Worthy EnergyTrek 12V 314Ah LiFePO4 Battery]], [[E05 Install charger, inverter, consumer unit and circuits]] and [[Shopping List]].

## 2026-11-14 — Sterling Power F50 50 L fridge/freezer for the kitchen

**Context:** The kitchen documentation assumed a roughly 30 L drawer-style 12/24 V compressor fridge, but no model had been selected. The kitchen needs a larger cold-storage volume and a freezer compartment, and a conventional under-worktop unit fits the planned galley layout.

**Options considered:**
- Sterling Power / AMPS 20.7 L drawer fridge.
- Sterling Power / AMPS F50 conventional 50 L fridge/freezer.
- Sterling Power / AMPS conventional 90 L fridge.
- Continue researching other 12/24 V compressor fridges.

**Decision:** Select the **Sterling Power / AMPS F50 50 L conventional fridge/freezer**, SKU `F50`, at **£238.80 inc VAT**, as the kitchen fridge. It is a 12/24 V unit with an LG compressor, rated at **60 W** (about **5 A at 12 V** or **3 A at 24 V**), measuring **380 × 479 × 532 mm**. It has separate fridge (**0–8 °C**) and freezer (**-12 to -20 °C**) compartments, a digital display and AMPS app control, internal lighting, a reversible door hinge, E-mark E24 certification and a three-year warranty.

**Consequences:** The kitchen layout changes from a drawer fridge to a conventional under-worktop unit, so the carcass, door swing and worktop clearance must accommodate the 532 mm height and 479 mm depth. Front and rear ventilation clearances must be taken from the F50 instructions; the manual is stored in the vault as `Sterling Power F50 Fridge Instructions.pdf` and linked from [[Kitchen]]. The 60 W load is added to the DC load schedule, with the duty cycle still to be measured. The £238.80 price raises the priced shopping-list total to £2,103.95 before the bin selection below. Stock and lead time are not yet confirmed, so the fridge remains `shortlisted` until ordered. The 24 V rating is not used on this 12 V system. See [[Kitchen]] and [[Shopping List]].

## 2026-11-14 — IKEA HÅLLBAR 10 L bins for waste and recycling

**Context:** The kitchen needs separate lidded bins for general waste and recycling that fit the compact galley and can be secured while travelling. The previous BOM left both bins unspecified.

**Options considered:**
- Two IKEA HÅLLBAR bins in the 3 L, 10 L, 22 L or 35 L sizes.
- Generic freestanding bins.
- A built-in cabinet bin system.

**Decision:** Use **two IKEA HÅLLBAR 10 L bins with lids**, light grey, article `803.980.58`, at **£7 each (£14 total)**. Each bin has a removable lid, bag-retaining ring, folding handle and sorting sticker. The upper outer dimensions are **263 × 212 mm**, the lower outer dimensions are **201 × 147 mm**, and the height is **326 mm**. The bins are stackable and can be freestanding or integrated into a cabinet or drawer.

**Consequences:** The 326 mm height and tapered footprint must be checked against the planned under-sink or cabinet space, and the bins need a travel restraint because the lids are removable rather than latched. The bucket, lid, hinge and ring are polypropylene with at least 50% recycled content; the handle is reinforced polyamide with at least 20% recycled content. They remain `shortlisted` until ordered. The £14 raises the priced shopping-list total to £2,117.95. See [[Kitchen]] and [[Shopping List]].

## 2026-11-16 — MaxxFan Dome Plus for shower extraction and lighting

**Context:** The shower needs a new extractor, and the previous design required a humidity sensor or timer, a separate roof vent, a duct, a cowl and a separate IP65 light. The preferred solution is a compact combined light and extractor. The shower ceiling is a dropped ceiling of about 5.6 mm PVC/ply, 38 mm battens and a 50 mm aluminium sandwich roof, giving about 93.6 mm from the shower ceiling to the exterior roof. The MaxxFan Dome Plus `00-03810B` is a 6¼" cutout, 12 V exhaust-only fan with an integrated LED ring and a manual lift lid; the manual is P/N `11-90056`.

**Options considered:**
- MaxxFan Dome Plus `00-03810B` as a combined direct-mounted extractor and light.
- A ducted 12 V extractor with a humidity sensor/timer, separate roof vent, cowl and IP65 light.
- Another compact roof or sidewall fan.

**Decision:** Shortlist the **MaxxFan Dome Plus `00-03810B`** (black, integrated LED) at approximately **£104–£119** as the preferred shower extractor/light. Use the integrated LED as the shower light and remove the separate IP65 light. Relax the humidity sensor/timer requirement to manual control: the fan is single-speed with manual on/off and a manual lift lid. Use a direct roof mount through the shower ceiling, with no separate duct, cowl or backdraught shutter. The nominal 93.6 mm build-up needs the extension sleeve trimmed to about **117 mm** (93.6 mm plus 23.8 mm for the LED garnish ring). Seal the flange with butyl tape and a compatible self-levelling lap sealant, and seal the interior garnish ring with neutral-cure silicone.

**Consequences:** The installation is simpler than the ducted design and provides ventilation and lighting in one fitting. However, the fan must be switched on manually and the lid opened before use; there is no humidity sensor, timer, thermostat or wall control. The fan draws about 2 A / 24 W and needs a 5 A circuit fuse. The design depends on a 159 mm roof penetration clear of the solar array, roof ribs and existing penetrations. Before ordering, confirm the sleeve and guard contents, the LED IP rating, the actual current and airflow, roof-skin screw purchase, sealant compatibility, headroom below the handle and the passive inlet. If the checks fail, revert to a ducted humidity-sensing extractor and a separate IP65 light. See [[MaxxFan Dome Plus]], [[Shower]] and [[Shopping List]].

## 2026-11-16 — Nofer retractable clotheslines for shower drying

**Context:** The shower compartment is also the drying room, but it had no hanging space. Three retractable lines are wanted at even spacing to dry clothes. The walls are 2 mm PVC on plywood over 3×2 CLS battens, so the fixings must reach the battens or added noggins.

**Options considered:**
- Three Nofer CLASSIC 09058.B retractable clotheslines.
- Fixed stainless rails or hooks.
- A freestanding drying rack.

**Decision:** Use **3 × Nofer CLASSIC 09058.B retractable clotheslines**, AISI 304 polished stainless steel, Ø90 × 55 mm, 2.2 m nylon cord, at **£29.99 inc VAT each (£89.97 total)**. Mount them between the two opposite walls across the ~700 mm shower width, at even spacing. Confirm whether the lines are side-by-side at one height or stacked at three heights. Fix through the 2 mm PVC and plywood into the battens; add noggins behind the ply wherever the fixing points do not align with a batten. Use stainless screws and sealing washers and seal every penetration with neutral-cure silicone.

**Consequences:** The priced shopping-list total rises to **£2,207.92** before the shortlisted MaxxFan. The installation needs three case fixings and three opposite supports, all on battens or noggins. The cases protrude 55 mm, so check clearance to the shower head, Loopz controls, heater diffuser, MaxxFan and toilet, and set the height to give clothes useful drop. Confirm that the opposite support is included; if not, source a stainless support. AISI 304 is suitable for fresh water but needs regular stainless-steel cleaner and no chloride/bleach cleaners. The nylon cord may stretch, so check the fixings and tension with wet clothes. See [[Shower]] and [[Shopping List]].

## 2026-11-18 — VEVOR 40 cm top-mount stainless sink

**Context:** The kitchen BOM had a 24 × 18 × 9 in (about 610 mm wide) Garvee single-bowl sink as the only shortlisted model, with no recorded price, stock or installation details. A narrower sink suits the compact galley and leaves more worktop, so a priced 400 mm two-model comparison was made.

**Options considered:**
- Garvee 24 × 18 × 9 in stainless single bowl, unpriced.
- VEVOR 40 cm top-mount 304 stainless single bowl (`QRSSCTSPDC40TOW17V0`).
- AliExpress single-bowl alternative.
- Continue researching other sinks.

**Decision:** Select the **VEVOR 40 cm top-mount single-bowl sink**, SKU `QRSSCTSPDC40TOW17V0`, model `T404519RS0`, at **£68.90**. It is 304 stainless steel, **400 × 450 × 190 mm** externally, with a **370 × 420 mm** internal bowl, a **3 mm** rim and a weight of **4.5 kg**. The drain hole is offset, the base has a quick-drain profile, and the supplied drain kit has two side pipe inlets. Sound-deadening pads and an anti-condensation base coat are fitted. The rim has tap and soap-dispenser holes. It is a drop-in top mount, sealed to the worktop with neutral-cure silicone.

**Consequences:** The sink is 210 mm narrower than the Garvee candidate, so the worktop layout and carcass can be re-planned around a smaller opening. The listing gives a 370 × 420 mm cutout, identical to the internal bowl size, so the supplied saw template must be checked before the worktop is cut. A review reports no fixing clips in the box, so the contents need checking on receipt. The product page shows the variant as both out of stock and in stock, so availability must be confirmed before ordering. Confirm the drain offset direction suits the trap and grey-tank route, the tap-hole size suits the chosen cold tap, and whether the second hole can take the optional drinking-water filter tap. The 40 mm sink inlet to the 60 L grey tank and the fill-point spill path are unchanged. The £68.90 price raises the priced shopping-list total to **£2,276.82**. The sink remains `shortlisted` until ordered. See [[Kitchen]] and [[Shopping List]].

## 2026-11-18 — Sterling IH1L 1000 W built-in induction hob

**Context:** The kitchen cooking section named the Sterling IH2L 1.5 kW built-in hob, but no price or installation detail had been recorded. The inverter is 2000 W and the kettle remains a 1.5 kW load, so a lower-power hob reduces the worst-case 230 V load and leaves more headroom. A compact circular built-in hob also suits the small galley worktop.

**Options considered:**
- Sterling IH2L, 1000 W rectangular built-in, 250 × 210 mm.
- Sterling IH1L, 1000 W circular built-in with a wired remote.
- Sterling IH1 or IHP portable hob.
- Another low-power induction hob.

**Decision:** Select the **Sterling IH1L** built-in single induction hob at **£67.20 inc VAT**. It is 230 V AC, 50 Hz, with a **1000 W** maximum and eight power settings from 200 W to 1000 W. The A-grade black crystal plate is **Ø195 mm** over a **Ø180 mm** body that sits about **65 mm** below the worktop. The worktop cutout is **186 mm**, with **100 mm** of clear worktop around it. Controls are on a supplied wired remote, **135 × 61 × 15 mm**. The unit has a 1.5 m AC cable with a Schuko plug and UK adaptor, eight temperature settings from 80 °C to 240 °C, overheat/voltage/current protection, and stops after 1 minute without a pan or 1 hour without operation.

**Consequences:** The previous kitchen page listed the IH2L as 1.5 kW; the current Sterling listing gives the IH2 as 2000 W and the IH2L as 1000 W, so the old label was wrong and is corrected here. The 1000 W maximum is below the existing 1.5 kW appliance limit, so the hob no longer sits close to the inverter's continuous rating; the kettle is now the larger load and the two must still not run together. The IH1L manual recommends a 1000 W inverter for P1–P6 and 1500 W for P7–P8, so confirm the top two settings on the installed 2000 W inverter. A dedicated 13 A outlet is required; 10 A or lower plugs and multiplugs are not permitted. The circular cutout, 100 mm clear worktop and 65 mm body depth must be set out before the worktop is cut, and the manual's 20 mm worktop, 50 mm and 125 mm details need confirming against the chosen worktop. The remote needs a dry, splash-free mounting position and cable route. Pans must be ferrous with a 12–20 cm base. Keep 12 cm from walls and the fan clear, and do not exceed about 11 kg on the plate. The product may take a few days to ship. The separate `Manual_IH1` PDF supplied in Downloads covers the 1500 W IH1, not the IH1L, so the correct IH1L manual was downloaded and both are stored in `Attachments/`. The £67.20 price raises the priced shopping-list total to **£2,344.02**. The hob remains `shortlisted` until ordered. See [[Kitchen]] and [[Shopping List]].

## Related

- [[Dashboard]]
- [[Project Plan]]
- [[Kanban]]
- [[Shopping List]]
- [[Kitchen, Shower & Toilet]]
- [[Kitchen]]
- [[Shower]]
- [[MaxxFan Dome Plus]]
- [[Toilet]]
- [[Water]]
- [[Ventilation & Moisture]]
- [[Diesel Heater]]
- [[Electrics Overview]]
- [[Eco-Worthy EnergyTrek 12V 314Ah LiFePO4 Battery]]
- [[Sterling Power BB1225 25A DC-DC Charger]]
