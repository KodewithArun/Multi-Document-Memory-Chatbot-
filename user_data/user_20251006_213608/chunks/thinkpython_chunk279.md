been_called = False

def example2():

been_called = True

# WRONG

But if you run it you will see that the value of been_called doesn’t change. The problem is that example2 creates a new local variable named been_called. The local variable goes away when the function ends, and has no effect on the global variable.

To reassign a global variable inside a function you have to declare the global variable before you use it:

been_called = False

def example2():

global been_called been_called = True

The global statement tells the interpreter something like, “In this function, when I say been_called, I mean the global variable; don’t create a local one.”

Here’s an example that tries to update a global variable:

count = 0

def example3():

count = count + 1

# WRONG

If you run it you get:

UnboundLocalError: local variable

’

count

’

referenced before assignment