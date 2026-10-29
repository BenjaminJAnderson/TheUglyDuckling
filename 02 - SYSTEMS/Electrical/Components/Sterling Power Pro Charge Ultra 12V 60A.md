---
tags: [systems, electrical, charger, shore-power]
status: research
updated: 2026-10-21
---

# Sterling Power Pro Charge Ultra 12V 60A

**Category:** AC → DC Battery Charger  
**Manufacturer:** Sterling Power  
**Model:** Pro Charge Ultra 12V / 60A  
**Part number:** PCU1260  
**Primary purpose:** Charging the 12V leisure battery bank from **230V mains / shore power**

## Purpose

The Pro Charge Ultra is a **mains-powered intelligent battery charger**. When the ambulance is connected to campsite/shore mains, it converts AC mains electricity into regulated DC power for charging the leisure batteries.

It is therefore the **shore-power charging system** in your electrical setup.

```text
230V Shore Power
       │
       ▼
Pro Charge Ultra
       │
       ├──────► Starter Battery
       │
       ├──────► Leisure Battery Bank
       │
       └──────► Other Battery Bank
```

The 60A model can supply up to **60A of charging current** to a 12V battery system.

---

## Key Specifications

|Specification|Value|
|---|---|
|Model|Pro Charge Ultra 12V / 60A|
|Part number|PCU1260|
|Nominal battery voltage|12V|
|Maximum charging current|60A|
|AC input voltage|80–270V AC|
|AC input frequency|40–70Hz|
|Efficiency|90.4%|
|Power factor|0.976 @ 230V|
|Maximum input current|4.6A @ 230V / 9.8A @ 110V|
|Charging outputs|3 isolated outputs|
|Battery profiles|11 preset + 1 custom|
|Lithium support|LiFePO4|
|Cooling|Temperature-controlled fan|
|Protection|High voltage, high temperature and other internal protections|
|Water protection|IP22 when correctly vertically mounted|
|Dimensions|315 × 215 × 90mm|
|Weight|3kg|
|Warranty|5 years|

The manufacturer's published figures give approximately **900W mains power consumption at full 60A output**. ([Sterling Power Products](https://sterling-power.com/products/pro-charge-ultra "Pro Charge Ultra (10A to 60A and 12V, 24V, 32V, 36V, 48V models availa – Sterling Power Products"))

---

## What Does "60A" Actually Mean?

The charger can provide up to **60A to the battery at the charging voltage**.

For example, during a charging stage at approximately 14V:

```text
14V × 60A ≈ 840W
```

