# CA-Project
GitHub repo for CA Project (Simulation) Group 22
Team:
Mohammed Kaif (2020084)
Pallav Singla (2020225)
Aayush Kapoor (2020007)
Ishan Malhotra (2020205)


For this project, we created a cycle-accurate simulator for a 5-stage CPU.

Initially, we created an assembler where we defined registers(R0 to R31) in a dictionary and also the type of instruction(i.e add, addi, sub etc) in a dictionary and converted the test instructions into binary. We also created a function “encoded_instruction()” where we used if-else conditions for each type of instruction by comparing their opcodes.

For the Simulator, we created different classes for each operation(i.e FETCH, DECODE, EXECUTE, MEMORY, WRITEBACK); all these classes contain different functions required for their proper and timely execution to get the pipeline and value of registers at each cycle. We also created 2 special types of instructions for peripheral support: LOADNOC and STORENOC, its working and the syntax are given in the pdf given to us. 

Finally, for the output, we get the pipeline diagram for the instruction set given, it is also capable of parsing all different binary instructions in the ISA, and the simulator generates a log file which contains the value of the register file per clock cycle, cycle number and ending memory state, we also see the necessary required plots in the output.
