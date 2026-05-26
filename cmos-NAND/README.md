# CMOS NAND Gate Simulation

Introduction to CMOS NAND gate operation using transistor-level simulation in LTspice.

---

# Project Overview

A CMOS NAND gate is one of the most important digital logic gates used in integrated circuits.

The circuit uses:
- PMOS pull-up network
- NMOS pull-down network

The output becomes LOW only when both inputs are HIGH.

---

# CMOS NAND Gate Operation

## Input A = 0, Input B = 0
- PMOS network ON
- NMOS network OFF
- Output ≈ 10 V

## Input A = 0, Input B = 10 V
- PMOS network partially ON
- NMOS network partially OFF
- Output ≈ 10 V

## Input A = 10 V, Input B = 0
- PMOS network partially ON
- NMOS network partially OFF
- Output ≈ 10 V

## Input A = 10 V, Input B = 10 V
- PMOS network OFF
- NMOS network ON
- Output ≈ 0 V

---

# Truth Table

| A | B | Output |
|---|---|---|
| 0 V | 0 V | 10 V |
| 0 V | 10 V | 10 V |
| 10 V | 0 V | 10 V |
| 10 V | 10 V | 0 V |

---

# CMOS Network Structure

## PMOS Network
- PMOS transistors connected in parallel
- Pulls output HIGH when at least one input is LOW

## NMOS Network
- NMOS transistors connected in series
- Pulls output LOW only when both inputs are HIGH

---

# LTspice Simulation

The circuit was simulated using transient analysis to observe:
- logic switching behavior
- multi-input waveform interaction

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
LTspice schematic files for the CMOS NAND gate simulation.

## `/images`
Simulation screenshots including:
- transistor-level schematic
- logic behavior visualization

---

# Tools Used

- LTspice
