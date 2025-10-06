version.

guardian: A programming pattern that uses a conditional statement to check for and han-

dle circumstances that might cause an error.

6.11 Exercises

Exercise 6.4. Draw a stack diagram for the following program. What does the program print? Solution: http://thinkpython.com/code/stack_diagram.py.

def b(z):

prod = a(z, z) print z, prod return prod

def a(x, y):

x = x + 1 return x * y

6.11. Exercises

def c(x, y, z):

total = x + y + z square = b(total)**2 return square

x = 1 y = x + 1 print c(x, y+3, x+y) Exercise 6.5. The Ackermann function, A(m,n), is deﬁned:

A(m,n) =

 



n + 1 A(m − 1,1) A(m − 1, A(m,n − 1))

if m = 0 if m > 0 and n = 0 if m > 0 and n > 0.