The charger therefore needs roughly **900W of AC input power** at maximum output after accounting for losses. ([Sterling Power Products](https://sterling-power.com/products/pro-charge-ultra "Pro Charge Ultra (10A to 60A and 12V, 24V, 32V, 36V, 48V models availa – Sterling Power Products"))

This is worth knowing when designing your 230V system.

A 10A UK campsite hookup can theoretically provide:

```text
230V × 10A = 2300W
```

So the Pro Charge Ultra's ~900W maximum consumption leaves substantial capacity for other appliances.

---

## Three Isolated Outputs

One particularly useful feature is that the PCU1260 has **three isolated charging outputs**.

This allows it to charge multiple battery banks without directly connecting those battery banks together.

For example:

```text
                 ┌──► Starter Battery
                 │
Pro Charge ──────┼──► Leisure Battery Bank
                 │
                 └──► Auxiliary Battery
```

For your ambulance, the most useful arrangement would potentially be:

```text
Output 1 ──► Starter battery
Output 2 ──► Leisure battery bank
Output 3 ──► Spare / auxiliary battery bank
```

If you don't need the additional outputs, they don't have to be used.

---

## Battery Chemistry

The charger has **11 preset charging algorithms**, including profiles for:

- Open lead-acid
    
- Sealed lead-acid
    
- AGM
    
- Gel
    
- Calcium
    
- LiFePO4
    

There is also a **custom profile** where absorption and float voltages can be manually configured. ([Sterling Power Products](https://sterling-power.com/products/pro-charge-ultra "Pro Charge Ultra (10A to 60A and 12V, 24V, 32V, 36V, 48V models availa – Sterling Power Products"))

This makes it considerably more flexible than a basic mains battery charger.

---

## Charging Stages

The charger automatically manages the charging process rather than simply supplying a constant voltage.

The exact behaviour depends on the selected battery profile, but broadly:

```text
Bulk
  │
  ▼
Absorption
  │
  ▼
Float
  │
  ▼
Maintenance
```

This means you can leave the charger connected to the leisure batteries while the ambulance is connected to shore power.

---

## Power Factor Correction

The Pro Charge Ultra has active **Power Factor Correction (PFC)**.

The manufacturer specifies a power factor of approximately **0.976 at 230V** and efficiency of **90.4%** for the 12V/60A model. ([Sterling Power Products](https://sterling-power.com/products/pro-charge-ultra "Pro Charge Ultra (10A to 60A and 12V, 24V, 32V, 36V, 48V models availa – Sterling Power Products"))

This is particularly useful in a camper because the charger makes relatively efficient use of limited shore-power capacity.

---

## Programmable Power Reduction

An excellent feature for van use is the ability to reduce the charger's output to:

- 100%
    
- 75%
    
- 50%
    
- 25%
    

This can be useful when connected to a limited electrical supply.

For example, if you're on a campsite with a weak hookup and simultaneously running other appliances, you could reduce the charger rather than continually tripping the hookup breaker.

---

## Battery Temperature Sensor

The charger includes a **battery temperature sensor**.

This allows charging voltage to be adjusted according to battery temperature and provides additional protection against excessive temperature. ([Sterling Power Products](https://sterling-power.com/products/pro-charge-ultra "Pro Charge Ultra (10A to 60A and 12V, 24V, 32V, 36V, 48V models availa – Sterling Power Products"))

This is particularly useful for lead-acid batteries.

---

## Automatic Battery Maintenance

The Pro Charge Ultra periodically performs a battery-health cycle, including desulphation/equalisation functions where appropriate.

The manufacturer states this occurs approximately every **7–10 days**. ([Sterling Power Products](https://sterling-power.com/products/pro-charge-ultra "Pro Charge Ultra (10A to 60A and 12V, 24V, 32V, 36V, 48V models availa – Sterling Power Products"))

**Important:** this is primarily relevant to compatible lead-acid battery profiles. You should use the appropriate LiFePO4 profile rather than applying lead-acid equalisation behaviour to lithium batteries.

---

## Installation

A simplified installation would be:

```text
             230V AC
                │
          Consumer Unit
                │
          RCD / MCB
                │
                ▼
      Pro Charge Ultra
                │
          DC Fuse/Breaker
                │
                ▼
         DC Busbar
                │
                ▼
       Leisure Batteries
```

The charger should have appropriate AC and DC protection and be installed according to Sterling's instructions.

The **60A DC output should be appropriately fused** close to the battery/DC distribution point.

---

## Integration With Your Ambulance

This is the component that provides **shore-power charging** in your system.

Your overall charging architecture is shaping up roughly like this:

```text
                         ┌── Solar Panels
                         │
                         ▼
                    MPPT Controller
                         │
                         │
                         ▼
Alternator ──► DC-DC ──► Battery Bank ◄── Pro Charge Ultra
                                      ▲
                                      │
                                 230V Shore
```

And then:

```text
Battery Bank
     │
     ├──► Xantrex PROwatt SW 2000i
     │
     ├──► DC Distribution
     │
     └──► Battery Protection / Monitoring
```

So the Pro Charge Ultra is **one of three major charging sources** you're planning:

1. ☀️ **Solar** → Voltanic panels + MPPT
    
2. 🚐 **Engine/alternator** → DC-DC charging
    
3. 🔌 **Shore power** → Sterling Pro Charge Ultra
    

That's a very sensible arrangement for an expedition-style ambulance because you aren't dependent on any single charging method.

---

## Important Consideration: 60A vs Your Batteries

Sterling recommends roughly **10% of battery capacity** as a general starting point for charger sizing, while acknowledging that larger chargers can be appropriate when faster charging is desired. ([Sterling Power Products](https://sterling-power.com/products/pro-charge-ultra "Pro Charge Ultra (10A to 60A and 12V, 24V, 32V, 36V, 48V models availa – Sterling Power Products"))

If your battery bank were around **230Ah**, for example:

```text
230Ah × 10% ≈ 23A
```

A 60A charger would therefore be a relatively aggressive charging rate for a conventional lead-acid bank.

However, your charger can be operated at reduced power, and the appropriate maximum charging current ultimately depends on the **specific batteries you're using**.

This will become particularly important if you retain the **Lucas LSLC125-12 and Fullriver DC115-12** batteries you've previously selected.

---

## Advantages

✅ 60A charging capability  
✅ Very flexible battery chemistry settings  
✅ LiFePO4 support  
✅ Three isolated outputs  
✅ Excellent efficiency  
✅ Power-factor correction  
✅ Adjustable charging power  
✅ Battery temperature compensation  
✅ Automatic battery maintenance  
✅ 80–270V global AC input  
✅ Compact for its power  
✅ 5-year warranty

---

## Limitations

❌ Relatively expensive compared with basic mains chargers  
❌ Fan-cooled, so it isn't completely silent  
❌ IP22 rather than fully waterproof  
❌ 60A may be excessive for a small lead-acid battery bank  
❌ Requires proper AC and DC protection  
❌ The three outputs don't mean you get 60A **per output** — the charger is a 60A unit overall

---

## Build Notes

### Recommended location

Mount it somewhere:

- Dry
    
- Well ventilated
    
- Accessible for configuration
    
- Close enough to the batteries to minimise DC cable length
    
- Away from direct water exposure
    

The IP22 rating is based on correct vertical mounting and drip protection, so **don't treat this as a waterproof charger**. ([Sterling Power Products](https://sterling-power.com/products/pro-charge-ultra "Pro Charge Ultra (10A to 60A and 12V, 24V, 32V, 36V, 48V models availa – Sterling Power Products"))

### Particularly useful feature for the ambulance

The adjustable power reduction is probably one of the most useful features for your build.

It means you can have:

**Full 60A charging when connected to a good shore supply**

but reduce it when:

**Sharing a limited campsite hookup with the inverter/other appliances.**

---

## My Assessment

**Very good choice for your electrical system.**

It is arguably more charger than you need if you only intend to occasionally plug the ambulance into mains, but the flexibility is valuable in a full conversion.

The **three isolated outputs, LiFePO4 support, temperature sensing, adjustable power and good efficiency** make it particularly well suited to a complicated multi-source camper electrical system.

The main thing I would revisit later is whether **60A is the correct charging rate for your final battery bank**. I would determine this once we've established the final battery chemistry and total Ah capacity rather than changing the charger now.

---


## References

- Sterling Power — Pro Charge Ultra  
    [Official product page](https://sterling-power.com/products/pro-charge-ultra)
    
- Sterling Power — Pro Charge Ultra technical specifications and manuals  
    [Technical information / downloads](https://sterling-power.com/products/pro-charge-ultra)

## Related

- [[Electrics Overview]]
- [[Fullriver DC115-12 AGM Deep-Cycle Leisure Battery]]
- [[Lucas LSLC125-12 AGM Leisure Battery]]
- [[Xantrex PROwatt SW 2000i Inverter]]
- [[Dashboard]]
