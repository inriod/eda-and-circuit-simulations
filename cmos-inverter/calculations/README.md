# CMOS Inverter Calculation Notes

## Supply Voltage

For this simulation:

```text
VDD = 10 V
```

The input signal switches between:

```text
LOW = 0 V
HIGH = 10 V
```

The inverter output ideally switches between:

```text
LOW ≈ 0 V
HIGH ≈ 10 V
```

---

## Logic Behavior

| Input Voltage | PMOS | NMOS | Output |
|---|---|---|---|
| 0 V | ON | OFF | HIGH ≈ 10 V |
| 10 V | OFF | ON | LOW ≈ 0 V |

---

## 50% Switching Point

For `VDD = 10 V`, the approximate switching midpoint is:

```text
50% point = VDD / 2 = 5 V
```

In LTspice, propagation delay can be estimated by comparing:
- when the input crosses 5 V
- when the output crosses 5 V

---

## Propagation Delay Concept

```text
tPLH = delay when output goes from LOW to HIGH
tPHL = delay when output goes from HIGH to LOW

tpd = (tPLH + tPHL) / 2
```

Propagation delay represents the time difference between an input transition and the corresponding output response.

---

## What Affects Delay?

CMOS inverter delay depends on:
- transistor size
- load capacitance
- supply voltage
- PMOS/NMOS drive strength
- input transition speed

---

## Key Learning

A CMOS inverter outputs the logical inverse of the input signal.

With a 10 V supply:
- LOW input produces HIGH output
- HIGH input produces LOW output

Real transistor circuits do not switch instantly due to capacitance and transistor switching behavior.
