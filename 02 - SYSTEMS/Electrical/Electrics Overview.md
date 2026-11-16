---
tags: [systems, electrical]
status: planning
updated: 2026-11-16
---

# Electrics Overview

## Overview

The ambulance uses a 12 V leisure system with an installed Eco-Worthy 314 Ah LiFePO4 battery, 800 W of solar, a 60 A MPPT controller, a Sterling Pro Charge Ultra 60 A shore charger and a Xantrex PROwatt SW 2000i pure-sine inverter. A Sterling BB1225 25 A DC-DC is planned to replace the installed Voltanic 60 A unit for alternator charging and starter battery maintenance.

## System diagram

```text
4 × 200 W solar panels
        │
        ▼
   60 A MPPT ──────────┐
                       │
230 V shore power      │
        │              ▼
        ▼        Leisure battery bank ◄──► Sterling BB1225 25 A DC-DC ◄──► Starter battery
Sterling 60 A charger ─┘        │
                                ├──► Xantrex 2000 W inverter ──► 230 V sockets
                                │
                                └──► DC fuse panel
                                       ├── Kitchen fridge/freezer
                                       ├── Water pump
                                       ├── Loopz Plus (60 W)
                                       ├── Diesel heater
                                       ├── Extractor fans
                                       └── Lighting
```

The BB1225 charges the leisure bank while the engine is running and reverse-charges the starter battery when the leisure bank is above 13.5 V on the lithium profile. The reverse-charge path is a maintenance function, not a full starter charger. Use the ignition feed for this installation and confirm it is live only while the engine is running.

## Charging sources

| Source | Equipment | Status |
| --- | --- | --- |
| Solar | 4 × 200 W panels, 2 series / 2 parallel, 60 A MPPT | Installed |
| Shore power | Sterling Pro Charge Ultra 12 V / 60 A | Planned |
| Alternator/DC-DC | Sterling BB1225 25 A battery-to-battery charger | Shortlisted |
| Starter maintenance | BB1225 reverse charge, 13.4 V maintenance | Shortlisted |

The installed Voltanic 60 A DC-DC is to be removed and sold. The BB1225 is a lower-current replacement intended for occasional driving and solar-primary charging, not bulk alternator charging.

## Battery bank

- Installed: [[Eco-Worthy EnergyTrek 12V 314Ah LiFePO4 Battery]], 12.8 V, 314 Ah, 4,019 Wh, 200 A BMS, Bluetooth monitoring, SOC LEDs and low-temperature charging protection.
- The product URL says 300 Ah, but the product page and specification table state 314 Ah; confirm the exact model.
- The previous lead-acid auxiliary system and split-charge relays have been removed. The DC-DC is the only alternator-to-leisure path.
- The MPPT, Pro Charge Ultra and BB1225 must all use a LiFePO4 profile. The battery's maximum charging voltage is 14.6 V; the BB1225 Lithium I profile uses 14.4 V absorption and lists 13.8 V float, but the manual also states that lithium profiles use live output voltage, so confirm the float behaviour.
- The 2000 W inverter and 1.5 kW induction/kettle loads are demanding for the bank. The 200 A BMS is adequate for the 1.5 kW loads, but the inverter's 3000 W surge is above the battery's 240 A/10 s peak; test before relying on the full inverter rating.
- The Fullriver DC115-12 and Lucas LSLC125-12 pages are retained as AGM research history, not as the installed bank.

## 12 V distribution

- Main battery fuse close to the battery positive terminal.
- DC busbars for high-current connections.
- Fuse panel/breakers for individual circuits.
- Large loads such as the inverter have their own fuse.
- The DC-DC output and reverse-charge path connect to the battery busbar or main fuse side.
- If a shunt or system battery monitor is added, connect all charge sources to the battery side of the shunt so their current is measured.
- Cable sizes and fuse ratings to be calculated from actual loads and run lengths. The BB1225 manual specifies 6 mm² / 10 AWG cable and about 30 A fuses at both batteries.

Typical 12 V loads:

