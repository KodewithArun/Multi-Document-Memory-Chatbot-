The four countdown frames have different values for the parameter n. The bottom of the stack, where n=0, is called the base case. It does not make a recursive call, so there are no more frames. Exercise 5.1. Draw a stack diagram for print_n called with s = Exercise 5.2. Write a function called do_n that takes a function object and a number, n, as argu- ments, and that calls the given function n times.

’

’

Hello

and n=2.

45

46

Chapter 5. Conditionals and recursion

<module>countdowncountdowncountdowncountdownn3n2n1n0

Figure 5.1: Stack diagram.

5.10 Inﬁnite recursion

If a recursion never reaches a base case, it goes on making recursive calls forever, and the program never terminates. This is known as inﬁnite recursion, and it is generally not a good idea. Here is a minimal program with an inﬁnite recursion:

def recurse():

recurse()