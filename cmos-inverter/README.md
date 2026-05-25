# Project Overview

A CMOS inverter is one of the most fundamental building blocks in digital integrated circuits.

The circuit uses:
- PMOS transistor as pull-up network
- NMOS transistor as pull-down network

The output becomes the logical inverse of the input signal.

---

# CMOS Inverter Operation

## Input LOW (0)
- PMOS turns ON
- NMOS turns OFF
- Output connected to VDD
- Output = HIGH (1)

## Input HIGH (1)
- PMOS turns OFF
- NMOS turns ON
- Output connected to GND
- Output = LOW (0)

---

# Truth Table

| Input | Output |
|------|------|
| 0 | 1 |
| 1 | 0 |

---

# LTspice Simulation

The circuit was simulated in LTspice using transient analysis to observe:
- input waveform behavior
- output inversion
- switching response
- rise and fall transitions

---

# Files Included

## `/schematics`
LTspice schematic files for the CMOS inverter simulation.

## `/images`
Simulation screenshots including:
- schematic diagram
- transient waveforms

---

# Tools Used

- LTspice

---

# Future Improvements

- CMOS NAND gate simulation
- Propagation delay analysis
- Basic layout exploration
- Additional digital logic simulations
