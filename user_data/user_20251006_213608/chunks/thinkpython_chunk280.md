UnboundLocalError: local variable

’

count

’

referenced before assignment

Python assumes that count is local, which means that you are reading it before writing it. The solution, again, is to declare count global.

def example3():

global count count += 1

If the global value is mutable, you can modify it without declaring it:

11.7. Long integers

known = {0:0, 1:1}

def example4():

known[2] = 1

So you can add, remove and replace elements of a global list or dictionary, but if you want to reassign the variable, you have to declare it:

def example5():

global known known = dict()

11.7 Long integers

If you compute fibonacci(50), you get:

>>> fibonacci(50) 12586269025L

The L at the end indicates that the result is a long integer, or type long. In Python 3, long is gone; all integers, even really big ones, are type int.

Values with type int have a limited range; long integers can be arbitrarily big, but as they get bigger they consume more space and time.