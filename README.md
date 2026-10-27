# The Ugly Duckling

The Ugly Duckling is an ambulance being converted into a self-sustaining, off-grid liveaboard. This repository documents the planned kitchen, shower and toilet area, including a recirculating shower, composting toilet, underslung water tanks and an 800 W solar array.

## Overview

The project is a full-time liveaboard conversion rather than a weekend camper. The ambulance body, roof and existing services provide the platform; the interior is being designed around limited space, finite water and energy, and winter conditions. The current phase covers the kitchen, shower and toilet, together with the water, waste, ventilation and electrical systems that support them.

The repository is the working design record. It holds requirements, bills of materials, supplier links, open questions, a decision log and a Kanban board, alongside FreeCAD models, CNC toolpaths and a KiCad wiring project. It deliberately distinguishes installed equipment from shortlisted or researched equipment: the solar array and diesel heater are installed and the table has been modelled and cut, while most of the wet-area systems remain at design stage.

The work is documentation-led. Significant choices are recorded with their context and consequences before fabrication, so that dimensions, power budgets and safety constraints can be checked as the build progresses.

## Features

The project combines an existing vehicle platform with a documented design package. The lists below separate what is installed from what has been designed or shortlisted.

### Installed and completed

- **800 W solar array:** Four 200 W black monocrystalline panels in a 2-series, 2-parallel configuration, with a 60 A MPPT controller and black anodised aluminium mounting extrusion.
- **Diesel air heating:** An Eberspächer Airtronic D4 12 V Mk1 with an 802 digital controller is already mounted.
- **CNC-cut table:** A FreeCAD table design has been toolpathed and cut, with the legs and stiffener fitted.
- **Design documentation:** A linked Obsidian vault with a dashboard, decision log, shopping list, bill-of-materials tables and a Kanban board.

### Designed or shortlisted

- **Recirculating shower:** A Hamwells Loopz Plus with a semi-permanent base, battened walls and removable waterproof trim. The unit has been shortlisted, not purchased.
- **Composting toilet:** A portable separating toilet that can be moved out of the shower compartment, with a fixed vent connection at the lower back wall. The model is not yet selected.
- **Water storage:** Underslung 75 L fresh and 45 L grey tanks, with insulation and heating still to be resolved.
- **Cold-water kitchen:** A stainless sink, 1.5 kW induction hob, 30 L drawer fridge and a 1.5 kW maximum kettle, all limited by the inverter and battery budget.
- **Electrical system:** A 12 V leisure architecture designed around a Xantrex PROwatt SW 2000i inverter, Sterling Pro Charge Ultra 60 A shore charger, Victron BatteryProtect BP-65 and a leisure battery bank whose final chemistry and capacity are still open.
- **Drying branch:** An 89 mm duct from the diesel heater to the shower, switched by a changeover damper so the same heater can warm the living space or dry the wet area.
- **Shower ventilation:** A new 12 V roof extractor with humidity sensing or timer control and a new roof vent; the existing black roof extractor is not reused.

## Technologies

- **Obsidian and Markdown:** The documentation is an Obsidian vault with frontmatter, wikilinks and a Kanban plugin. The README uses standard Markdown links so that it renders correctly on GitHub.
- **FreeCAD:** Parametric models for the van, bed, kitchen and shower, roof, sofa, table and electrical layout, with STEP, STL and DXF exports.
- **KiCad:** Schematic, PCB layout, project and symbol-library files for the electrical wiring guide.
- **CNC routing and G-code:** Toolpaths for the table legs, stiffener and table.
- **12 V DC and 230 V AC system design:** Solar charging, shore charging, battery protection, inverter loads, fusing and distribution.
- **Referenced hardware:** Hamwells, Eberspächer, Xantrex, Sterling Power, Victron Energy, Fullriver, Lucas and Voltanic equipment, recorded with specifications and source links in the relevant pages.

## Technical Details

### Wet-area concept

The shower compartment is the centre of the current phase and is designed to double as a drying room. The Loopz Plus base forms the compartment floor, with a 1° fall towards the drain and a threshold or ramp for the 10 cm base height. The walls are designed around 3×2 CLS battens at 300 mm centres, fixed to the ambulance's structural ribs with rivnuts, plus nuts or structural rivets. Noggins support panel edges, joints, curtain rails and fixtures.

