Function deﬁnitions do not alter the ﬂow of execution of the program, but remember that statements inside the function are not executed until the function is called.

A function call is like a detour in the ﬂow of execution. Instead of going to the next state- ment, the ﬂow jumps to the body of the function, executes all the statements there, and then comes back to pick up where it left off.

That sounds simple enough, until you remember that one function can call another. While in the middle of one function, the program might have to execute the statements in another function. But while executing that new function, the program might have to execute yet another function!

Fortunately, Python is good at keeping track of where it is, so each time a function com- pletes, the program picks up where it left off in the function that called it. When it gets to the end of the program, it terminates.