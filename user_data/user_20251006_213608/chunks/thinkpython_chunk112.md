ables and parameters of the function.

traceback: A list of the functions that are executing, printed when an exception occurs.

3.16 Exercises

Exercise 3.3. Python provides a built-in function called len that returns the length of a string, so the value of len(

’

’

allen

) is 5.

Write a function named right_justify that takes a string named s as a parameter and prints the string with enough leading spaces so that the last letter of the string is in column 70 of the display.

>>> right_justify(

’

allen

’

)

allen

Exercise 3.4. A function object is a value you can assign to a variable or pass as an argument. For example, do_twice is a function that takes a function object as an argument and calls it twice:

def do_twice(f):

f() f()

Here’s an example that uses do_twice to call a function named print_spam twice.

def print_spam():

’

’

print

spam

do_twice(print_spam)

1. Type this example into a script and test it.