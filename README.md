# Pep/9 Traps

## Description
This project involves extending the Pep/9 operating system with custom trap instructions. These enhancements are based on exercises from "Computer Systems, 5th Edition" by J. Stanley Warford. The main focus is on implementing and testing new unary and nonunary instructions within the Pep/9 simulator.

## Features
- **ASL2**: A new unary instruction replacing NOP0, which performs two left shifts on the accumulator. Flags NZC are updated based on the new accumulator value, and V is set if there's an overflow in either shift.
- **MULA**: A nonunary instruction to multiply the accumulator with the operand using direct addressing. It utilizes the iterative shift-and-add method detailed in Problem 6.24 of the course textbook.
- **BOOLO**: Introduces a Boolean output instruction that evaluates the truthiness of the operand. It supports immediate, direct, and stack-relative addressing modes.
- **STWADI**: Implements double indirect addressing for storing the word in the accumulator, showcasing the layered addressing capabilities of Pep/9.

## Installation
1. Clone this repository to your local machine.
2. Ensure you have the Pep/9 simulator installed.
3. Load the `.pep` files into the simulator to begin testing the new instructions.

## Usage
To test the new instructions:
1. Open the Pep/9 simulator.
2. Load the test files provided in the `/tests` directory.
3. Execute the code and observe the behavior of the system flags and outputs as described in the features.


## Acknowledgments
- Special thanks to Professor David Duvall-Early at Piedmont Virginia Community College for his guidance and support throughout this project.
- "Computer Systems, 5th Edition" by J. Stanley Warford, which served as a primary resource.
