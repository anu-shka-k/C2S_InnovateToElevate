# C2S_InnovateToElevate : 4-bit Arithmetic Logic Unit (ALU)

## Project Overview

This project implements a **4-bit Arithmetic Logic Unit (ALU)** designed and verified at the CMOS transistor level using **Cadence Virtuoso** and **Cadence Spectre** simulation tools (45 nm technology node). The ALU integrates multiple arithmetic and logic sub-units — Adder, Subtractor, Multiplier, Divider, and basic logic gates — and selects outputs using a 16:1 multiplexer (MUX). Each sub-unit accepts two 4-bit inputs and produces an 8-bit output (via a Parallel-In Serial-Out / PISO converter) to the MUX for operation selection and verification.

---

## Objectives

* To understand CMOS-level implementation of basic logic gates
* To design arithmetic and logical circuits using CMOS technology
* To integrate these circuits into a 4-bit ALU
* To verify the functionality of the ALU using simulation

---

## ALU Components

The ALU is designed using the following sub-blocks:

* Basic logic gates : AND, OR, NAND, NOR, XOR, XNOR, NOT (implemented via NAND primitives)
* 4-bit Adder
* 4-bit Subtractor
* 4-bit Multiplier
* 4-bit Divider
* Multiplexer for operation selection

Each block is designed at the transistor level and verified individually before integration.

---

## Design Methodology

* CMOS-level schematic design of individual logic gates
* Construction of arithmetic circuits using these logic gates
* Integration of all arithmetic and logic blocks into a single ALU architecture
* Simulation and verification using Cadence tools

---

## Verification & Test Strategy

* Truth-table verification: Each sub-unit was validated against the truth tables for all relevant 4-bit input combinations.
* Waveform inspection: The testbench toggles select lines every 8 clock cycles to observe the serialized 8-bit output in Spectre waveforms.
* Sample test case: A = 1011, B = 0101 was used to demonstrate and capture sample outputs for the full set of operations.

## Outcome

The final outcome of the project is a fully functional and verified 4-bit ALU designed from scratch at the CMOS level, demonstrating correct arithmetic and logical operations through simulation results.

---

## Academic Context

This project was carried out as part of a **two-month internship**, with an emphasis on hands-on learning and practical exposure to VLSI design using industry-standard tools supported by the **Chips to Startup (C2S)** grant from the **Ministry of Electronics and Information Technology (MeitY)**.