The wall surface is to be 6 mm solid PVC or compact laminate, mechanically fixed with stainless screws and sealing washers. Panel joints use H-trims, and penetrations and joints are sealed with neutral-cure silicone. Insulation sits behind the panels to reduce condensation, and a heat shield is planned near the diesel-heater outlet. The panel product and its fire rating have not been finalised.

The Loopz base is designed to slide into place and be sealed around its perimeter with a removable rubber trim. A removable bead or clamp is intended to retain the base without relying on permanent silicone, so the unit can still be taken out for servicing or storage. The composting toilet is portable and moves out of the compartment when the shower is in use; its fixed vent is planned for the lower section of the back wall.

### Recirculating shower

The Loopz Plus is a portable recirculating shower with a 6 L reservoir, three-stage filtration including UV-C treatment, and a reusable 325-mesh stainless microfilter. Its documentation is inconsistent: power is quoted as 27 W, 45 W or 60 W, weight as 7 kg or 10 kg, and maximum water temperature as 45 °C or 60 °C. The build therefore uses a conservative design envelope of 60 W / 5 A, 10 kg unit weight plus 6 kg of water, a 45 °C maximum water temperature and a 100 kg maximum deck load until Hamwells confirms otherwise.

The unit does not heat water. It draws from a 12 V socket outside the cubicle, protected by a 7.5–10 A fuse, with a sealed cable entry and drip loop. Filling is done with a jug, funnel or short food-grade hose from the kitchen tap. The reservoir drains after each shower to the grey tank through a HepvO or P-trap, a removable coupling and a cap. A continuous fall is required; a small sump pump is the fallback if the final tank position cannot provide one.

### Water and waste

The design stores fresh water in a 75 L underslung tank and delivers it by a 12 V diaphragm pump through an accumulator and a sediment and carbon filter to the cold kitchen tap. Grey water from the sink and the Loopz drain is to be collected in a 45 L underslung tank with a vent, level sensing and a drain valve. The kitchen drain is to include a trap and an air-admittance valve.

There is no hot-water system, no calorifier and no black-water tank. Hot water comes from a kettle, and the kitchen is cold-water only. If preheated water is used for the shower, it must be mixed down to 45 °C or below before filling the Loopz. The planned composting toilet separates urine into a portable container and solids into a removable container with cover material. Because the tanks and pipework are underslung, insulation, a heating method, low-point drains and a winterising procedure are required; candidate measures include thermostatically controlled heater pads and insulated pipework, and the final choice and power budget remain open.

### Electrical architecture

The installed solar array is wired 2S2P and feeds a 60 A MPPT controller. A Sterling Pro Charge Ultra 12 V / 60 A charger is planned for shore power, while alternator or DC-DC charging remains an open question. The planned 12 V bank supplies DC loads through a fuse panel and a Victron BatteryProtect BP-65, with the inverter bypassing the BatteryProtect on its own fuse. The Xantrex PROwatt SW 2000i provides 230 V pure-sine power through an RCD/RCBO-protected consumer unit.

The induction hob and kettle are limited to 1.5 kW each and must not run together: either load is already close to the inverter's continuous rating, and both together would overload it. The final battery chemistry and capacity are unresolved. The component notes compare the Fullriver DC115-12 and Lucas LSLC125-12 AGM batteries, warn against mixing different models in one permanent parallel bank, and set out the case for a matched pair or a LiFePO4 bank.

### Heating and ventilation

The Eberspächer Airtronic D4 is rated at 4 kW nominal and is controlled by an 802 digital controller. Its 89 mm hot-air outlet is intended to feed either the living space or the shower through a changeover damper, while the 76 mm return draws from the dry living space rather than the shower. The 24 mm combustion-air intake and exhaust terminate outside. The main heater outlet must remain open so the unit is never dead-ended, and a CO alarm, high-temperature ducting, a closable diffuser and a heat shield are required.

A new 12 V shower extractor with a humidity sensor or timer will duct to a new roof vent with a cowl, insect mesh and backdraught shutter. The old black roof extractor is not reused. A passive air inlet is needed so the extractor can move air, and the kitchen and toilet require their own extraction. The drying sequence is to squeegee the surfaces, extract for 10–15 minutes, direct heater air into the compartment with ventilation open, then finish with a short extract to remove the moist air.

### CAD, CNC and electrical design

