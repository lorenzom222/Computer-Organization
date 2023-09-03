# Chapter 1: Tour of Computer Science

### Bits + Context
- Source file = hello.c -> Created by programming in some language
- File -> Text-Chars -> bytes (sequence of bits) -> {0,1}
- Machine representation of nums are NOT ints or real numbers
- THEY ARE FINITE APPROXIMATIONS
- This causes weird behaviours sometimes

### Program Cycle
- Source program = hello.c (High level bc human readable)
- Preprocessing Phase = hello.i (Reads in necessary libraries from #, #include, and modifies source program, C files)
- Compilation = hello.s (Converts C file with # into assembly code to be compiled)
- Assembly = hello.o (Gets the assembly code and turns into binary machine instructions, puts in object file)
- Link = hello (Executable file to be ran connected to object file hello.o)

### Hardware
- Shell: Interpreter for commands
- Buses: Vehicle for bytes of info between component
- I/O Devices: Connections to external world. Ex: Keyboard, mouse, disk drive. I/O devs are connected to I/O buses such as adapters.
- Main memory: Temp storage that holds program being executed and data it uses. 
    - Physically: Made of DRAM chips. 
    - Logically: Organized as a linear array of bytes, which means that the data stored in memory is arranged in a sequential order. Each byte of data has its own unique address, which is used to locate and access it. These addresses are like array indexes, starting at zero and increasing by one for each subsequent byte. 
- Processors (CPU): The Chef. Engine that interprets or executes instructions from main memory. 
    - Program Counter (PC): Register, storage location in CPU, that points to some machine instructions from main memory.
    - CPU run continously, performing task PC points at and updates it
    - ISA (Instruction Set Architecture): The Cookbook for the CPU. Set of rules the CPU follows to understand and execute each instruction. Instructions are followed in this strict order:
        - Fetch: Reads instruction pointed at by PC
        - Decode: Interprets the bits to determine operation
        - Execute: Performs operation
        - Update PC: PC advances to next instruction necessary
- Arithmetic/Logic Unit (ALU): Math Wizard. Responsible for calculations and logical operation. Computes new data and address values
- Example of Simple operations:
    - Load: Copy byte or word from main memory into a register, replacing what the register had before
    - Store: Copy byte or word from a register to location in main memory, overriding what was at the location
    - Operate: Copy content of 2 registers to ALU, perform arithmetic on both words, store result in register, overwrites what was in that register
    - Jump: Extract word from instruction itself and copy it into the PC, replacing the previous PC value or instruction. So, just skipping to new instruction.

### Operating System x Hardware
#### Process
The OS creates an illusion that each program has access to hardware. This is called process. This is a seperate entity that manages and execute the program
- Process represents a running program. Meaning when you start a program, the OS creates a box that captures the program's code and data.
- This allows is to run independently alongside other processess.

#### Threads
- Within a process, it can have multiple execution units called threads.
- Threads share the same program code and global data within the process
- Allows for concurrent programming, data sharing compared to processes..
