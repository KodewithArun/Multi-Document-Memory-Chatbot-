A compiler reads the program and translates it completely before the program starts run- ning. In this context, the high-level program is called the source code, and the translated program is called the object code or the executable. Once a program is compiled, you can execute it repeatedly without further translation. Figure 1.2 shows the structure of a compiler.

Python is considered an interpreted language because Python programs are executed by an interpreter. There are two ways to use the interpreter: interactive mode and script mode. In interactive mode, you type Python programs and the interpreter displays the result: >>> 1 + 1 2

The chevron, >>>, is the prompt the interpreter uses to indicate that it is ready. If you type 1 + 1, the interpreter replies 2.

Alternatively, you can store code in a ﬁle and use the interpreter to execute the contents of the ﬁle, which is called a script. By convention, Python scripts have names that end with .py.