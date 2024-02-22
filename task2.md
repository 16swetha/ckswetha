# VARIOUS TYPES OF RISC-V INSTRUCTIONS
<p align="justify">RISC-V is a modular, extensible computer instruction set architecture (ISA) that supports 16-bit (RV16E), 32-bit (RV32I).RISC-V instructions are encoded using a fixed-length 32-bit format, which simplifies decoding and execution of instructions handling the upper bits and the lower bits</p>
 

<details>
<summary><b>R-type instructions:
</b></summary>
<br>
<p align="justify">The R-type instruction in the RISC-V architecture is used for operations without an immediate value. It is primarily used for register-register operations.</p>
Example: </p>
'add rd, rs1, rs2':This instruction adds the values in register rs1 and rs2 and stores the result in register 'rd '</p>
	
'and rd, rs1, rs2': This instruction performs a bitwise AND of the values in register rs1 and rs2 and stores the result in register 'rd'</p>
  </details>
<details>
<summary><b>I-type instructions:
</b></summary>
<br>
<p align="justify">The I-type instruction set in RISC-V is used for instructions with immediates and loads. It is used for performing various arithmetic and logical operations using immediate values and memory. </p>
Example:</p>
addi rd, rs1, imm: This instruction adds an immediate value to the value in register rs1 and stores the result in register rd.
	
  </details>
<details>
<summary><b>S-type instructions:
</b></summary>
<br>
<p align="justify">Used for store operations, which store data from a register to memory. They include two register operands and a 12-bit immediate value for the memory address offset. </p>
Example:</p>
sw rs2, offset(rs1): This instruction stores the value in register rs2 to the memory location specified by the sum of an immediate offset and the value in register rs1.</p>
	
sh rs2, offset(rs1): This instruction stores the least significant 2 bytes of the value in register rs2 to the memory location specified by the sum of an immediate offset and the value in register rs1.</p>

  </details>
<details>
<summary><b>B-type instructions:
</b></summary>
<br>
<p align="justify">B-type instructions in RISC-V are variations of S-type instructions, primarily used for conditional branches. They share the same structure as S-type instructions, with two register sources (rs1/rs2) and a 12-bit immediate imm[12:1], but differ in the interpretation of the immediate value. In B-type instructions, the least significant bit of the immediate value is ignored, effectively scaling the branch offset by 2 bytes</p>
Example:</p>
beq rs1, rs2, label: This instruction branches to the address of the labeled instruction if the values in registers rs1 and rs2 are equal.</p>
bne rs1, rs2, label: This instruction branches to the address of the labeled instruction if the values in registers rs1 and rs2 are not equal.</p>
  </details>
<details>
<summary><b>U-type instructions:
</b></summary>
<br>
<p align="justify"> The U-type instruction format in RISC-V is used for instructions containing a 20-bit unsigned immediate value. Two common examples of U-type instructions include:</p>
	
auipc (Add Unsigned Immediate to Program Counter): This instruction calculates the effective address of a symbol relative to the current instruction pointer.</p>
assembly</p>
auipc rt, imm(19:12)</p>

lui (Load Upper Immediate): This instruction loads a constant value into a general-purpose register.</p>
assembly</p>
lui rt, imm(19:12)</p>
  </details>
<details>
<summary><b>J-type instructions:
</b></summary>
<br>
<p align="justify">The J-type instruction format in RISC-V is used for unconditional jumps. The J-type instructions include the JAL (Jump and Link) instruction, which is used to perform an unconditional jump and save the address of the next instruction in the link register.</p>
Example:</p>
jump</p>
</details>

# Base Instructions Format

<p align="justify">The base instruction format in RISC-V consists of 32 bits and is designed to be simple and modular. The format is divided into several fields, each serving a specific purpose. The opcode field, typically the leftmost 7 bits, specifies the operation to be performed. Depending on the opcode, additional fields may follow, such as the destination register (rd), source registers (rs1 and rs2), and immediate values for certain instructions. The RISC-V instruction set architecture supports different instruction formats to accommodate various types of operations, including R-type (register-register), I-type (immediate), S-type (store), B-type (branch), U-type (upper immediate), and J-type (jump). The consistent structure of these instructions simplifies decoding and execution in the processor, contributing to the overall simplicity and efficiency of the RISC-V architecture. The modular design of the instruction format allows for easy expansion and customization, making RISC-V versatile and adaptable to diverse computing needs.</p>

<details>
<summary><b>Instruction code format </b></summary>![Gkjuc](https://github.com/16swetha/ckswetha/assets/160165692/4a7bdbee-c335-4794-bdde-99a13b8526a2)

</details>

# RISC-V REGISTER FILE: 
 <p align="justify">In RISC-V, the register file is a small, fast storage area that holds the processor's general-purpose registers. The architecture defines a set of 32 integer registers (x0 to x31), each 32 bits wide. Among these, register x0 is hardwired to zero and reads as zero when used in computations. The remaining registers can be used for various purposes in program execution, such as holding data, addresses, or intermediate results. The register file is accessed by the instructions to read operands and store results during the execution of programs. Instructions explicitly specify the source and destination registers, facilitating a simple and efficient design. The use of a relatively small number of registers is a characteristic feature of RISC (Reduced Instruction Set Computing) architectures, promoting a streamlined instruction set and enabling faster execution by minimizing the number of clock cycles needed for instruction execution. The register file plays a crucial role in supporting the RISC-V instruction set, providing a set of versatile storage locations for data manipulation and computation within the processor.</p>
