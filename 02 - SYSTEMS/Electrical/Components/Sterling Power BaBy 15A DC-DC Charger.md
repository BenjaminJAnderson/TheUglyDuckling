---
tags: [systems, electrical, charger, dc-dc]
status: shortlisted
updated: 2026-11-05
---

# Sterling Power BaBy 15A DC-DC Charger

**Category:** DC → DC Battery Charger / Battery Maintainer
**Manufacturer:** Sterling Power Products
**Model:** BaBy (BB1215)
**Part number:** SKU `BABY`
**Product page:** [Sterling Power BaBy 15A](https://sterling-power.com/products/baby?variant=56896771424630)
**Primary purpose:** Bidirectional charging between the starter battery and the 12 V leisure bank, including starter battery maintenance from surplus solar.

## Purpose

The BaBy is a low-power bidirectional DC-DC charger and battery maintainer. In the normal direction it charges the leisure bank from the starter battery when the engine is running. In reverse it uses surplus leisure-bank voltage, normally from solar, to maintain the starter battery.

It is to replace the installed Voltanic 60 A DC-DC. The 60 A unit is to be removed and sold because the vehicle spends most of its time stationary, the 314 Ah LiFePO4 bank is charged mainly by the 800 W solar array, and the lower current greatly simplifies the alternator, cable and fuse requirements. The BaBy also provides the starter maintenance that the Voltanic unit could not.

## Key specifications

| Specification | Value |
| --- | --- |
| Nominal voltage | 12 V |
| Input voltage range | 9–16 V |
| Output current | 5–15 A nominal; manual lists 19 A maximum for BB1215 |
| Maximum output power | About 268 W at 14.41 V per manual |
| Maximum input current | About 21 A at 13.68 V per manual |
| Reverse charge current | 13 A per manual; product page describes about one-third of rating |
| Efficiency | 98% |
| Quiescent current | 5 mA |
| Reverse charge quiescent | 1.5–6 W per manual; confirm meaning |
| Battery profiles | 6 preset plus custom; LiFePO4 14.4 V absorption / 13.8 V float |
| Low-temperature protection | Stops charging at 0 °C on lithium profiles |
| Activation | Input above 13.5 V or ignition feed; vibration sense optional |
| Smart alternator support | Yes; use ignition feed on Euro 6 vehicles |
| Dimensions | 123 × 130 × 56 mm |
| Weight | 0.6 kg per manual; 1 kg on the product listing |
| Terminal diameter | 6.1 mm |
| Recommended cable | 4 mm² or larger for runs under 3 m; upsize for longer runs |
| Recommended fuses | 25 A input and output |
| Cooling | Thermostatically controlled variable-speed fan |
| Protections | Under-voltage, input over-voltage, output over-voltage, over-current, over-temperature |
| Approvals | CE, UKCA, E-marking |
| Water protection | Not stated as waterproof; the manual warns against water, spray and condensation |
| Warranty | 5 years advertised; manual states 2 years |
| Price | £149 inc VAT |

The product page advertises a 5–15 A range and a 5-year warranty, while the manual lists the BB1215 at 19 A maximum and a 2-year warranty. Confirm the current specification and warranty with Sterling before ordering.

## How it works

- The unit turns on when the input is above 13.5 V or when the ignition feed is live.
- On a Euro 6 or smart-alternator vehicle, use the ignition feed. The feed must be live only when the engine is running, not in accessory mode.
- Once an ignition feed has been connected, the unit remains dependent on that signal.
- Reverse charging engages when the leisure side is above 13.2 V on lead-acid profiles or 13.5 V on lithium profiles. It aims to bring the starter battery to a 13.4 V maintenance voltage.
- Reverse charging is enabled by default and can be disabled.
- Jump Start Assist forces reverse charging for 20 minutes. It is an assist, not a substitute for a jump pack.
- Vibration-sense activation is available but is not recommended for a camper because movement or wind could activate charging when the engine is off.

## Suitability for the ambulance

- The installed leisure bank is a 314 Ah LiFePO4 battery. At 15 A the charge rate is about 0.048C, so the BaBy is a maintenance and trickle source rather than the bulk charger. Solar through the 60 A MPPT remains the main source.
- Replacing 50% depth of discharge on the 314 Ah bank would take about 10.5 hours at 15 A, or about 16.7 hours for 80%. This is acceptable because driving is infrequent.
- The BaBy's 14.4 V absorption and 13.8 V float profile is compatible with the battery's 14.6 V maximum.
- The BaBy's 0 °C low-temperature trip is more conservative than the battery BMS cutoff at about -7 °C. This is safe but means the BaBy will not charge between -7 °C and 0 °C.
- The Pro Charge Ultra has three isolated outputs and can maintain the starter battery on shore power. The BaBy adds starter maintenance from solar when off-grid. Use the ignition-feed mode so the shore charger's starter output cannot trigger forward charging through the BaBy.
- Connect the BaBy output and reverse-charge path to the battery busbar or the battery side of the main fuse.
- The BaBy is not an MPPT. The existing 60 A solar MPPT remains in service.

## Installation notes

- Take the positive input from the starter battery or an alternator linearisation device, not directly from an alternator with no battery on the same line.
- Fit a 25 A fuse close to the starter battery and a 25 A fuse close to the leisure battery.
- Both negatives on the unit are common. Run a direct negative between the starter battery, the BaBy and the leisure battery; avoid chassis points where possible.
- Fit the temperature sensor to the negative terminal of the leisure battery.
- Use a fused ignition feed that is live only when the engine is running. Do not use an accessory-only circuit.
- Mount the unit in a dry, ventilated location. The proposed location has been confirmed dry. It is not waterproof and has a cooling fan. Avoid sideways mounting where water could pool.
- The unit is small and light enough to mount near the leisure bank, but keep the cable run as short as practical. Upsize to 6 mm² if the run exceeds about 3 m.
- Set the lithium charge profile and confirm the absorption and float voltages against the battery manufacturer's requirements.
- Test forward charging with the engine running and reverse charging with the leisure bank above 13.5 V.

## Removal of the Voltanic 60 A unit

- The Voltanic 60 A DC-DC is installed and is to be removed.
- Remove its 60 A fuses; do not reuse them with the BaBy.
- The existing heavy cable may be reused if the lugs fit the BaBy's 6.1 mm terminals and the fuses are changed to 25 A. Otherwise fit 4–6 mm² cable.
- Reuse the existing ignition feed only if it is live solely with the engine running.
- The removed unit can be sold. Record the removal and any sale proceeds with the electrical budget.

## Limitations and open questions

- Confirm the output rating: 15 A nominal on the product page versus 19 A maximum in the manual.
- Confirm the warranty: 5 years on the product page versus 2 years in the manual.
- Confirm the reverse-charge current: 13 A in the manual versus about one-third of rating on the product page.
- Confirm whether the 1.5–6 W reverse-charge quiescent figure is a continuous standby draw. If it is, consider disabling reverse charging or isolating the unit for long storage.
- The unit has no display. Use the Eco-Worthy battery's Bluetooth app and SOC LEDs for battery status. The optional BBR remote adds live voltage and current readings.
- Confirm the mounting location is dry and has airflow. The unit is not waterproof.
- Confirm the existing cable lugs, fuse holders and ignition feed before ordering.
- Confirm stock and lead time before relying on the April 2026 release date.

## Purchase

| Item | Qty | Spec / Model | Supplier / Link | Price | Status | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| Sterling BaBy 15 A DC-DC | 1 | BB1215, SKU `BABY`, bidirectional, 12 V–12 V, 5–15 A | [Sterling Power](https://sterling-power.com/products/baby?variant=56896771424630) | £149 inc VAT | shortlisted | 19 A maximum per manual; 4 mm² and 25 A fuses; confirm 5-year warranty |
| 25 A fuse and holder | 2 | Input and output protection | TBC | TBC | research | One close to each battery |
| DC-DC cable | TBC | 4–6 mm², length TBC | TBC | TBC | research | Upsize for runs over 3 m |
| Ignition feed fuse | 1 | 2–5 A, engine-only live | TBC | TBC | research | Do not use an accessory circuit |

## Related

- [[Electrics Overview]]
- [[Eco-Worthy EnergyTrek 12V 314Ah LiFePO4 Battery]]
- [[Sterling Power Pro Charge Ultra 12V 60A]]
- [[Xantrex PROwatt SW 2000i Inverter]]
- [[Solar]]
- [[Decisions]]
- [[Shopping List]]
