## 1. FUNCTIONAL SIMULATION

### 1.1 About iverilog and gtkwave
- Icarus Verilog is an implementation of the Verilog hardware description language.
- GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing.
  
### 1.2 Installing iverilog and gtkwave

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

### 1.3 The output waveform

![WhatsApp Image 2024-03-05 at 14 17 57_b53184ad](https://github.com/16swetha/ckswetha/assets/160165692/ad99262b-6c42-44a2-8ef4-c35773c6a9d3)

![WhatsApp Image 2024-03-05 at 14 20 04_e2a37576](https://github.com/16swetha/ckswetha/assets/160165692/cf230436-0dc8-493b-b200-b34150cae12d)








