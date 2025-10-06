4.2 Simple repetition

Chances are you wrote something like this (leaving out the code that creates TurtleWorld and waits for the user):

fd(bob, 100) lt(bob)

fd(bob, 100) lt(bob)

fd(bob, 100) lt(bob)

fd(bob, 100)

We can do the same thing more concisely with a for statement. Add this example to mypolygon.py and run it again:

for i in range(4): ’

’

print

Hello!

You should see something like this:

4.3. Exercises

Hello! Hello! Hello! Hello!

This is the simplest use of the for statement; we will see more later. But that should be enough to let you rewrite your square-drawing program. Don’t go on until you do.

Here is a for statement that draws a square:

for i in range(4):

fd(bob, 100) lt(bob)

The syntax of a for statement is similar to a function deﬁnition. It has a header that ends with a colon and an indented body. The body can contain any number of statements.