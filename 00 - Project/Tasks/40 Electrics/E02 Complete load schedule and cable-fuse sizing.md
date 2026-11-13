---
tags: [task, area/electrics, phase/design]
status: todo
start: 2026-11-09
end: 2026-11-20
effort_days: 1
progress: 0
after:
  - "FS:[[E01 Decide battery chemistry and capacity]]"
updated: 2026-11-13
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
- The BB1225 manual specifies 6 mm² / 10 AWG cable and about 30 A fuses at both batteries; some mode diagrams show 50 A, so confirm the final fuse rating.
- Replace the removed 60 A DC-DC's fuses with about 30 A fuses and check whether the existing lugs fit the BB1225 terminals; the manual does not state the terminal diameter.
- The Xantrex 2000 W inverter draws about 185 A continuously and about 278 A at its 3000 W surge. The battery's BMS is 200 A continuous and 240 A for 10 seconds; test the surge and keep the 1.5 kW appliance limit.

## Links

- [[Electrics Overview]]
- [[Water]]
- [[Project Plan]]
- [[Eco-Worthy EnergyTrek 12V 314Ah LiFePO4 Battery]]
- [[Sterling Power BB1225 25A DC-DC Charger]]