FreeCAD holds the master models for the van, bed, bed mount, kitchen and shower, roof, sofa, table and electrical layout. Exports include STL, STEP, DXF and SVG files for the bed mount and other parts. G-code exists for the table legs, stiffener and table, and the legs and stiffener have been cut and fitted. The KiCad project contains the wiring schematic, PCB layout, project files and a custom symbol library.

These are working models rather than as-built records. Dimensions, mounting points and cable routes should be checked against the vehicle before cutting or drilling.

### Documentation model

The vault is organised by area and system. Every content page opens with one level-one heading, then uses `##` sections for requirements, the current design, open questions, bills of materials and related pages. Frontmatter records tags, status and the last update date. Bills of materials use a consistent table with item, quantity, specification, supplier, price, status and notes. Status values are `idea`, `research`, `shortlisted`, `ordered`, `received`, `installed` and `cancelled`.

The [Dashboard](00%20-%20Project/Dashboard.md) is the entry point. The [Kanban](00%20-%20Project/Kanban.md) board holds the next physical and research tasks, the [Decisions](00%20-%20Project/Decisions.md) log records why choices were made, and the [Shopping List](00%20-%20Project/Shopping%20List.md) consolidates purchases without duplicating the detailed specifications.

## Challenges and Solutions

1. **Conflicting Loopz specifications.** Public material and the safety sheet disagree on power, weight, maximum water temperature and connector rating. These figures determine cable size, fusing, floor loading and safe operating temperature. The design adopts the conservative values and treats manufacturer confirmation as an outstanding action. The result is a wiring and floor design that remains valid even if the lower figures prove correct.

2. **A shower and toilet sharing one small compartment.** A fixed toilet would obstruct showering, while a completely portable toilet still needs odour control. The chosen approach keeps the composting toilet portable and provides a fixed vent at the lower back wall with a removable hose or docking connection. This avoids a black-water tank, but the vent detail depends on the toilet model, which is not yet selected.

3. **No hot water and a shower that does not heat it.** A calorifier would add plumbing, weight, freeze risk and cost. The project instead uses a kettle for hot water and keeps the kitchen cold-water only. Shower water is either ambient or preheated and mixed down to 45 °C or below. The water system is simpler, but shower temperature depends on careful preheating.

4. **A 2 kW inverter against an undecided battery bank.** The inverter can deliver 2 kW continuously, but a small AGM bank would suffer voltage sag and rapid depletion under that load. The design caps the hob and kettle at 1.5 kW each and prohibits running them together, while the component notes compare a matched AGM pair with LiFePO4. The load rules are settled; the bank itself is not.

5. **Moisture behind waterproof panels near a diesel heater.** Plastic panels are vapour-tight, so moisture can form behind them if the wall is cold, and ordinary thin PVC may be unsuitable close to the heater outlet. The design uses battens, insulation behind the panels, sealed penetrations and a heat shield, with the panel fire rating still to be confirmed. This addresses condensation and clearance without committing to a product prematurely.

6. **Underslung tanks in freezing weather.** Below-floor tanks are exposed to road conditions and low temperatures. The design requires insulation and a heating method; candidate measures include thermostatically controlled 12 V heater pads, insulated pipework and low-point drain valves, with no antifreeze in the fresh tank. The requirement is captured, but the heating hardware and its effect on the power budget are unresolved.

## Results and Validation

The project has produced installed hardware and a substantial design record, but the wet-area systems have not yet been built or tested. Validation is therefore documentary and fabrication-based rather than experimental.

| Area | Current evidence |
| --- | --- |
| Solar | Four 200 W panels installed; 2S2P wiring and 60 A MPPT recorded. No generation logs are included. |
| Diesel heating | Airtronic D4 and 802 controller mounted. The shower drying branch and changeover damper are not installed. |
| Furniture | Table modelled, toolpathed and CNC-cut; legs and stiffener cut and fitted. |
| Shower, toilet, water and electrical distribution | Requirements, bills of materials and decision records only. No installation, water-use, thermal or electrical performance data. |

No automated test suite exists because this is a documentation and fabrication project. The main recorded outcomes are the installed solar array, the mounted heater and controller, the fitted table parts, and a cross-linked design record that identifies conflicting manufacturer data and unresolved safety questions. The Loopz specifications and the battery bank remain the most significant unverified assumptions.

## Getting Started

### Prerequisites

