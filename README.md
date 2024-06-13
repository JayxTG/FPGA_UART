# UART Implementation on FPGA

This repository contains the implementation of a Universal Asynchronous Receiver/Transmitter (UART) module on a Field-Programmable Gate Array (FPGA) platform. The project was completed by the group members:

- Fernando W.W.R.N.S.
- Gammune D.J.T.
- Herath H.M.S.I.

Special thanks to Lohan, Charels, and Kaveendra for their assistance in transferring and verifying the data.

## Project Overview

The project is divided into four distinct phases, each focusing on a specific aspect of the design and verification process.

### Phase 1: Research and Design Selection

- Research the UART protocol, including data framing, synchronization, and baud rate settings.
- Explore existing Verilog implementations of UART transceivers.
- Review and select a suitable implementation that meets the specified requirements.

### Phase 2: Testbench Development

- Understand the UART module's input and output signals.
- Write a Verilog testbench to simulate the UART environment.
- Test the UART module with various data patterns, baud rates, and edge cases.
- Utilize simulation tools like ModelSim or Vivado's integrated simulator for debugging.

### Phase 3: FPGA Implementation

- Set up the FPGA development environment (Xilinx Vivado or Intel Quartus).
- Develop additional RTL for driving the 7-segment displays.
- Simulate and verify the UART and 7-segment drive circuit.
- Integrate the UART RTL with FPGA specifics, such as GPIO pin assignments and clock frequency matching.
- Synthesize the design, perform place and route, and download the bitstream to the FPGA board.

### Phase 4: Signal Analysis

- Set up an oscilloscope and connect probes to the UART TX and RX lines.
- Configure the oscilloscope for appropriate time and voltage settings.
- Transmit data from the FPGA and observe the waveform corresponding to the UART protocol.
- Analyze the signal for correct start bit, data bits, parity bit, stop bit, and potential signal integrity issues.

## Repository Structure

The repository contains the following directories:

- `Documentation/`: Contains the project task document and the final report.
- `Project Files/`: Contains the Verilog code for the UART implementation, testbenches, and additional files related to the project.
