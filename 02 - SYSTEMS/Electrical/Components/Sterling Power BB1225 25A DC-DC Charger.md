---
tags: [systems, electrical, charger, dc-dc]
status: shortlisted
updated: 2026-11-13
---

# Sterling Power BB1225 25A DC-DC Charger

**Category:** DC → DC Battery Charger / Battery Maintainer
**Manufacturer:** Sterling Power Products
**Model:** BB1225 (Saturn range)
**Part number:** BB1225
**Product page:** [Sterling Power BB1225](https://sterling-power.com/products/bb1220-reverse-charge-jump-start-assistance-copy)
**Primary purpose:** Charge the 12 V leisure bank from the starter battery and alternator while the engine is running, with reverse charging to maintain the starter battery from surplus leisure-bank charge.

## Purpose

The BB1225 is a 12 V to 12 V, 25 A battery-to-battery charger (26 A input rated). It charges the leisure bank from the starter battery and alternator while the engine is running. Its reverse-charging feature uses surplus leisure-bank voltage, normally from solar or shore power, to maintain the starter battery at about 13.4 V.

It is to replace the installed Voltanic 60 A DC-DC. The 60 A unit is to be removed and sold because the vehicle spends most of its time stationary, the 314 Ah LiFePO4 bank is charged mainly by the 800 W solar array, and the lower current simplifies the alternator, cable and fuse requirements. The BB1225 also provides starter maintenance that the Voltanic unit does not.

## Key specifications

| Specification | Value |
| --- | --- |
| Nominal voltage | 12 V |
| Input voltage range | 9–16 V |
| Output current | 25 A nominal; 24 A maximum at 14.41 V per manual |
| Maximum output power | About 345 W at 14.41 V |
| Maximum input current | 26 A at 13.68 V, about 355 W |
| Output at lower input voltage | About 24 A above 13.2 V; about 19 A at 12.8–13.2 V; about 15 A below 12.8 V |
| Efficiency | 98% |
| Quiescent current | 5 mA |
| Battery profiles | Six presets: Lead I/II, AGM I/II and Lithium I/II |
| Default profile | Lead I: 14.4 V absorption and 13.3 V float |
| Lithium I profile | 14.4 V absorption and 13.8 V float listed; the manual also states that lithium profiles use live output voltage, so confirm the float behaviour |
| Low-temperature protection | Stops charging at 0 °C or below on lithium profiles |
| Activation | Automatic at 13.5 V input on and 12.8 V off; ignition feed at 11 V on and 10 V off; vibration sense |
| Reverse charging | Maintains the starter battery at about 13.4 V; engages at 13.5 V leisure voltage on lithium or 13.2 V on lead-acid; can be disabled |
| Jump start assist | Select button pressed four times; needs at least 11 V on the leisure battery and 5.5 V on the starter battery |
| Smart alternator support | Yes; use the ignition feed on Euro 6 vehicles |
| Dimensions | 123 × 130 × 56 mm |
| Weight | 0.6 kg |
| Cooling | Thermostatically controlled variable low-speed fan |
| Protections | Under-voltage, input over-voltage, output over-voltage, over-current, over-temperature and fan fault |
| Approvals | CE, UKCA and E-marking |
| Water protection | Not waterproof; the manual requires a dry, well-ventilated, dust-free and condensation-free location |
| Warranty | 2 years return to factory per the supplied 2023 manual; current Sterling Saturn listings state 5 years, so confirm |
| Price | £190.80 inc VAT on the Sterling listing; confirm current price and stock |

The manual specifies 6 mm² / 10 AWG cable for both the input and output and a fuse of about 30 A at each battery. Some of the manual's mode diagrams show 50 A fuses instead, so confirm the final fuse rating against the installed cable and the unit's 26 A input rating.

## How it works

- In automatic mode the unit starts when the input is above 13.5 V and stops when it falls below 12.8 V. Use the ignition-feed mode on a Euro 6 or smart-alternator vehicle: the unit then runs when the feed is live and needs at least 11 V on the input battery.
- Once an ignition feed has been connected, the unit remains dependent on that signal. To revert to automatic mode, remove the feed and hold the front button for about 15 seconds until the battery-type LEDs flash together.
- Select the Lithium I profile for the Eco-Worthy bank and confirm the absorption and float behaviour against the battery requirements.
- Reverse charging engages from surplus leisure-bank voltage and maintains the starter battery at about 13.4 V. It does not intentionally deplete the leisure bank. It can be disabled by holding the Select button for 20 seconds, then toggling the reverse-charging LED.
- Jump start assist forces a back-feed to the starter battery. It is an assist, not a substitute for a jump pack.
- Vibration-sense activation is available but is not recommended for a camper because movement or wind could activate charging when the engine is off.
- Optional connections include a 12 V 50 mA signal output, a 12 V 100 mA alarm output, the included temperature sensor and the optional BBR remote control.

## Suitability for the ambulance

- The installed leisure bank is a 314 Ah LiFePO4 battery. At 25 A the charge rate is about 0.080C, so the BB1225 is a maintenance and trickle source rather than the bulk charger. Solar through the 60 A MPPT remains the main source.
- Replacing 50% depth of discharge on the 314 Ah bank would take about 6.3 hours at 25 A, or about 10 hours for 80%. This is acceptable because driving is infrequent.
- The Lithium I absorption voltage of 14.4 V is compatible with the battery's 14.6 V maximum. The manual's lithium float statement is ambiguous, so confirm whether the profile holds a float or a live output voltage.
- The BB1225's 0 °C low-temperature trip is more conservative than the battery BMS cutoff at about -7 °C. This is safe but means the BB1225 will not charge between -7 °C and 0 °C.
- The Pro Charge Ultra has three isolated outputs and can maintain the starter battery on shore power. The BB1225 adds starter maintenance from solar when off-grid. Use the ignition-feed mode so the shore charger's starter output cannot trigger forward charging through the BB1225.
- Connect the BB1225 output and reverse-charge path to the battery busbar or the battery side of the main fuse.
- The BB1225 is not an MPPT. The existing 60 A solar MPPT remains in service.

## Installation notes

- Take the positive input from the starter battery, not directly from an alternator with no battery on the same line.
- Fit a fuse of about 30 A close to the starter battery and another close to the leisure battery. Replace the removed 60 A fuses. Confirm the 30 A figure because the manual's mode diagrams also show 50 A.
- Use 6 mm² / 10 AWG cable for the input and output. Check the voltage drop on long runs and upsize if required.
- Both negatives on the unit are common. Run a direct negative between the starter battery, the BB1225 and the leisure battery; avoid chassis points where possible.
- Fit the included temperature sensor to the negative terminal of the leisure battery.
- Use a fused ignition feed that is live only when the engine is running. Do not use an accessory-only circuit.
- Mount the unit in a dry, ventilated, dust-free location. It is not waterproof and has a cooling fan. It can be mounted in any orientation, but avoid an orientation where water could pool.
- Set the Lithium I profile and confirm the absorption and float voltages against the battery manufacturer's requirements.
- Test forward charging with the engine running and reverse charging with the leisure bank above 13.5 V.

## Removal of the Voltanic 60 A unit

- The Voltanic 60 A DC-DC is installed and is to be removed. Do not run both units.
- Remove its 60 A fuses; do not reuse them with the BB1225.
- Check whether the existing cable lugs fit the BB1225 terminals. The manual does not state the terminal diameter. Reuse the heavy cable only if the lugs fit and the fuses are changed to about 30 A; otherwise fit 6 mm² / 10 AWG cable.
- Reuse the existing ignition feed only if it is live solely with the engine running.
- The removed unit can be sold. Record the removal and any sale proceeds with the electrical budget.

## Limitations and open questions

- Confirm the price, stock and lead time. The Sterling listing currently shows £190.80 inc VAT.
- Confirm the warranty: the supplied 2023 manual states 2 years, while current Sterling Saturn listings state 5 years.
- Confirm the fuse rating: the connector instructions say about 30 A, while some mode diagrams show 50 A.
- Confirm the terminal diameter and whether the existing lugs fit; the manual does not state it.
- Confirm the Lithium I float behaviour and whether a different profile is preferable for long-term maintenance of the LiFePO4 bank.
- Confirm the reverse-charge current; the manual states the 13.4 V maintenance voltage but does not give a current figure.
- A full LiFePO4 bank at rest may sit below the 13.5 V reverse-charge threshold, so starter maintenance may stop overnight.
- The unit has no display. Use the Eco-Worthy battery's Bluetooth app and SOC LEDs for battery status. The optional BBR remote adds live voltage and current readings.
- Confirm the mounting location is dry and has airflow. The unit is not waterproof.
- Confirm the existing cable lugs, fuse holders and ignition feed before ordering.

## Purchase

| Item | Qty | Spec / Model | Supplier / Link | Price | Status | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| Sterling BB1225 25 A DC-DC | 1 | BB1225, 12 V–12 V, 25 A, reverse charging | [Sterling Power](https://sterling-power.com/products/bb1220-reverse-charge-jump-start-assistance-copy) | £190.80 inc VAT | shortlisted | 6 mm² cable and about 30 A fuses; 2-year manual warranty; confirm price |
| 30 A fuse and holder | 2 | Input and output protection | TBC | TBC | research | One close to each battery; some diagrams show 50 A |
| DC-DC cable | TBC | 6 mm² / 10 AWG, length TBC | TBC | TBC | research | Upsize if the voltage drop is excessive |
| Ignition feed fuse | 1 | 2–5 A, engine-only live | TBC | TBC | research | Do not use an accessory circuit |
| Temperature sensor | 1 | Included with the unit | — | — | included | Fit to the leisure battery negative |

## Related

- [[Electrics Overview]]
- [[Eco-Worthy EnergyTrek 12V 314Ah LiFePO4 Battery]]
- [[Sterling Power Pro Charge Ultra 12V 60A]]
- [[Xantrex PROwatt SW 2000i Inverter]]
- [[Solar]]
- [[Decisions]]
- [[Shopping List]]
