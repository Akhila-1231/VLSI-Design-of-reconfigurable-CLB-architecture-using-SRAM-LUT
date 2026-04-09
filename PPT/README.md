# 🔷 Design of Reconfigurable CLB Architecture using SRAM-LUT

## Overview

This project focuses on the design and analysis of a **Reconfigurable Configurable Logic Block (CLB)** using **SRAM-based Look-Up Tables (LUTs)**, which are the fundamental building elements of modern **Field Programmable Gate Arrays (FPGAs)**.

The architecture enables flexible implementation of digital logic functions by storing truth table values in SRAM, allowing dynamic reconfiguration without modifying hardware.

---

## Objectives

* To design a **CLB architecture using SRAM-based LUT**
* To understand the working of LUT as a programmable logic element
* To analyze **reconfigurability in FPGA systems**
* To evaluate performance in terms of **area, delay, and power**

---

## Key Concepts

### Configurable Logic Block (CLB)

A CLB is the core unit of an FPGA that can implement both **combinational and sequential logic** using:

* LUTs (Look-Up Tables)
* Flip-Flops
* Multiplexers

---

###  SRAM-based LUT

A **Look-Up Table (LUT)** is a memory block that stores output values for all input combinations.

* For an n-input LUT → requires **2ⁿ memory cells**
* Inputs act as **address lines**
* Stored values represent the **truth table**

---

###  Reconfigurability

The functionality of the CLB can be changed by updating the SRAM contents:

* No hardware modification required
* Enables rapid prototyping and flexibility

---

## Architecture

###  Components:

* SRAM cells (store logic values)
* Multiplexer (selects output)
* Input lines (address signals)
* Flip-Flop (optional for sequential logic)

### Working:

1. Inputs are applied as address signals
2. Corresponding SRAM location is selected
3. MUX outputs the stored value
4. Output can be registered using flip-flops

---

## Example

For a 2-input function:
F(A, B) = A AND B

| A | B | Output |
| - | - | ------ |
| 0 | 0 | 0      |
| 0 | 1 | 0      |
| 1 | 0 | 0      |
| 1 | 1 | 1      |

Stored in LUT as: `0001`

---

## Features

* ✔️ High flexibility and reusability
* ✔️ Fast reconfiguration
* ✔️ Supports complex logic functions
* ✔️ Suitable for FPGA-based designs

---

## Limitations

* ❌ Memory requirement increases exponentially (2ⁿ)
* ❌ Power consumption due to SRAM usage
* ❌ Delay introduced by multiplexers

---

## Applications

* FPGA design and prototyping
* Digital system implementation
* Signal processing
* Embedded systems
* AI and hardware acceleration

---

## References

1. FPGA Architecture Documentation (Xilinx/Intel)
2. Research papers on SRAM-based LUT design
3. IEEE journals on low-power FPGA architectures
4. Digital Design textbooks

---



## Future Work

* Implementation using **Verilog/VHDL**
* Simulation using **Vivado/ModelSim**
* Power and delay optimization techniques
* Integration with larger FPGA systems

---

