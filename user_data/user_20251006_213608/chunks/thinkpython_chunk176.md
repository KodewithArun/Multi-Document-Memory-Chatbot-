6.9 Debugging

Breaking a large program into smaller functions creates natural checkpoints for debugging. If a function is not working, there are three possibilities to consider:

There is something wrong with the arguments the function is getting; a precondition is violated.

There is something wrong with the function; a postcondition is violated.

There is something wrong with the return value or the way it is being used.

To rule out the ﬁrst possibility, you can add a print statement at the beginning of the function and display the values of the parameters (and maybe their types). Or you can write code that checks the preconditions explicitly.

If the parameters look good, add a print statement before each return statement that dis- plays the return value. If possible, check the result by hand. Consider calling the function with values that make it easy to check the result (as in Section 6.2).