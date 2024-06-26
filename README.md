# UART Implementation on FPGA

This repository contains the implementation of a Universal Asynchronous Receiver/Transmitter (UART) module on a Field-Programmable Gate Array (FPGA) platform. The project was completed as part of the EN2111 - Electronic Circuit Design module at the Department of Electronic & Telecommunication Engineering, University of Moratuwa, Sri Lanka.

## 👥 Group Members

- 210169L Fernando W.W.R.N.S.
- 210179R Gammune D.J.T.
- 210218M Herath H.M.S.I.

Special thanks to Lohan, Charels, and Kaveendra for their assistance in transferring and verifying the data.

## 🎯 Objective

The objective of this project is to design, implement, and verify a UART module on an FPGA, providing reliable asynchronous serial communication.

## 🔑 Key Features

- 📡 UART protocol implementation
- 💻 FPGA-based design and verification
- 🔬 Comprehensive testbench development
- 🛠️ RTL code for transmitter and receiver
- 📊 ModelSim simulation and timing diagram analysis

## Project Overview

The project is divided into four distinct phases:

### Phase 1: Research and Design Selection
- Research the UART protocol, including data framing, synchronization, and baud rate settings.
- Explore existing Verilog implementations of UART transceivers.
- Review and select a suitable implementation that meets the specified requirements.

### Phase 2: Testbench Development
- Understand the UART module's input and output signals.
- Write a Verilog testbench to simulate the UART environment.
- Test the UART module with various data patterns, baud rates, and edge cases.
- Utilize ModelSim for simulation and debugging.

### Phase 3: FPGA Implementation
- Set up the FPGA development environment (Intel Quartus).
- Develop additional RTL for driving the 7-segment displays.
- Simulate and verify the UART and 7-segment drive circuit.
- Integrate the UART RTL with FPGA specifics, such as GPIO pin assignments and clock frequency matching.
- Synthesize the design, perform place and route, and download the bitstream to the FPGA board.

### Phase 4: Signal Analysis
- Set up an oscilloscope and connect probes to the UART TX and RX lines.
- Configure the oscilloscope for appropriate time and voltage settings.
- Transmit data from the FPGA and observe the waveform corresponding to the UART protocol.
- Analyze the signal for correct start bit, data bits, parity bit, stop bit, and potential signal integrity issues.

## 🛠️ Hardware and Software Requirements

**Hardware:**
- FPGA development board (e.g., DE0 Nano)
- Oscilloscope (for signal analysis)

**Software:**
- Intel Quartus (for FPGA development)
- ModelSim (for simulation)

## 📁 Repository Structure

- `RTL/`: Contains the Verilog code for the UART implementation
  - `uart.v`: Top-level UART module
  - `transmitter.v`: UART transmitter module
  - `receiver.v`: UART receiver module
- `Testbench/`: Contains testbench files
  - `testbench.v`: Main testbench for UART
  - `transmitter_tb.v`: Testbench for transmitter
  - `trans_rec_tb.v`: Testbench for transmitter and receiver
- `Docs/`: Documentation files
  - `Project_Report.pdf`: Detailed project report
- `Simulation/`: ModelSim simulation files and results
- `FPGA/`: FPGA-specific files (pin assignments, etc.)

## 🚀 How to Use

1. **Clone the Repository:**
```bash
git clone https://github.com/your-username/UART-FPGA-Implementation.git
```

2. **RTL Implementation:**
- Open the RTL files in the `RTL/` directory to view or modify the UART implementation.

3. **Simulation:**
- Use ModelSim to run the testbenches in the `Testbench/` directory.
- Analyze the timing diagrams and simulation results.

4. **FPGA Implementation:**
- Open the project in Intel Quartus.
- Synthesize the design and program the FPGA board.

5. **Testing:**
- Use the provided testbenches to verify functionality.
- For hardware testing, refer to the pin planner in the report for proper connections.

## 📊 Results

- Successful implementation of UART transmitter and receiver modules.
- Verified functionality through comprehensive testbenches and ModelSim simulations.
- Timing diagrams and pin planning available in the project report.

## 📚 References

1. [Implementation of UART Protocol Using FPGA](https://medium.com/@namiwije/implementation-of-uart-protocol-using-fpga-a04d0b3b5bcb)
2. [FPGA Basics (Intel)](https://www.intel.com/content/www/us/en/support/programmable/support-resources/fpga-training/getting-started.html)
3. [UART: A Hardware Communication Protocol](https://www.analog.com/en/resources/analog-dialogue/articles/uart-a-hardware-communication-protocol.html)
4. [UART-Implementation-Using-FPGA (GitHub)](https://github.com/namiwijeuom/UART-Implementation-Using-FPGA/tree/main)
5. [DE0 Nano User Manual](https://www.terasic.com.tw/attachment/archive/941/DE0-Nano-SoC_User_manual_rev.D0.pdf)

## 📄 License

This project is open-source and available under the MIT License.
