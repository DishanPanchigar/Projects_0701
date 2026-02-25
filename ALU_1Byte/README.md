# Gate-Level Arithmetic Logic Unit (ALU)

## Overview
This project implements a fully functional **Arithmetic Logic Unit (ALU)** designed at the **gate level** using fundamental digital logic components.  
The objective was to understand processor computation by building the datapath and control logic from scratch instead of using predefined arithmetic modules.

The design follows a **bit-slice architecture**, where each bit operates in parallel while sharing common control signals.

---

## Features

### Arithmetic Operations
- Addition (ADD)
- Subtraction (SUB)

### Logical Operations
- AND
- OR
- XOR
- NOT
- NAND
- NOR
- XNOR
- IMPLIES
- NIMPLIES

### Shift Operations
- Left Shift
- Right Shift

### Status Flags
- Zero Flag
- Auxiliary Carry
- Overflow Flag

---

## Design Highlights
- Opcode-based operation selection using a decoder
- Multiplexer-driven output architecture
- Ripple-carry adder structure
- Logic reuse: XOR and AND operations derived from internal adder signals
- Gate-level implementation without high-level arithmetic blocks

---

## Simulation Environment
A dedicated simulation circuit was created to:
- Apply test inputs
- Validate opcode execution
- Verify flag behavior
- Observe real-time output responses

---

## Architecture
The ALU consists of:
- Input registers (Operand A & Operand B)
- Opcode decoder
- Arithmetic and logic computation blocks
- Output selection multiplexers
- Flag generation logic

---

## Learning Outcomes
This project demonstrates practical understanding of:
- Digital System Design
- Computer Architecture fundamentals
- Datapath & Control Logic
- Hardware optimization techniques

---

## Future Improvements
- Carry Lookahead Adder implementation
- FPGA synthesis
- Pipelined ALU architecture
- Timing optimization

---

## Author
Dishan Panchigar

---

## License
This project is licensed under the MIT License - see the LICENSE file for details.