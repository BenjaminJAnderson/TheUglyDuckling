**Category:** Leisure / Auxiliary Battery  
**Manufacturer:** Lucas  
**Model:** LSLC125-12  
**Battery chemistry:** AGM (Absorbent Glass Mat) lead-acid  
**Nominal voltage:** 12V  
**Capacity:** 125Ah

## Purpose

The Lucas LSLC125-12 is a **12V AGM deep-cycle leisure battery** intended for supplying power to auxiliary electrical systems such as those found in caravans, motorhomes and boats.

In your ambulance conversion, this is part of the **12V leisure battery bank** that stores energy from:

- Solar panels
    
- Alternator/DC-DC charging
    
- 230V mains charging
    

It then supplies your:

- 12V DC appliances
    
- Inverter
    
- Lighting
    
- Pumps
    
- Fridge
    
- Other auxiliary equipment
    

---

# Key Specifications

| Specification   | Value                                                 |
| --------------- | ----------------------------------------------------- |
| Model           | LSLC125-12                                            |
| Manufacturer    | Lucas                                                 |
| Battery type    | AGM                                                   |
| Chemistry       | Lead-acid                                             |
| Nominal voltage | 12V                                                   |
| Capacity        | 125Ah                                                 |
| Energy capacity | ~1,500Wh                                              |
| Terminal type   | TBC — verify on supplied battery                      |
| Maintenance     | Maintenance-free                                      |
| Recommended use | Leisure / deep-cycle                                  |
| Charging        | Suitable for regulated 12V lead-acid charging systems |

**Energy calculation:**

```text
12V × 125Ah = 1,500Wh
```

So the battery contains approximately **1.5kWh of nominal stored energy**.

However, you should not treat all 1,500Wh as practically usable.

---

# Usable Capacity

Because this is a lead-acid AGM battery, regularly discharging it to 0% is undesirable.

A sensible design target is approximately **50% depth of discharge** for good battery life.

```text
125Ah × 50% ≈ 62.5Ah usable
```

Therefore:

```text
12V × 62.5Ah ≈ 750Wh usable
```

A useful way to think about it is:

> **125Ah nominal → roughly 60–65Ah of routinely usable capacity**

The exact usable capacity will depend on discharge rate, temperature and the manufacturer's specified cycle-life limits.

---

# What Is AGM?

AGM stands for **Absorbent Glass Mat**.

Instead of having liquid electrolyte freely moving around inside the battery, the electrolyte is absorbed into a fibreglass mat between the plates.

This gives AGM batteries several advantages over conventional flooded lead-acid batteries:

- No topping-up with water
    
- Much lower risk of electrolyte leakage
    
- Can tolerate vibration well
    
- Lower internal resistance
    
- Can provide relatively high current
    
- Can accept relatively high charging currents
    
- Can be mounted in various orientations, subject to manufacturer restrictions
    

It is still fundamentally a **lead-acid battery**, however, and therefore has many of the same limitations around deep discharge and weight.

---

# Weight vs Energy

One of the major disadvantages of this battery chemistry is its energy density.

A 125Ah 12V AGM battery stores approximately:

```text
1.5kWh
```

but a substantial proportion of that energy isn't practically usable if you want good cycle life.

This makes AGM considerably less space-efficient than LiFePO4.

---

# Running Your Inverter

This is particularly important for your **Xantrex PROwatt SW 2000i**.

At a 2,000W load, ignoring losses:

```text
2,000W ÷ 12V ≈ 167A
```

In reality the battery would probably supply around **180A+** once inverter losses and voltage drop are considered.

That is an enormous current for a 125Ah lead-acid battery.

If you attempted to run the inverter at full power:

```text
125Ah ÷ ~180A ≈ 0.7 hours
```

but this calculation is misleading because:

1. You shouldn't fully discharge the AGM.
    
2. Lead-acid capacity decreases at high discharge rates.
    
3. Battery voltage will sag significantly.
    
4. The inverter may shut down due to low voltage.
    

So **a single LSLC125-12 is not a good battery for sustained 2kW inverter loads.**

---

# Your Proposed Battery Bank

You previously selected:

- Lucas LSLC125-12
    
- Fullriver DC115-12
    

If these are intended to form one battery bank, **I would not recommend simply connecting the two different batteries in parallel.**

They have different:

- Capacities
    
- Manufacturers
    
- Internal resistances
    
- Charging characteristics
    
- Age/history (if not purchased simultaneously)
    

Parallel battery banks work best when the batteries are:

> **Identical model + identical capacity + identical age + identical condition.**

