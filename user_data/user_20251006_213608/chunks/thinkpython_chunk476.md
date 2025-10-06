A.2.1 My program does absolutely nothing.

This problem is most common when your ﬁle consists of functions and classes but does not actually invoke anything to start execution. This may be intentional if you only plan to import this module to supply classes and functions.

If it is not intentional, make sure that you are invoking a function to start execution, or execute one from the interactive prompt. Also see the “Flow of Execution” section below.

A.2.2 My program hangs.

If a program stops and seems to be doing nothing, it is “hanging.” Often that means that it is caught in an inﬁnite loop or inﬁnite recursion.

If there is a particular loop that you suspect is the problem, add a print statement immediately before the loop that says “entering the loop” and another immediately after that says “exiting the loop.” Run the program. If you get the ﬁrst message and not the second, you’ve got an inﬁnite loop. Go to the “Inﬁnite Loop” section below.