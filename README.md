# RISC-Custom-Assembler-and-Simulator
RISC : Custom Assembler and Simulator

# Assembler

    An assembler is a software tool or program that translates assembly 
    language code into machine code, which can be directly executed by 
    a computer's processor. It plays a vital role in the development of
    low-level software and system programming, as it bridges the gap 
    between human-readable assembly instructions and the binary
     representations understood by the hardware.

    Assembly language is a low-level programming language that closely 
    corresponds to the machine language instructions of a specific 
    computer architecture. It uses mnemonic codes to represent individual 
    instructions, memory addresses, and data operands. Assembly language 
    provides a more human-readable and manageable alternative to working 
    directly with binary machine code.

    The assembler reads the assembly code, processes each instruction, 
    and generates the corresponding machine code.

# Table of Contents
    1. Contributions
    2. Introduction
    3. Prerequisites
    4. Usage
    5. Supported Instructions

# 1. Introduction
    The Assembler program is designed to convert assembly language instructions into 
    machine code that can be executed by a computer. It follows a simple and straightforward
    approach, translating each assembly instruction into its binary representation.

    The program is written in Python, which provides a high-level and easy-to-understand
    syntax, making it suitable for educational purposes or small-scale projects.

# 2. Pre-requisites
    To run this Assembler program, you need to have the following software installed on your system:

    Python (version 3.6 or higher)

# 3. Usage
    (i) Clone the repository or download the source code files.
    (ii) Open a terminal or command prompt and navigate to the program's directory.
    (iii) Run the program using the following command:
                    python assembler.py
    (iv)The program will read the assembly code from the terminal, assemble
        it, and print the output on the terminal.

# 4. Supported Instructions
    The Assembler program supports a subset of assembly instructions. 
    
    Here is a list of the supported instructions:
    LOAD - Load a value into a register
    STORE - Store a value from a register into memory
    ADD - Add two values and store the result in a register
    SUB - Subtract one value from another and store the result in a register
    MULT - Multiply two values and store the result in a register
    DIV - Divide one value by another and store the result in a register
    MOV Imm - Performs reg1 = $Imm where Imm is a 7 bit value.
    MOV REG - Move content of reg2 into reg1.
    CMP - Compares reg1 and reg2 and sets up the FLAGS register.
    JUMP - Unconditionally jump to a specific memory address
    JUMPEQ - Jump to a specific memory address if two values are equal
    JUMPLT - Jump to a specific memory address if one value is less than another
    JUMPGT - Jump to a specific memory address if one value is greater than another
    LEFT SHIFT - Left shifts reg1 by $Imm, where $Imm is a 7 bit value.
    RIGHT SHIFT - Right shifts reg1 by $Imm, where $Imm is a 7 bit value.
    XOR - Performs bitwise XOR of reg2 and reg3. Stores the result in reg1.
    OR - Performs bitwise OR of reg2 and reg3. Stores the result in reg1.
    AND - Performs bitwise AND of reg2 and reg3. Stores the result in reg1.
    Invert - Performs bitwise NOT of reg2. Stores the result in reg1.
    HALT - Stops the machine from executing until reset.

# Simulator

<p>This Python code provides a simulator for a 16-bit ISA (Instruction Set Architecture) that supports various instructions and opcodes. The simulator allows you to execute binary instructions and observe the effects on the registers and flags.</p>

<h2>ISA Description</h2>

The ISA supports a 16-bit architecture with the following instructions and opcodes, along with their syntax:
- Addition (add reg1 reg2 reg3)
- Subtraction (sub reg1 reg2 reg3)
- Move Immediate (mov reg1 $Imm)
- Move Register (mov reg1 reg2)
- Load (ld reg1 mem_addr)
- Store (st reg1 mem_addr)
- Multiply (mul reg1 reg2 reg3)
- Divide (div reg3 reg4)
- Right Shift (rs reg1 $Imm)
- Left Shift (ls reg1 $Imm)
- Exclusive OR (xor reg1 reg2 reg3)
- OR (or reg1 reg2 reg3)
- AND (and reg1 reg2 reg3)
- Invert (not reg1 reg2)
- Compare (cmp reg1 reg2)
- Unconditional Jump (jmp mem_addr)
- Jump If Less Than (jlt mem_addr)
- Jump If Greater Than (jgt mem_addr)
- Jump If Equal (je mem_addr)
- Halt (hlt)
The ISA includes 7 general-purpose registers (R0 to R6) and 1 flag register (FLAGS). Each register is 16 bits in size.

<h2>Usage</h2>

To simulate the execution of binary instructions, follow these steps:

  1. Define the binary instructions in a list, where each element represents a 16-bit instruction.
     
  2. Create an instance of the BinaryInstructionSimulator class by passing the binary instructions list as an argument.
     
  3. Call the simulate() method on the simulator instance to execute the instructions.
   
  4. After simulation, you can access the current state of registers and flags using the registers and flags attributes of the simulator instance.

<h2>Simulate the execution of instructions</h2>
    
    1. python3 Simulator.py
    2. enter all the instructions line by line
    3. press Ctrl+Z to get the output

<h2>Example</h2>
Here's an example code snippet that demonstrates how to use the binary instruction simulator:

  Define the binary instructions
 
    0b0000000000101011,  # add R1, R2, R3
    0b0000100100101011,  # rs R2, $4
    0b0010000000110010,  # ld R0, 1100100
    0b1001000000000100   # jlt 00000100

  # Contributions
    (i) Namit Jain (2022315)
    (ii) Prayag Parashar (2022377)
    (iii) Naman Jindal (2022311)
    (iv) Niteen Kumar (2022336)
