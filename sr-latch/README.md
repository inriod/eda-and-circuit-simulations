# SR Latch Simulation

Introduction to SR latch operation using transistor-level CMOS logic simulation in LTspice.

This project explores sequential logic concepts including feedback-based state retention, memory behavior, and introductory digital storage mechanisms used in integrated circuits.

---

# Project Overview

An SR (Set-Reset) latch is one of the most fundamental sequential logic circuits used in digital systems.

Unlike combinational logic gates, the SR latch can store a previous logic state using feedback connections between logic gates.

This project was implemented using cross-coupled CMOS NOR gates.

---

# Sequential Logic Concept

Combinational logic depends only on current inputs.

Sequential logic depends on:
- current inputs
- previous circuit state

The SR latch introduces:
- memory behavior
- feedback loops
- state retention

which are foundational concepts in digital IC design.

---

# SR Latch Operation

## Set State

```text
S = HIGH
R = LOW
```

Result:
```text
Q = HIGH
```

The latch stores a logic HIGH state.

---

## Reset State

```text
S = LOW
R = HIGH
```

Result:
```text
Q = LOW
```

The latch stores a logic LOW state.

---

## Hold State

```text
S = LOW
R = LOW
```

Result:
```text
Previous state is preserved
```

The circuit remembers its last stored value.

---

## Invalid State

```text
S = HIGH
R = HIGH
```

This condition creates an invalid or unstable state for a NOR-based SR latch.

---

# Truth Table

| S | R | Q(next) |
|---|---|---|
| 0 V | 0 V | Hold Previous State |
| 5 V | 0 V | Set |
| 0 V | 5 V | Reset |
| 5 V | 5 V | Invalid |

---

# LTspice Simulation

The circuit was simulated using transient analysis to observe:
- latch state transitions
- feedback behavior
- memory retention
- sequential logic operation

---

# Supply Voltage

For this simulation:

```text
VDD = 5 V
```

Input signals switch between:

```text
LOW = 0 V
HIGH = 5 V
```

---

# Key Learnings

- Sequential logic fundamentals
- Feedback-based state retention
- Basic digital memory concepts
- CMOS latch behavior
- Transient waveform analysis
- Introductory custom IC workflow concepts

---

# Files Included

## `/schematics`
LTspice schematic files for the SR latch simulation.

## `/images`
Simulation screenshots including:
- transistor-level schematic
- transient waveforms
- feedback behavior visualization
- hardware assembly diagram


---

# Tools Used

- LTspice
- Arduino

---

# Future Improvements

- D latch implementation
- D flip-flop design
- Clocked sequential logic
- Timing analysis exploration
- FSM-oriented CMOS logic design
