# Design, Implementation and Simulation of an 8-Point FFT Circuit in 45nm CMOS

## Overview

This project presents the RTL design, simulation, synthesis, and
performance analysis of an 8-Point Fast Fourier Transform (FFT)
circuit implemented using 45nm CMOS technology.

The design processes eight complex-valued inputs using signed
16-bit fixed-point arithmetic in 8.8 format.

The complete design flow includes RTL development, functional
simulation, synthesis, static timing analysis, and power analysis.

## Key Features

- 8-Point FFT architecture
- 16-bit signed fixed-point arithmetic
- 8.8 fixed-point representation
- Complex-valued input and output
- Carry Select Adder (CSA)
- Borrow Select Subtractor (BSS)
- Fixed-point multiplier
- Twiddle-factor based FFT computation
- RTL simulation and waveform verification
- 45nm CMOS synthesis
- Static Timing Analysis
- Power and energy analysis

## Architecture

The FFT architecture consists of:

- 12 Adder-Subtractor blocks
- 12 Twiddle-Factor blocks
- Carry Select Adders
- Borrow Select Subtractors
- Fixed-point multipliers

The circuit performs an FFT computation in **2 clock cycles** after
the input arrives. :chatgpt-content-reference{index="1"} :chatgpt-content-reference{index="2"}

## Design Flow

```text
Verilog RTL Design
        ↓
Icarus Verilog Simulation
        ↓
GTKWave Verification
        ↓
Yosys Synthesis
        ↓
45nm Standard Cell Library
        ↓
OpenSTA Timing Analysis
        ↓
Power & Energy Analysis
