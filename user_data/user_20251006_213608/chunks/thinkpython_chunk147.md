def recurse():

recurse()

In most programming environments, a program with inﬁnite recursion does not really run forever. Python reports an error message when the maximum recursion depth is reached:

File "<stdin>", line 2, in recurse File "<stdin>", line 2, in recurse File "<stdin>", line 2, in recurse . . . File "<stdin>", line 2, in recurse

RuntimeError: Maximum recursion depth exceeded

This traceback is a little bigger than the one we saw in the previous chapter. When the error occurs, there are 1000 recurse frames on the stack!

5.11 Keyboard input

The programs we have written so far are a bit rude in the sense that they accept no input from the user. They just do the same thing every time.