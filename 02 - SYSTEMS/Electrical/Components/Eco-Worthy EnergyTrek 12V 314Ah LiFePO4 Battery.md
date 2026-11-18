---
tags: [systems, electrical, battery, lithium]
status: installed
updated: 2026-11-18
---

# Eco-Worthy EnergyTrek 12V 314Ah LiFePO4 Battery

**Category:** 12 V LiFePO4 Leisure Battery
**Manufacturer:** Eco-Worthy
**Model:** EnergyTrek 12V 314Ah (the product URL uses 300Ah)
**Product page:** [Eco-Worthy EnergyTrek 12V 314Ah](https://uk.eco-worthy.com/products/eco-worthy-12v-300ah-lifepo4-lithium-battery-bluetooth-with-soc-leds-and-low-temp-protection?currency=GBP&country=GB&variant=47914078830832)
**Primary purpose:** Installed 12 V leisure battery bank for the ambulance.

## Purpose

The Eco-Worthy EnergyTrek is the installed leisure bank. It is a 12.8 V LiFePO4 battery with a nominal 314 Ah capacity, a 200 A battery management system (BMS), Bluetooth monitoring and low-temperature charging protection.

The previous lead-acid auxiliary system and its split-charge relays have been removed. The alternator now reaches the leisure bank only through the DC-DC charger, which is to be replaced by the [[Sterling Power BB1225 25A DC-DC Charger]]. Solar remains the primary charging source.

## Key specifications

| Specification | Value |
| --- | --- |
| Chemistry | LiFePO4 |
| Nominal voltage | 12.8 V |
| Rated capacity | 314 Ah |
| Nominal energy | 4,019 Wh |
| Operating voltage | 9.2–14.6 V |
| Maximum charging voltage | 14.6 V |
| Standard charge current | 157 A |
| Maximum charge current | 200 A |
| Standard discharge current | 157 A |
| Maximum continuous discharge current | 200 A |
| Peak discharge current | 240 A for 10 seconds |
| Charging temperature | 0–55 °C |
| Discharging temperature | -20–55 °C |
| Low-temperature protection | Charging stops below approximately -7 °C |
| BMS | Integrated 200 A |
| Monitoring | Bluetooth app and SOC LED indicators |
| Terminal size | M8 |
| Case material | ABS + PC |
| Dimensions | 414 × 215 × 260 mm |
| Weight | Approximately 27.4 kg |
| Cycle life | 6,000+ cycles under suitable conditions |
| Warranty | Confirm with Eco-Worthy; not recorded |

The listing URL says 300 Ah, but the product page and specification table state 314 Ah. Recorded as 314 Ah with the discrepancy noted.

## Installed configuration

- The battery is the single 12 V leisure bank. No series or parallel expansion is recorded.
- The old lead-acid auxiliary battery system and split-charge relays have been removed.
- The installed Voltanic 60 A DC-DC is the present alternator-to-leisure path and is to be replaced by the Sterling BB1225 25 A DC-DC.
- The 800 W solar array and 60 A MPPT are installed. The Sterling Pro Charge Ultra 60 A shore charger and the BB1225 are planned additions.
- The planned Xantrex PROwatt SW 2000i inverter is to have its own fuse and isolation.
- No separate shunt or system battery monitor is recorded; the battery's Bluetooth app and SOC LEDs provide direct battery monitoring.

## Charging

- The battery's maximum charging voltage is 14.6 V.
- The BB1225 Lithium I profile uses 14.4 V absorption and lists 13.8 V float, which is compatible. The manual also states that lithium profiles use live output voltage, so confirm the float behaviour.
- The MPPT and Pro Charge Ultra must both use a LiFePO4 profile, not a lead-acid or equalisation profile.
- At 25 A, the BB1225 charges at about 0.080C. Replacing 50% depth of discharge (157 Ah) takes about 6.3 hours; 80% (251 Ah) takes about 10 hours. The BB1225 is a maintenance and trickle source, not the bulk charger. The 800 W solar array and 60 A MPPT remain the bulk source.
- The battery BMS stops charging below approximately -7 °C. The BB1225 stops at 0 °C, which is more conservative and matches the battery's stated 0–55 °C charging range. Fit the BB1225 temperature sensor to the battery negative.
- The battery has its own low-temperature protection, so the BB1225 trip is a second layer rather than the only protection.

## Discharge and inverter

- The 200 A BMS supports 200 A continuous discharge and 240 A for 10 seconds.
- A 2 kW inverter load at 12 V is about 185 A after allowing for efficiency, within the 200 A continuous rating but with little headroom for other DC loads.
- The Xantrex PROwatt SW 2000i has a 3000 W surge for 5 seconds, roughly 278 A at 12 V. That exceeds the battery's 240 A/10 s peak. Test the inverter surge against the BMS before relying on the full inverter rating.
- The 1.5 kW kettle draws about 139 A after efficiency losses and the 1.0 kW Sterling IH1L hob about 93 A; both remain comfortably within the BMS rating. Do not run them together.

## Installation notes

- The battery weighs about 27.4 kg and measures 414 × 215 × 260 mm. Confirm the floor, restraint and ventilation before final assembly.
- Use M8 terminals and correctly rated cable lugs.
- Fit a main fuse close to the battery positive terminal and provide a battery isolation switch.
- Keep the battery in a dry, ventilated location and away from direct heat sources.
- Check the inverter cable size, fuse rating and isolation switch against the 200 A BMS and the 2 kW inverter load.
- If a shunt is added later, connect the BB1225 output and all charge sources to the battery side of the shunt so their current is measured.

## Open questions

- Confirm the exact model and purchase price paid. The page currently shows £409.99 for one battery, with a £499.98 comparison price.
- Confirm whether the battery is the 314 Ah model or a 300 Ah variant; the URL and product page disagree.
- Confirm the BMS surge behaviour with the Xantrex 2000 W inverter, especially the 3000 W/5 s surge.
- Confirm the BMS low-temperature cutoff against the BB1225's 0 °C trip.
- Confirm whether a shunt or system battery monitor will be added.
- Confirm the battery mounting, restraint and ventilation in the final layout.
- Confirm the battery warranty terms.

## Purchase

| Item | Qty | Spec / Model | Supplier / Link | Price | Status | Notes |
| --- | --- | --- | --- | --- | --- | --- |
| Eco-Worthy EnergyTrek battery | 1 | 12 V 314 Ah LiFePO4, 4,019 Wh, 200 A BMS, Bluetooth, low-temperature protection | [Eco-Worthy](https://uk.eco-worthy.com/products/eco-worthy-12v-300ah-lifepo4-lithium-battery-bluetooth-with-soc-leds-and-low-temp-protection?currency=GBP&country=GB&variant=47914078830832) | £409.99 current; paid TBC | installed | Listing URL says 300 Ah; product page says 314 Ah |

## Related

- [[Electrics Overview]]
- [[Sterling Power BB1225 25A DC-DC Charger]]
- [[Sterling Power Pro Charge Ultra 12V 60A]]
- [[Xantrex PROwatt SW 2000i Inverter]]
- [[Solar]]
- [[Decisions]]
- [[Shopping List]]
