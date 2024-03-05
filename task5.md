# As per the Update given for the next task "Should Use the RISC-V Core Verilog netlist and testbench for functional Simulation.
# Veriog code is being executed and the waveforms are generated using the gtkwave

# Aim: To verify the Functional Simulation:-
# Table of contents
- [1.RISC-V RV32I](#1-RISC-V-RV32I)
 - [2.BLOCK DIAGRAM OF RISC-V RV32I](#2-BLOCK-DIAGRAM-OF-RISC-V-RV32I)
 - [3.INSTRUCTION SET OF RISC-V RV32I](#3-INSTRUCTION-SET-OF-RISC-V-RV32I)
 - [4.FUNCTIONAL SIMULATION](#4-FUNCTIONAL-SIMULATION)
    - [4.1 About iverilog and gtkwave](#41-About-iverilog-and-gtkwave)
    - [4.2 Installing iverilog and gtkwave](#42-Installing-iverilog-and-gtkwave)
    - [4.3 The output waveform](#43-The-output-waveform)
  
   ## 1. RISC-V RV32I

This project provides an insight into the working of a few important instructions of the instruction set of a Single cycle Reduced Instruction Set Computer - Five(RISC-V) Instruction Set Architecture suitable for use across wide-spectrum of Applications from low-power embedded devices to high-performance Cloud-based Server processors. The base RISC-V is a 32-bit processor with 31 general-purpose registers, so all the instructions are 32-bit long. Some Applications where the RISC-V processors have begun to make some significant threads are in Artificial intelligence and machine learning, Embedded systems, ultra-low power processing systems, etc.

## 2. BLOCK DIAGRAM OF RISC-V RV32I

![WhatsApp Image 2024-03-05 at 14 01 24_65bae9fa](https://github.com/16swetha/ckswetha/assets/160165692/03c93012-f251-4fdd-bc6c-2e94672da274)

## 3. INSTRUCTION SET OF RISC-V RV32I

![WhatsApp Image 2024-03-05 at 14 02 51_cb8e3b8b](https://github.com/16swetha/ckswetha/assets/160165692/8dd160f4-dfa2-4bde-92e4-e8e355cb14a3)


![WhatsApp Image 2024-03-05 at 14 02 54_0772040f](https://github.com/16swetha/ckswetha/assets/160165692/ae150d1a-01e6-4eb0-9d5c-90a8bb0f51ed)

## 4. FUNCTIONAL SIMULATION

### 4.1 About iverilog and gtkwave
- Icarus Verilog is an implementation of the Verilog hardware description language.
- GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing.
  
### 4.2 Installing iverilog and gtkwave

- **For Ubuntu**

 Open your terminal and type the following to install iverilog and GTKWave
 ```
 $   sudo apt get update
 $   sudo apt get install iverilog gtkwave
 ```

![WhatsApp Image 2024-03-05 at 14 06 21_b7b43118](https://github.com/16swetha/ckswetha/assets/160165692/71c7eb68-c8f0-4e0b-a0ba-8f530bb000eb)

- **To clone the repository and download the netlist files for simulation, enter the following commands in your terminal.**

 ```
 $ git clonehttps://github.com/16swetha/ckswetha.git
 $ cd 
```

![WhatsApp Image 2024-03-05 at 14 06 21_b7b43118](https://github.com/16swetha/ckswetha/assets/160165692/84ea886a-0423-46d1-b400-dda567150e17)

- **To simulate and run the Verilog code, enter the following commands in your terminal.**

```
$ iverilog -o hello hello.v hello_tb.v
$ ./hello
```



- **To see the output waveform in gtkwave, enter the following commands in your terminal.**

`$ gtkwave hello.vcd`

![WhatsApp Image 2024-03-05 at 14 15 14_178d0b78](https://github.com/16swetha/ckswetha/assets/160165692/bfa30f90-b0e4-415b-ac9b-04b7076ae91a)

### 4.3 The output waveform

 The output waveform showing the instructions performed in a 5-stage pipelined architecture.
 
 Instruction 1:add r6,r2,r1
 <img width="1282" alt="1" src="https://github.com/Abdulbitm/Abdul/assets/160620896/9475de20-c117-476a-bebc-54dd3548c109">

 Instruction 2:sub r7,r1,r2
 <img width="1280" alt="2" src="https://github.com/Abdulbitm/Abdul/assets/160620896/2c95f18f-191e-4500-9cda-e7e838d1e609">

Instruction 3:and r8,r1,r3
<img width="1282" alt="3" src="https://github.com/Abdulbitm/Abdul/assets/160620896/18bfdf76-1173-4984-b50b-83443ab48596">

Instruction 4:or r9,r2,r5
<img width="1294" alt="4" src="https://github.com/Abdulbitm/Abdul/assets/160620896/4f214bb2-c934-4778-bf46-841efe877fb8">

 Instruction 5:xor r10,r1,r4
 <img width="1293" alt="5" src="https://github.com/Abdulbitm/Abdul/assets/160620896/6fa91f49-5e73-4133-8bf6-84ec4aca64da">

 Instruction 6:slt r11,r2,r4
<img width="1290" alt="6" src="https://github.com/Abdulbitm/Abdul/assets/160620896/c9c32048-62ed-4f55-8e11-9763816b1bd1">

 Instruction 7:addi r12,r4,5
 <img width="1285" alt="7" src="https://github.com/Abdulbitm/Abdul/assets/160620896/308b8a9d-46c8-4a0e-8824-90e11d9a6a1e">

 Instruction 8:sw r3,r1,2
 <img width="1280" alt="8" src="https://github.com/Abdulbitm/Abdul/assets/160620896/84f16d7f-9d16-4236-b64d-615e187a00ff">

 Instruction 9:lw r13,r1,2
<img width="1295" alt="9" src="https://github.com/Abdulbitm/Abdul/assets/160620896/c7bc7d9a-6745-4eeb-903d-fa723dca1394">

 Instruction 10:beq r0,r0,15
 <img width="1287" alt="10" src="https://github.com/Abdulbitm/Abdul/assets/160620896/a1c6781f-c301-45d9-a502-fb32e6204e4c">

 After branching, performing
 Instruction 11:add r14,r2,r2
 <img width="1287" alt="11" src="https://github.com/Abdulbitm/Abdul/assets/160620896/56b50ce0-60aa-41fe-8f53-0b4583b39665">

  Full 5-stage instruction pipeline and pc-increment description Waveform
  
<img width="1325" alt="12" src="https://github.com/Abdulbitm/Abdul/assets/160620896/e5ebc923-ad2c-44fc-a577-3ce7b8419bce">


![WhatsApp Image 2024-03-05 at 14 17 57_b53184ad](https://github.com/16swetha/ckswetha/assets/160165692/ad99262b-6c42-44a2-8ef4-c35773c6a9d3)

![WhatsApp Image 2024-03-05 at 14 20 04_e2a37576](https://github.com/16swetha/ckswetha/assets/160165692/cf230436-0dc8-493b-b200-b34150cae12d)





