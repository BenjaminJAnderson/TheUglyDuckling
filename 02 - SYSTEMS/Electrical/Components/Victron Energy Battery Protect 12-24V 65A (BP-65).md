---
tags: [systems, electrical, battery-protection]
status: research
updated: 2026-10-21
---

# Victron Energy Battery Protect 12-24V 65A (BP-65)

**Category:** DC Battery Protection / Low Voltage Disconnect  
**Manufacturer:** Victron Energy  
**Model:** BatteryProtect BP-65  
**Product page:** [Victron BatteryProtect 12/24V 65A](https://www.splitcharge.co.uk/product/victron-energy-battery-protect-12-24v-65a/)

## Purpose
The Victron BatteryProtect is an automatic **low-voltage disconnect switch** designed to prevent batteries from being discharged too deeply.

It sits between the leisure battery and non-essential DC loads. If battery voltage drops below a programmed threshold, it disconnects the loads before the battery becomes damaged.

It can also be used as a remotely controlled **master DC switch**.

Typical uses:
- Protecting leisure batteries from over-discharge
- Disconnecting DC loads when the battery is low
- Preventing lithium batteries being damaged by excessive discharge
- Acting as an electronically controlled isolation switch


---

## Key Specifications

|Specification|Value|
|---|---|
|Model|BP-65|
|Nominal voltage|12V / 24V automatic detection|
|Continuous current rating|65A|
|Peak current (30 seconds)|250A|
|Operating voltage range|6–35V DC|
|Current consumption (on)|1.5mA|
|Current consumption (off)|0.6mA|
|Switching method|MOSFET (no mechanical relay)|
|Protection type|Low voltage disconnect|
|Alarm output|Yes|
|Alarm output maximum current|50mA|
|Connection terminals|M6 studs|
|Weight|0.2kg|
|Dimensions|40 × 48 × 106mm|
|Protection rating|Electronics IP67 (potted), terminals IP00|
|Operating temperature|-40°C to +40°C at full load|

---

## How It Works

```
Battery Positive
      |
      |
BatteryProtect
      |
      |
DC Loads
      |
Battery Negative
```

The BatteryProtect monitors battery voltage.

Example with a 12V lead-acid system:

- Battery healthy → loads connected
- Battery voltage drops → warning/alarm output activated
- Voltage remains low → loads disconnected
- Battery recharged → loads automatically reconnect

Default thresholds:

|System|Disconnect|Reconnect|
|---|---|---|
|12V|10.5V|12V|
|24V|21V|24V|

The thresholds can be programmed to suit different battery chemistries.

---
## Lithium Battery Compatibility

The BatteryProtect has a dedicated lithium mode.

Important because lithium batteries have a very flat discharge curve and can be damaged if discharged too far.

It can also accept an external control signal from a Battery Management System (BMS), allowing the BMS to disconnect loads.

---
## Installation Notes

## Correct placement

Recommended:

```
Battery +
   |
 Fuse
   |
BatteryProtect
   |
DC Distribution Bus
   |
Loads
```

The BatteryProtect should **not** normally be used between the battery and charging sources.

Examples:

✅ Good:

- Battery → BatteryProtect → lights
- Battery → BatteryProtect → fridge
- Battery → BatteryProtect → DC fuse panel

❌ Avoid:

- Solar controller → BatteryProtect → battery
- Alternator charger → BatteryProtect → battery

The device only allows current flow from the **Battery terminal to Load terminal** and is not designed for reverse charging currents.

---

## Suitability For Fiat Ducato Ambulance Conversion

## Possible uses

Good candidates:

- Interior lighting circuits
    
- Water pumps
    
- USB outlets
    
- Fans
    
- Compressor fridge
    
- Small DC appliances
    

Less suitable:

- Large inverter
    
- High-current DC heaters
    
- Large compressors
    

The 65A rating means:

At 12V:

```
65A × 12V ≈ 780W maximum DC load
```

However, it is better not to run continuously at the maximum rating. For a camper electrical system, keeping normal loads below ~40–50A gives more reliability.

---

## Integration With My System

Current planned electrical system:

- 12V leisure batteries
    
- Xantrex inverter
    
- Solar charging
    
- Shore charging
    
- DC distribution
    

Potential placement:

```
Leisure Battery Bank
        |
      Fuse
        |
Victron BatteryProtect 65A
        |
   DC Fuse Box
        |
 Lights
 Fridge
 Pumps
 Fans
 USB
```

Large loads should bypass it:

```
Battery
 |
 Main Fuse
 |
 +---------------- Inverter
 |
 +---------------- DC Charger
 |
 +---------------- BatteryProtect → DC Loads
```

---

## Advantages

✅ Very low standby consumption  
✅ No mechanical relay to fail  
✅ Spark-free MOSFET switching  
✅ Works with 12V and 24V systems  
✅ Lithium compatible  
✅ Programmable disconnect levels  
✅ Compact size  
✅ Victron ecosystem compatibility

---
## Limitations

❌ No built-in current monitoring  
❌ No Bluetooth/app monitoring (unlike Smart BatteryProtect)  
❌ 65A may be limiting for larger van systems  
❌ Cannot replace proper fusing  
❌ Not a battery monitor — it only measures voltage

---
## Related Components

Often paired with:
- **Victron SmartShunt** → monitors battery state of charge/current flow
- **Victron Lynx Distributor** → fused DC distribution
- **Victron MPPT Solar Controller** → solar charging
- **Victron Orion DC-DC Charger** → alternator charging

---

## Decision Notes For Build

**Do I need this component?**

For a simple van electrical system: **yes, it is a sensible safety component.**

For a larger ambulance conversion with:

- 2000W inverter
- high capacity lithium bank
- large DC loads

I would consider using a **larger BatteryProtect (100A/220A)** or a properly designed fused distribution system instead.

For the current planned system, this is best used as a **protected DC loads disconnect**, not as the main battery isolation device.

---

## References

- [Victron BatteryProtect datasheet](https://www.victronenergy.com/upload/documents/Datasheet-Battery-Protect-65-A--100-A--220-A-EN-.pdf)
- [Victron Smart BatteryProtect manual](https://www.victronenergy.com/upload/documents/BatteryProtect_12V_24V/114439-Smart_BatteryProtect-pdf-en.pdf)
- [Victron BatteryProtect product page](https://www.victronenergy.jp/battery_protect/battery-protect)

## Related

- [[Electrics Overview]]
- [[Xantrex PROwatt SW 2000i Inverter]]
- [[Fullriver DC115-12 AGM Deep-Cycle Leisure Battery]]
- [[Lucas LSLC125-12 AGM Leisure Battery]]
- [[Dashboard]]