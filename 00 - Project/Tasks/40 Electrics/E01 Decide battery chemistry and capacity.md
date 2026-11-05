---
tags: [task, area/electrics, phase/design]
status: done
start: 2026-11-02
end: 2026-11-15
effort_days: 1
progress: 100
updated: 2026-11-05
---

# E01 Decide battery chemistry and capacity

## Outcome

The leisure battery bank chemistry and capacity are chosen.

## Done when

- [x] AGM and LiFePO4 options compared
- [x] Capacity chosen: 314 Ah LiFePO4 installed
- [x] Inverter surge and 1.5 kW loads considered; detailed test moved to [[E02 Complete load schedule and cable-fuse sizing]]
- [x] Charging sources checked for compatibility
- [x] [[Electrics Overview]] and [[Decisions]] updated

## Notes

- Installed bank: [[Eco-Worthy EnergyTrek 12V 314Ah LiFePO4 Battery]], 12.8 V, 314 Ah, 4,019 Wh, 200 A BMS, Bluetooth, low-temperature protection.
- The old lead-acid auxiliary system and split-charge relays have been removed. The DC-DC charger is the only alternator-to-leisure path.
- The 200 A BMS is adequate for the 1.5 kW loads, but the Xantrex 3000 W surge is above the battery's 240 A/10 s peak. Test it in E02.
- The MPPT, Pro Charge Ultra and BaBy must all use a LiFePO4 profile.
- The AGM component pages remain as research history.

## Links

- [[Electrics Overview]]
- [[Decisions]]
- [[Project Plan]]
- [[Eco-Worthy EnergyTrek 12V 314Ah LiFePO4 Battery]]
