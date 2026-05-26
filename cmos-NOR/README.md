# CMOS NOR Gate Simulation

Introduction to CMOS NOR gate operation using transistor-level simulation in LTspice.

---

# Project Overview

A CMOS NOR gate is a fundamental digital logic gate widely used in integrated circuit design.

The circuit uses:
- PMOS pull-up network
- NMOS pull-down network

The output becomes HIGH only when both inputs are LOW.

---

# CMOS NOR Gate Operation

## Input A = 0 V, Input B = 0 V
- PMOS network ON
- NMOS network OFF
- Output ≈ 10 V

## Input A = 0 V, Input B = 10 V
- PMOS network partially OFF
- NMOS network partially ON
- Output ≈ 0 V

## Input A = 10 V, Input B = 0 V
- PMOS network partially OFF
- NMOS network partially ON
- Output ≈ 0 V

## Input A = 10 V, Input B = 10 V
- PMOS network OFF
- NMOS network ON
- Output ≈ 0 V

---

# Truth Table

| A | B | Output |
|---|---|---|
| 0 V | 0 V | 10 V |
| 0 V | 10 V | 0 V |
| 10 V | 0 V | 0 V |
| 10 V | 10 V | 0 V |

---

# CMOS Network Structure

## PMOS Network
- PMOS transistors connected in series
- Pulls output HIGH only when both inputs are LOW

## NMOS Network
- NMOS transistors connected in parallel
- Pulls output LOW when at least one input is HIGH

---

# LTspice Simulation

The circuit was simulated using transient analysis to observe:
- logic switching behavior
- multi-input waveform interaction
- CMOS pull-up and pull-down network operation

---

# Supply Voltage

For this simulation:

```text
VDD = 10 V
```

Input signals switch between:

```text
LOW = 0 V
HIGH = 10 V
```

---

# Files Included

## `/schematics`
LTspice schematic files for the CMOS NOR gate simulation.

## `/images`
Simulation screenshots including:
- transistor-level schematic
- transient waveforms
- logic behavior visualization
- 
---

# Tools Used

- LTspice
