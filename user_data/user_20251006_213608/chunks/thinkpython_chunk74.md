An assignment statement creates new variables and gives them values:

’

>>> message = >>> n = 17 >>> pi = 3.1415926535897932

And now for something completely different

’

This example makes three assignments. The ﬁrst assigns a string to a new variable named message; the second gives the integer 17 to n; the third assigns the (approximate) value of π to pi.

A common way to represent variables on paper is to write the name with an arrow pointing to the variable’s value. This kind of ﬁgure is called a state diagram because it shows what state each of the variables is in (think of it as the variable’s state of mind). Figure 2.1 shows the result of the previous example.

The type of a variable is the type of the value it refers to.

>>> type(message) <type str >>> type(n) ’ <type > >>> type(pi) ’ float <type

’

’

>

’

int

’

>

2.3 Variable names and keywords

Programmers generally choose names for their variables that are meaningful—they docu- ment what the variable is used for.