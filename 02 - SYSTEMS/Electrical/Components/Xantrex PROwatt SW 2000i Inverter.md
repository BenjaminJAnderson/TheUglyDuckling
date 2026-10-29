---
tags: [systems, electrical, inverter]
status: research
updated: 2026-10-21
---

# Xantrex PROwatt SW 2000i Inverter

**Category:** DC → AC Power Inverter  
**Manufacturer:** Xantrex  
**Model:** PROwatt SW 2000i  
**Type:** Pure Sine Wave Inverter

## Purpose
The Xantrex PROwatt SW 2000i converts **12V DC battery power into 230V AC mains power** suitable for running household appliances inside a camper conversion.

It produces a **pure sine wave output**, meaning the AC waveform closely matches grid electricity. This makes it suitable for sensitive electronics such as:

- Laptops
- Phone chargers
- Camera equipment
- TVs
- Audio equipment
- Medical equipment
- Induction loads (within power limits)

It is designed for mobile applications such as:

- Campervans
- Boats
- Off-grid cabins
- Emergency power systems

---

## Key Specifications

|Specification|Value|
|---|---|
|Model|PROwatt SW 2000i|
|Output power (continuous)|2000W|
|Surge power|3000W (5 seconds)|
|Input voltage|12V DC|
|Output voltage|230V AC|
|Output waveform|Pure sine wave|
|Output frequency|50Hz|
|Maximum efficiency|~90%|
|No-load current draw|~0.8A|
|Low voltage shutdown|~10.5V|
|High voltage shutdown|~15.5V|
|AC outlets|2 × UK style sockets|
|USB output|2.1A USB port|
|Remote switch capability|Yes|
|Cooling|Temperature-controlled fan|
|Protection|Overload, short circuit, over-temperature, low/high voltage|
|Weight|~4.2kg|
|Dimensions|355 × 165 × 71mm|

---

## How It Works

Basic operation:

```
Leisure Battery (12V DC)
          |
          |
     High Current DC
          |
          |
 Xantrex PROwatt SW 2000i
          |
          |
     230V AC Output
          |
          |
 Household Appliances
```

The inverter uses electronic switching circuits to:

1. Convert 12V DC into high-frequency AC
2. Increase voltage using transformers
3. Reconstruct a clean 50Hz sine wave output

---

## Power Requirements

A 2000W inverter can draw significant current from a 12V battery system.

Approximate current draw:

```
Current = Power ÷ Voltage

2000W ÷ 12V ≈ 167A
```

Accounting for inverter losses:

**Real-world maximum current draw: ~180A**

This means it requires:

- Large battery cables
- Proper fusing
- Short cable runs
- High-capacity battery bank

Recommended cable size:

|Cable length|Recommended cable|
|---|---|
|<1m|50mm² minimum|
|1–2m|70mm² preferred|

Recommended fuse:

**200–250A Class T or ANL fuse**

---

## Battery Requirements

A 2000W inverter is demanding on a battery.

Example:

## Lead Acid

A typical 115Ah leisure battery:

```
115Ah × 12V ≈ 1380Wh
```

However, only ~50% should be used:

```
≈690Wh usable
```

Running a 2000W load:

```
690Wh ÷ 2000W ≈ 20 minutes
```

before reaching recommended discharge limits.

---

## Lithium (LiFePO4)

A lithium bank is much better suited.

Example:

```
200Ah × 12.8V ≈ 2560Wh
```

Usable energy:

```
≈2300Wh
```

A 2000W load could theoretically run:

```
2300Wh ÷ 2000W ≈ 1 hour
```

---

## Suitable Loads

## Good Uses

✅ Laptop charging  
✅ Camera equipment  
✅ Power tools (within limits)  
✅ Kitchen appliances  
✅ Small microwave  
✅ TV/projector  
✅ Audio equipment  
✅ Battery chargers

---

## Potentially Problematic Loads

⚠️ High startup current devices:

- Fridges with compressors
- Motors
- Pumps
- Air compressors
- Large power tools

Although the inverter has a 3000W surge rating, some motors can briefly exceed this.

---

## Integration Into Ambulance Conversion

Likely wiring:

```
Battery Bank
      |
      |
  Main Fuse
      |
      |
Battery Isolation Switch
      |
      |
Xantrex PROwatt SW 2000i
      |
      |
230V Consumer Unit
      |
      |
Sockets
```

The inverter should have:

- Dedicated battery cables
- Dedicated fuse
- Physical isolation switch
- Ventilation around cooling fans

---

## Relationship To Existing Components

Current planned system:

- Leisure batteries:
    - Lucas LSLC125-12
    - Fullriver DC115-12
- Charger:
    - Pro Charge Ultra 12V-60A
- Solar:
    - 4 × Voltanic 200W panels
    - Voltanic 60A MPPT

The Xantrex is likely to be the **largest electrical load in the van**.

Important consideration:

The existing lead-acid batteries are relatively small for a 2000W inverter. The inverter can handle the power, but the batteries and cabling will determine real-world performance.

A future upgrade to:

- 200–400Ah LiFePO4
- Larger DC busbars
- Proper high-current distribution

would better match this inverter.

---

## Advantages

✅ Pure sine wave output  
✅ Can run sensitive electronics  
✅ Good surge capability  
✅ Reliable brand reputation  
✅ Built-in protection systems  
✅ Remote switching available  
✅ Suitable for full camper electrical systems

---

## Limitations

❌ Large DC current requirements  
❌ Inefficient for small loads (USB charging etc.)  
❌ Requires expensive cabling and fusing  
❌ 12V system limits practical power  
❌ Overkill for many small appliances

---

## Build Notes

Recommended usage strategy:

Use the inverter for:

- Occasional high-power appliances
- Tools
- Kitchen equipment
- Electronics

Avoid leaving it permanently powered on because the standby consumption will slowly drain the batteries.

For everyday loads:

- USB chargers
- LED lights
- Fans
- Pumps

use direct 12V circuits instead.

---


## References

- [Xantrex PROwatt SW Series Product Page](https://xantrex.com/products/inverters/prowattswi/)

## Related

- [[Electrics Overview]]
- [[Sterling Power Pro Charge Ultra 12V 60A]]
- [[Victron Energy Battery Protect 12-24V 65A (BP-65)]]
- [[Fullriver DC115-12 AGM Deep-Cycle Leisure Battery]]
- [[Lucas LSLC125-12 AGM Leisure Battery]]
- [[Dashboard]]
