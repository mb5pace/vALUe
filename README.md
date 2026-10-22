# vALUe — 16-bit Arithmetic Logic Unit

A 16-bit Arithmetic Logic Unit (ALU) designed and implemented in **Logisim** as part of the **Digital Logic with Hardware Description Language (DLHDL)** course.

This project explores digital circuit design, arithmetic operations, bitwise logic, comparison, and the integration of smaller adder circuits into a wider datapath.

## About the Project

The objective is to design a 16-bit ALU that performs multiple arithmetic and logical operations based on a 3-bit select input.

The project includes a 16-bit adder built using smaller 4-bit adders and full adders, as developed in the current project.

**Course:** Digital Logic with Hardware Description Language (DLHDL)  
**Tool:** Logisim  
**Project Type:** Academic coursework  
**Category:** Digital Logic Design

## Inputs and Outputs

### Inputs

| Input | Width | Description |
|---|---:|---|
| A | 16-bit | First operand |
| B | 16-bit | Second operand |
| Select | 3-bit | Selects the ALU operation |
| Reset | 1-bit | Resets the outputs, as specified in the assignment |

### Outputs

| Output | Width | Description |
|---|---:|---|
| Output | 16-bit | Result of the selected operation |
| Overflow | 1-bit | Indicates signed arithmetic overflow |
| Equal | 1-bit | Indicates whether A = B |
| Less Than | 1-bit | Indicates whether A < B |
| Greater Than | 1-bit | Indicates whether A > B |

## Supported ALU Operations

The assignment defines eight operations selected by the 3-bit `Select` input.

| Select | Operation | Function |
|:---:|---|---|
| `000` | ADD | A + B |
| `001` | SUB | A − B using two's complement |
| `010` | AND | Bitwise A AND B |
| `011` | OR | Bitwise A OR B |
| `100` | Comparator | Compare A and B |
| `101` | XOR | Bitwise A XOR B |
| `110` | NOT | Bitwise NOT of A |
| `111` | Increment | A + 1 |

## Learning Objectives

- Understand the design and operation of arithmetic and logic circuits.
- Build wider arithmetic circuits using smaller adder components.
- Explore two's-complement subtraction and signed overflow.
- Implement bitwise operations and comparison logic.
- Integrate circuit components into a functional ALU in Logisim.

## Project Files

- `16bit_ALU.circ` — Logisim circuit file.
- `ALU-Project-Instructions.pdf` — Original assignment specification, if included in this repository.

## Project Scope

This is an academic digital logic design project completed as part of coursework. It focuses on understanding circuit-level implementation and the integration of arithmetic and logical components rather than presenting a production-ready processor component.

## Getting Started

1. Install and open Logisim or a compatible Logisim version.
2. Download or clone this repository.
3. Open `16bit_ALU.circ` in Logisim.
4. Inspect the circuit and test the supported operations using the input controls.

## Status

The project currently includes the 16-bit adder developed using 4-bit adders and full adders. The remaining ALU functionality and its verification should be documented as they are implemented.

---

Created for learning and experimentation as part of the Digital Logic with Hardware Description Language course.
