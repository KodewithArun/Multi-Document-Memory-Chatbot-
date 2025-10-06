1. Write a function that draws a grid like the following:

29

30

Chapter 3. Functions

+ - - - - + - - - - + | | | | | | | | | | | | + - - - - + - - - - + | | | | | | | | | | | | + - - - - + - - - - +

Hint: to print more than one value on a line, you can print a comma-separated sequence:

print

’

+

’

,

’



’

If the sequence ends with a comma, Python leaves the line unﬁnished, so the value printed next appears on the same line.

print print

’ ’

+ -

’ ’

,

The output of these statements is

’

+ -

’

.

A print statement all by itself ends the current line and goes to the next line.

2. Write a function that draws a similar grid with four rows and four columns.

Solution: http://thinkpython.com/code/grid.py. Credit: This exercise is based on an exercise in Oualline, Practical C Programming, Third Edition, O’Reilly Media, 1997.

Chapter 4

Case study: interface design

Code examples from this chapter are available from http://thinkpython.com/code/ polygon.py.