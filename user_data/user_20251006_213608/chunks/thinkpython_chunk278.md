107

108

Chapter 11. Dictionaries

11.6 Global variables

In the previous example, known is created outside the function, so it belongs to the special frame called __main__. Variables in __main__ are sometimes called global because they can be accessed from any function. Unlike local variables, which disappear when their function ends, global variables persist from one function call to the next.

It is common to use global variables for ﬂags; that is, boolean variables that indicate (“ﬂag”) whether a condition is true. For example, some programs use a ﬂag named verbose to control the level of detail in the output:

verbose = True

def example1(): if verbose: ’

print

Running example1

’

If you try to reassign a global variable, you might be surprised. The following example is supposed to keep track of whether the function has been called:

been_called = False

def example2():

been_called = True

# WRONG