- A Markdown viewer or GitHub for reading the documentation.
- [Obsidian](https://obsidian.md/) with the Kanban plugin to render the board and follow wikilinks as intended.
- [FreeCAD](https://www.freecad.org/) to open the `.FCStd` models and fabrication exports.
- [KiCad](https://www.kicad.org/) to open the schematic and PCB project.

### Clone the repository

```bash
git clone git@github.com:BenjaminJAnderson/TheUglyDuckling.git
```

### Browse the documentation

1. Open [Dashboard](00%20-%20Project/Dashboard.md) for the current focus and the full page map.
2. Start with [Kitchen, Shower & Toilet](01%20-%20INTERIOR/Kitchen%2C%20Shower%20%26%20Toilet.md) for the wet-area overview.
3. Follow the area pages for [Kitchen](01%20-%20INTERIOR/Kitchen.md), [Shower](01%20-%20INTERIOR/Shower.md) and [Toilet](01%20-%20INTERIOR/Toilet.md).
4. Read the shared system pages for [Water](02%20-%20SYSTEMS/Water.md), [Ventilation & Moisture](02%20-%20SYSTEMS/Ventilation%20%26%20Moisture.md), [Diesel Heater](02%20-%20SYSTEMS/Diesel%20Heater.md) and [Electrics Overview](02%20-%20SYSTEMS/Electrical/Electrics%20Overview.md).
5. Check [Decisions](00%20-%20Project/Decisions.md) before changing a design, and update [Kanban](00%20-%20Project/Kanban.md) and [Shopping List](00%20-%20Project/Shopping%20List.md) when work or purchasing status changes.

### Work with the models

Open the native FreeCAD or KiCad files rather than the exported STL, STEP, DXF or G-code. The exports are fabrication outputs and may not reflect later changes to the master model. Check dimensions against the vehicle before cutting, drilling or ordering parts.

## Roadmap

- [ ] Order the Loopz Plus and confirm maximum water temperature, weight and deck load with Hamwells.
- [ ] Choose the composting toilet model and its vent connection.
- [ ] Build the shower walls, floor support, threshold and removable base seal.
- [ ] Install the new shower extractor, duct and roof vent.
- [ ] Install the diesel-heater drying branch, changeover damper, diffuser and heat shield.
- [ ] Source and mount the underslung fresh and grey tanks.
- [ ] Resolve tank insulation, heating and winterising.
- [ ] Decide the final battery chemistry and capacity, then complete the 12 V and 230 V load schedule.
- [ ] Specify and install the kitchen sink, filtration, induction hob, fridge and ventilation.
- [ ] Confirm the fire rating of the shower panels near the heater outlet.
- [ ] Design safe roof access for solar and vent maintenance without a permanent ladder.

## Project Structure

```text
TheUglyDuckling/
├── 00 - Project/        Dashboard, Kanban, decisions, shopping list and page template
├── 01 - INTERIOR/       Kitchen, shower, toilet, bed, seating, cab, lining and storage
├── 02 - SYSTEMS/        Water, ventilation, diesel heating and electrical notes
├── 03 - EXTERIOR/       Solar, roof, caulking, lights, paint, antenna and ladder
├── CAD Files/
│   ├── FreeCAD/         Native models and STEP, STL and DXF exports
│   ├── GCODE/           CNC toolpaths for table and stiffener parts
│   └── STL/             STL, STEP, DXF and SVG fabrication exports
├── Electric Wiring Guide/
│   └── Wiring/          KiCad schematic, PCB layout, project and symbol library
├── AGENTS.md            Repository conventions, design decisions and safety notes
└── README.md            Project overview and portfolio entry point
```

## Credits and Licensing

### Tools and references

- [Obsidian](https://obsidian.md/) for the linked Markdown vault and Kanban board.
- [FreeCAD](https://www.freecad.org/) for parametric models and fabrication exports.
- [KiCad](https://www.kicad.org/) for the electrical schematic and PCB design.
- Product references and supplier links for Hamwells, Eberspächer, Xantrex, Sterling Power, Victron Energy, Fullriver, Lucas and Voltanic are recorded in the relevant system pages and the [Shopping List](00%20-%20Project/Shopping%20List.md).

Product names and trademarks remain the property of their respective owners. Component specifications are quoted from manufacturer material and supplier pages; where sources disagree, the discrepancy is recorded in the page rather than resolved by assumption.

### Licensing

No licence file is currently included in this repository. Reuse permissions for the documentation, CAD models and fabrication files are therefore unspecified. Anyone wishing to reuse or redistribute the material should contact the repository owner first.
