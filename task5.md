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
![WhatsApp Image 2024-03-05 at 14 15 14_178d0b78](https://github.com/16swetha/ckswetha/assets/160165692/bfa30f90-b0e4-415b-ac9b-04b7076ae91a)



- **To see the output waveform in gtkwave, enter the following commands in your terminal.**

`$ gtkwave hello.vcd`

![WhatsApp Image 2024-03-05 at 14 24 30_dfc8c135](https://github.com/16swetha/ckswetha/assets/160165692/c6066c79-ebe1-424c-a305-9826ab99aa53)

### 4.3 The output waveform


 


  Full 5-stage instruction pipeline and pc-increment description Waveform
  
<img width="1325" alt="12" src="https://github.com/Abdulbitm/Abdul/assets/160620896/e5ebc923-ad2c-44fc-a577-3ce7b8419bce">


![WhatsApp Image 2024-03-05 at 14 17 57_b53184ad](https://github.com/16swetha/ckswetha/assets/160165692/ad99262b-6c42-44a2-8ef4-c35773c6a9d3)

![WhatsApp Image 2024-03-05 at 14 20 04_e2a37576](https://github.com/16swetha/ckswetha/assets/160165692/cf230436-0dc8-493b-b200-b34150cae12d)





