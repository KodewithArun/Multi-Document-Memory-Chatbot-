Although multiple assignment is frequently helpful, you should use it with caution. If the values of variables change frequently, it can make the code difﬁcult to read and debug.

64

Chapter 7. Iteration

75bruce

Figure 7.1: State diagram.

7.2 Updating variables

One of the most common forms of multiple assignment is an update, where the new value of the variable depends on the old.

x = x+1

This means “get the current value of x, add one, and then update x with the new value.”

If you try to update a variable that doesn’t exist, you get an error, because Python evaluates the right side before it assigns a value to x:

>>> x = x+1 NameError: name

’

x

’

is not defined

Before you can update a variable, you have to initialize it, usually with a simple assign- ment:

>>> x = 0 >>> x = x+1

Updating a variable by adding 1 is called an increment; subtracting 1 is called a decrement.

7.3 The while statement