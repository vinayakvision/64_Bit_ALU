# 64-Bit Arithmetic Logic Unit (ALU)

This repository contains the design and simulation files for a 64-bit Arithmetic Logic Unit (ALU). The ALU is a fundamental component of a CPU, capable of performing various arithmetic, logical, shift, and comparison operations on 64-bit data inputs.

## Features
- **Arithmetic Operations**: Addition, subtraction, multiplication, and division.
- **Logical Operations**: AND, OR, XOR, and NOT.
- **Shift Operations**: Logical and arithmetic left/right shifts.
- **Comparison Operations**: Greater-than, less-than, and equality checks.
- **Condition Flags**: Outputs such as Carry, Zero, Overflow, and Negative indicate operation results.

## Design Overview
- The ALU takes two 64-bit operands and a control signal (`opcode`) to determine the operation.
- It produces a 64-bit result along with status flags.
- Designed and verified using **Vivado** for simulation and testing.

## How It Works
1. **Input**:
   - Two 64-bit operands: `A[63:0]` and `B[63:0]`
   - Control signal (`opcode`): Specifies the operation type.
2. **Operation**:
   - The ALU decodes the `opcode` and executes the corresponding operation on the inputs.
3. **Output**:
   - 64-bit result (`Result[63:0]`)
   - Flags:
     - **Carry**: Indicates an overflow in unsigned arithmetic operations.
     - **Zero**: Set if the result is zero.
     - **Overflow**: Indicates overflow in signed arithmetic.
     - **Negative**: Set if the result is negative.

## Simulation
- The functionality of the 64-bit ALU has been verified using test benches in Vivado.
- Corner cases, including overflow and zero conditions, were thoroughly tested.

## Files Included
- `64bit_alu.v`: Verilog code for the 64-bit ALU.
- `testbench_alu.v`: Testbench for simulating the ALU.
- `block_diagram.png`: Simplified schematic of the ALU design.

## Applications
- High-performance CPUs and processors.
- Digital signal processing (DSP) applications.
- Complex computation systems requiring 64-bit precision.

## Getting Started
### Prerequisites
- **Vivado Design Suite**: For simulating and synthesizing the design.

### Steps to Simulate
1. Clone the repository to your local system.
2. Open the Vivado project and load the ALU design files.
3. Run the simulation using the provided testbench.
4. Observe the results in the waveform viewer.

## Contribution
Feel free to submit issues or pull requests to enhance the project or add new features.

## Demonstration
- The simulation in Vivado validates the functionality of the ALU.
- The design can be further synthesized for FPGA implementation.

---
### Contact
For queries, reach out via GitHub issues or email.
