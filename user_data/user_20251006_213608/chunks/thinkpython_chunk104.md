If an error occurs during a function call, Python prints the name of the function, and the name of the function that called it, and the name of the function that called that, all the way back to __main__.

For example, if you try to access cat from within print_twice, you get a NameError: Traceback (innermost last):

File "test.py", line 13, in __main__

cat_twice(line1, line2)

File "test.py", line 5, in cat_twice

print_twice(cat)

File "test.py", line 9, in print_twice

print cat

NameError: name

’

cat

’

is not defined

This list of functions is called a traceback. It tells you what program ﬁle the error occurred in, and what line, and what functions were executing at the time. It also shows the line of code that caused the error.

25

26

Chapter 3. Functions

The order of the functions in the traceback is the same as the order of the frames in the stack diagram. The function that is currently running is at the bottom.

3.11 Fruitful functions and void functions