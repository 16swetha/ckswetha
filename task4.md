**The conventional GCC X86 compiler and the riscv compiler should be simulated for the C code (SPIKE Simulation).**

**GCC (F1) SHOULD HAVE AN EQUAL OUTPUT TO THE RISCV GCC (F2) AS REQUIRED.**

![WhatsApp Image 2024-02-28 at 19 31 55_ededea33](https://github.com/16swetha/ckswetha/assets/160165692/e2b1296e-1056-46dc-bc8e-6fef83a2fb9c)

**Step 1:** To use the standard GCC compiler to run the code To get the code compiled:gcc sum1ton.c -o sum1ton. Utilize "./a.out" to obtain the output: Here, the results show that 125250 is the sum of the numbers from 1 to 50.

**Step 2:** Use the RISC-V GCC compiler to run the code

To get the code compiled: riscv64-unknown-elf-gcc -o sum1ton sum1ton.c  Utilize "./a.out" to obtain the output: Here, the results show that 125250 is the sum of the numbers from 1 to 50.


![WhatsApp Image 2024-02-29 at 11 40 58_fa6a7b73](https://github.com/16swetha/ckswetha/assets/160165692/a49f3fbe-e8d2-4d4b-abae-c34cb99ee28b)


![WhatsApp Image 2024-02-29 at 11 40 45_78527a86](https://github.com/16swetha/ckswetha/assets/160165692/000f5593-9cdf-46f4-96f5-7c7b9c0e50ac)


![WhatsApp Image 2024-02-29 at 11 40 52_643e3e67](https://github.com/16swetha/ckswetha/assets/160165692/4a5ea8b4-1d1c-44fa-9dc8-a9a9d7d6d176)