| Load | Approximate load | Notes |
| --- | --- | --- |
| Loopz Plus shower | 60 W / ~5 A | Only while showering |
| Diesel heater | TBC | Installed; fuse per Eberspächer manual |
| Water pump | TBC | Intermittent |
| 50 L fridge/freezer | 60 W / ~5 A at 12 V | Compressor cycling; confirm duty cycle. The 24 V rating is not used on this 12 V system. |
| Shower extractor/light (MaxxFan Dome Plus) | 24 W / ~2 A | Single speed; 5 A circuit fuse; intermittent |
| Kitchen extractor | TBC | Intermittent |
| Lighting | TBC | LED |
| USB sockets | TBC | Small |

## 230 V distribution

- [[Xantrex PROwatt SW 2000i Inverter]] supplies 230 V sockets when off-grid.
- Shore power inlet with RCD/RCBO protection.
- Consumer unit with RCD/RCBO.
- Earth bonding.
- Dedicated isolation for the induction hob and kettle circuits.
- Drip loops and water separation.

### 230 V loads

| Load | Rating | Notes |
| --- | --- | --- |
| Induction hob | 1.5 kW max | Inverter-powered; do not run with kettle |
| Kettle | 1.5 kW max | Inverter-powered; do not run with hob |
| 230 V sockets | TBC | Small electronics and chargers |

The 2000 W inverter is close to its continuous limit with either the hob or the kettle. Both together will overload it.

## Protection and safety

- Fuse DC circuits close to the source.
- Use RCD/RCBO protection on 230 V circuits.
- Keep 230 V AC and water separated.
- Use drip loops and sealed cable entries.
- Label all circuits.
- Provide a main battery isolation switch.
- Check cable size and fuse rating for the inverter, charger and solar controller.
- Do not leave the inverter permanently on; standby current drains the battery.

## Components

- [[Eco-Worthy EnergyTrek 12V 314Ah LiFePO4 Battery]]
- [[Sterling Power BB1225 25A DC-DC Charger]]
- [[MaxxFan Dome Plus]]
- [[Diesel Heater]]
- [[Xantrex PROwatt SW 2000i Inverter]]
- [[Sterling Power Pro Charge Ultra 12V 60A]]
- [[Fullriver DC115-12 AGM Deep-Cycle Leisure Battery]] — AGM research history
- [[Lucas LSLC125-12 AGM Leisure Battery]] — AGM research history

## CAD and wiring

- `Electric Wiring Guide/Wiring/Wiring.kicad_sch`
- `Electric Wiring Guide/Wiring/Wiring.kicad_pcb`
- `CAD Files/FreeCAD/Electrics.FCStd`

## Open questions

- Inverter surge versus the 200 A BMS; test the 3000 W surge and keep the 1.5 kW appliance limit.
- Whether 25 A alternator charging is adequate for the final travel pattern; the BB1225 is a maintenance source, not a bulk charger.
- BB1225 ignition-feed source and whether the existing feed is live only with the engine running.
- Whether the existing 60 A cable lugs fit the BB1225 terminals; the manual does not state the terminal diameter. Replace the 60 A fuses with about 30 A fuses.
- Reverse-charge behaviour and whether to disable reverse charging for long storage.
- Whether the manual's lithium float statement means Lithium I holds a float or a live output voltage.
- Whether a shunt or system battery monitor will be added.
- Inverter cable size, fuse rating and isolation switch.
- Fridge/freezer duty cycle for the load schedule.
- Confirm the MaxxFan Dome Plus current with the LED; allow a 5 A circuit fuse.
- Whether the induction hob and kettle can run from the bank without unacceptable voltage sag.
- 230 V socket layout.
- Solar cable entry, isolation and fusing.
- Shore-power inlet location and changeover method.
- KiCad schematic and FreeCAD electrical layout still show the removed 60 A unit; update them separately if required.

## Related

- [[Kitchen]]
- [[Shower]]
- [[Toilet]]
- [[Water]]
- [[Ventilation & Moisture]]
- [[Diesel Heater]]
- [[Solar]]
- [[Roof]]
- [[Dashboard]]
