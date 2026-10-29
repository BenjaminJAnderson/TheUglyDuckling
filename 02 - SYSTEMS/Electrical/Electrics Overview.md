---
tags: [systems, electrical]
status: planning
updated: 2026-10-21
---

# Electrics Overview

## Overview

The ambulance uses a 12 V leisure system with 800 W of solar, a 60 A MPPT controller, a Sterling Pro Charge Ultra 60 A shore charger and a Xantrex PROwatt SW 2000i pure-sine inverter. The final leisure battery chemistry and capacity are still open.

## System diagram

```text
4 × 200 W solar panels
        │
        ▼
   60 A MPPT ──────────┐
                       │
230 V shore power      │
        │              ▼
        ▼        Leisure battery bank
Sterling 60 A charger ─┘        │
                                ├──► Xantrex 2000 W inverter ──► 230 V sockets
                                │
                                ├──► DC fuse panel
                                │      ├── Kitchen fridge
                                │      ├── Water pump
                                │      ├── Loopz Plus (60 W)
                                │      ├── Diesel heater
                                │      ├── Extractor fans
                                │      └── Lighting
                                │
                                └──► Victron BatteryProtect BP-65
```

Alternator/DC-DC charging is referenced in the component notes but still needs to be confirmed in the final design.

## Charging sources

| Source | Equipment | Status |
| --- | --- | --- |
| Solar | 4 × 200 W panels, 2 series / 2 parallel, 60 A MPPT | Installed |
| Shore power | Sterling Pro Charge Ultra 12 V / 60 A | Planned |
| Alternator/DC-DC | TBC | Open |

## Battery bank

- Current candidate batteries: [[Fullriver DC115-12 AGM Deep-Cycle Leisure Battery]] and [[Lucas LSLC125-12 AGM Leisure Battery]].
- Do not mix different battery models in one permanent parallel bank.
- The 2000 W inverter and 1.5 kW induction/kettle loads are demanding for a small AGM bank.
- A matched AGM bank or a LiFePO4 bank still needs to be decided.

## 12 V distribution

- Main battery fuse close to the battery positive terminal.
- DC busbars for high-current connections.
- Fuse panel/breakers for individual circuits.
- [[Victron Energy Battery Protect 12-24V 65A (BP-65)]] for protected DC loads.
- Large loads such as the inverter bypass the BatteryProtect and have their own fuse.
- Cable sizes and fuse ratings to be calculated from actual loads and run lengths.

Typical 12 V loads:

| Load | Approximate load | Notes |
| --- | --- | --- |
| Loopz Plus shower | 60 W / ~5 A | Only while showering |
| Composting-toilet fan | TBC | Continuous, low power |
| Diesel heater | TBC | Installed; fuse per Eberspächer manual |
| Water pump | TBC | Intermittent |
| Drawer fridge | TBC | Compressor cycling |
| Extractor fans | TBC | Intermittent |
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

- [[Diesel Heater]]
- [[Xantrex PROwatt SW 2000i Inverter]]
- [[Sterling Power Pro Charge Ultra 12V 60A]]
- [[Victron Energy Battery Protect 12-24V 65A (BP-65)]]
- [[Fullriver DC115-12 AGM Deep-Cycle Leisure Battery]]
- [[Lucas LSLC125-12 AGM Leisure Battery]]

## CAD and wiring

- `Electric Wiring Guide/Wiring/Wiring.kicad_sch`
- `Electric Wiring Guide/Wiring/Wiring.kicad_pcb`
- `CAD Files/FreeCAD/Electrics.FCStd`

## Open questions

- Final battery chemistry and capacity.
- Alternator/DC-DC charging design.
- Inverter cable size, fuse rating and isolation switch.
- Whether the induction hob and kettle can run from the AGM bank without unacceptable voltage sag.
- 230 V socket layout.
- Solar cable entry, isolation and fusing.
- Battery monitoring and shunt.
- Shore-power inlet location and changeover method.

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
