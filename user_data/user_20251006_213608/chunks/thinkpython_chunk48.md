2

Chapter 1. The way of the program

SOURCECODEINTERPRETEROUTPUT

Figure 1.1: An interpreter processes the program a little at a time, alternately reading lines and performing computations.

CODEOBJECTEXECUTORCODESOURCECOMPILEROUTPUT

Figure 1.2: A compiler translates source code into object code, which is run by a hardware executor.

Due to these advantages, almost all programs are written in high-level languages. Low- level languages are used only for a few specialized applications.

Two kinds of programs process high-level languages into low-level languages: interpreters and compilers. An interpreter reads a high-level program and executes it, meaning that it does what the program says. It processes the program a little at a time, alternately reading lines and performing computations. Figure 1.1 shows the structure of an interpreter.