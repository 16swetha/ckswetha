By Referring to C-based Lab videos and RISC-V-based lab videos

close-up shots of the compiled C code and RISC-V

Step 1:</p> 
(i)check whether the leafpad is installed in ur machine by using the commands leafpad sum1ton.c& (sum1ton.c is the file name) </p>
(ii)If the leafpad editor is opened without any errors then type the C code. </p>
(iii)If the leafpad is not installed in ur machine then install by using the following command. </p>

**sudo snap install leafpad**

Step 2: Writing the C code in the leafpad editor using the following command

**leafpad sum1ton.c&**

![WhatsApp Image 2024-02-27 at 10 13 51_018e4b9b](https://github.com/16swetha/ckswetha/assets/160165692/33dc2b4d-1ffe-4751-ab87-5ff7cc19d283)

Step 3:  Ctrl+s (to save the code)

Step 4: Check compilation step for the errors 

**gcc sum1ton.c**

![WhatsApp Image 2024-02-27 at 10 17 00_c190e9ce](https://github.com/16swetha/ckswetha/assets/160165692/7b150c74-49c4-4298-b3cb-0abbb9f7f2aa)

Step 5: To check the output use the command

**./a.out**

![WhatsApp Image 2024-02-27 at 11 05 05_74b8f972](https://github.com/16swetha/ckswetha/assets/160165692/b0964a0f-6d28-4874-8a58-4c170038be6c)

The results will be displayed as

Sum of numbers from 1 to 500 is 125250

***RISCV Compilation and Execution

Step 1: View the C Code in the editor window 

**cat sum1ton.c**


![WhatsApp Image 2024-02-27 at 11 36 16_b29ba0a3](https://github.com/16swetha/ckswetha/assets/160165692/0e30ad0b-106e-4e4b-905e-8539f06571aa)

Step 2: Compile the code in riscv using the command

riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c

![WhatsApp Image 2024-02-27 at 11 36 16_b29ba0a3](https://github.com/16swetha/ckswetha/assets/160165692/d95eb78c-e309-4ad3-9534-5c411ede8d78)

Step 3: The ls ltr command iis used to list the contents of the current directory in long format, sorted by last modified time in reverse order in the linux.

use the command

**ls -ltr sum1ton.c**

![WhatsApp Image 2024-02-27 at 10 38 54_71e2f192](https://github.com/16swetha/ckswetha/assets/160165692/57030d99-b29d-4447-be08-9a63dd5bc8fa)

![WhatsApp Image 2024-02-27 at 10 38 54_c623ae40](https://github.com/16swetha/ckswetha/assets/160165692/b573eb29-fa29-4537-b0f9-2f31b3a6d0f3)

![WhatsApp Image 2024-02-27 at 11 10 38_06ab8223](https://github.com/16swetha/ckswetha/assets/160165692/b0709154-b4a1-4c39-9540-17f02b585c1b)

![WhatsApp Image 2024-02-27 at 11 45 41_04bb5211](https://github.com/16swetha/ckswetha/assets/160165692/681289cf-2749-4080-8fc1-d44aaec2417d)

 
 