For your build, I would strongly prefer either:

### Option A — Two identical LSLC125-12

```text
125Ah + 125Ah
       ↓
250Ah @ 12V
```

or

### Option B — Two identical Fullriver batteries

depending on the final battery-bank design.

---

# Charging

Your **Sterling Pro Charge Ultra 12V-60A** can supply up to 60A.

For a single 125Ah AGM battery:

```text
60A ÷ 125Ah ≈ 0.48C
```

That's a relatively high charging rate for a conventional AGM battery.

It may be acceptable depending on the exact manufacturer's charging specification, but **I would not assume that 60A is appropriate without checking the LSLC125-12's datasheet.**

If you had two identical 125Ah batteries in parallel:

```text
250Ah bank
60A ÷ 250Ah = 0.24C
```

which is considerably more reasonable.

This is one reason your final battery-bank capacity matters when configuring the Sterling charger.

---

# Solar Charging

Your planned solar system is:

**4 × 200W panels = 800W**

At ~14V charging voltage:

```text
800W ÷ 14V ≈ 57A
```

So your solar system could theoretically provide **roughly 57A of charging current** under ideal conditions.

This is another reason why the battery bank needs to be sufficiently large.

A single 125Ah AGM battery potentially receiving ~57A from solar alone would be undergoing a very high charging rate.

A 250Ah bank would be much more comfortable:

```text
57A ÷ 250Ah ≈ 0.23C
```

---

# Important Compatibility Issue

Your proposed charging system could potentially deliver approximately:

- **60A from mains**
    
- ~**57A from solar**
    
- Additional current from alternator/DC-DC charging
    

You therefore need to make sure the **final battery bank is designed around the maximum possible charging current**.

You don't necessarily add all charging sources together in normal operation, but they can potentially operate simultaneously.

This is something we should account for when we eventually design the complete electrical system.

---

# Advantages

✅ AGM is maintenance-free  
✅ Good vibration resistance  
✅ Good high-current capability  
✅ No regular electrolyte maintenance  
✅ Suitable for camper/vehicle applications  
✅ More tolerant of rough conditions than flooded batteries  
✅ Can provide substantial short-term current  
✅ Relatively inexpensive compared with lithium

---

# Limitations

❌ Heavy  
❌ Low usable energy compared with LiFePO4  
❌ Shouldn't routinely be deeply discharged  
❌ Significant voltage sag under high loads  
❌ Reduced capacity at high discharge rates  
❌ Requires careful charging  
❌ Shorter cycle life than LiFePO4 when deeply cycled  
❌ 125Ah is relatively small for your planned 2kW inverter + 800W solar system

---

# Ambulance Build Assessment

### As a single battery:

**⚠️ Too small for your planned system.**

125Ah AGM is perfectly reasonable for a modest camper electrical system, but your planned system is considerably more substantial.

You have:

```text
800W Solar
      +
60A Mains Charger
      +
2,000W Inverter
```

That's a fairly serious electrical system for a single 125Ah AGM.

### As part of a larger bank:

**👍 Much more sensible.**

I'd aim for at least **250Ah of matched AGM** if you're committed to lead-acid.

However, before buying multiple AGM batteries, I'd seriously consider whether **LiFePO4 makes more sense for the ambulance**, especially given your large solar array and 2kW inverter.

---

# Important Note About The Exact Battery

The Go Batteries product page gives the basic product information, but I would like to get the **manufacturer's actual LSLC125-12 technical datasheet** before treating things such as:

- Maximum charging current
    
- Recommended float voltage
    
- Absorption voltage
    
- Cycle life
    
- Maximum continuous discharge current
    
- Temperature compensation
    
- Terminal specifications
    

as confirmed specifications.

Those figures are important enough that I don't want to invent them or assume generic AGM values.

---

# Obsidian Tags

`#Electrical` `#Battery` `#AGM` `#LeadAcid` `#12VSystem` `#Lucas` `#LeisureBattery`

# References

- Go Batteries — Lucas LSLC125-12 AGM 12V 125Ah  
    [Product page](https://www.gobatteries.co.uk/product/battery-types/leisure-batteries/caravan/lslc125-12-lucas-agm-battery-12v-125ah/?utm_source=chatgpt.com)
    
- Sterling Power — Pro Charge Ultra  
    [Pro Charge Ultra product page](https://sterling-power.com/products/pro-charge-ultra?utm_source=chatgpt.com)
    
- Xantrex — PROwatt SW  
    [PROwatt SW product page](https://xantrex.com/products/inverters/prowattswi/?utm_source=chatgpt.com)