---
tags: [task, area/electrics, phase/design]
status: todo
start: 2026-11-09
end: 2026-11-20
effort_days: 1
progress: 0
after:
  - "FS:[[E01 Decide battery chemistry and capacity]]"
updated: 2026-11-05
---

# E02 Complete load schedule and cable-fuse sizing

## Outcome

The 12 V and 230 V load schedule is complete, with cable sizes and fuse ratings calculated.

## Done when

- [ ] All 12 V loads listed with current and duty cycle
- [ ] All 230 V loads listed with ratings
- [ ] Inverter, charger, DC-DC and MPPT cable sizes calculated
- [ ] Main fuse and branch fuse ratings chosen
- [ ] 230 V RCBO and circuit ratings chosen
- [ ] Inverter surge checked against the 200 A battery BMS
- [ ] [[Electrics Overview]] updated

## Notes

- The induction hob and kettle are limited to 1.5 kW each and must not run together.
- Include the tank heating, extractors, heater and Loopz. The Boxio toilet has no electrical load.
- The BaBy manual recommends 4 mm² cable and 25 A fuses for the 15 A unit; upsize for runs over about 3 m.
- Replace the removed 60 A DC-DC's fuses with 25 A fuses and check whether the existing lugs fit the BaBy's 6.1 mm terminals.
- The Xantrex 2000 W inverter draws about 185 A continuously and about 278 A at its 3000 W surge. The battery's BMS is 200 A continuous and 240 A for 10 seconds; test the surge and keep the 1.5 kW appliance limit.

## Links

- [[Electrics Overview]]
- [[Water]]
- [[Project Plan]]
- [[Eco-Worthy EnergyTrek 12V 314Ah LiFePO4 Battery]]
- [[Sterling Power BaBy 15A DC-DC Charger]]
