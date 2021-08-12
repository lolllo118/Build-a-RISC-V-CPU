## Build-a-RISC-V-CPU (edX course)

Course: LinuxFoundationX LFD111x

Platform: Makerchip

Language: TL-Verilog


* No need declare signal/wires 
* No need testbench, provides random stimulus.
* [Website](https://www.redwoodeda.com/tl-verilog)

## CPU Microarchitecture and Implementation 

![RISC-V_CPU_Block_Diagram](https://user-images.githubusercontent.com/88729576/129226502-81671689-c7d8-4723-b83c-0d9771b428a6.png)

1. Identifies the instruction our CPU will execute next. Most instructions execute sequentially, meaning the default behavior of the PC is to increment to the following instruction each clock cycle. Branch and jump instructions, however, are non-sequential.
2. Holds the instructions to execute. To read the IMem, or "fetch", we simply pull out the instruction pointed to by the PC.
3. Interpret/decode instruction to execute.Tell us which registers to read, which operation to perform, etc.
4. Small local storage of values the program is actively working with. We decoded the instruction to determine which registers we need to operate on. Now, we need to read those registers from the register file.
5. Add, subtract, multiply, shift, etc, based on the operation specified in the instruction.
6. Result value from the ALU can be written back to the destination register specified in the instruction.
7. DMem is written to by store instructions and read from by load instructions.


## Lab

* L1: Full adder
* L2: Calculator (Combinational)
* L3: Calculator (Sequential)
* L4: Counter


