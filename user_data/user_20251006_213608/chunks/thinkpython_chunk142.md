Although the indentation of the statements makes the structure apparent, nested condi- tionals become difﬁcult to read very quickly. In general, it is a good idea to avoid them when you can.

Logical operators often provide a way to simplify nested conditional statements. For ex- ample, we can rewrite the following code using a single conditional: if 0 < x:

if x < 10:

print

’

x is a positive single-digit number.

’

The print statement is executed only if we make it past both conditionals, so we can get the same effect with the and operator: if 0 < x and x < 10: ’

’

print

x is a positive single-digit number.

5.8 Recursion

It is legal for one function to call another; it is also legal for a function to call itself. It may not be obvious why that is a good thing, but it turns out to be one of the most magical things a program can do. For example, look at the following function: def countdown(n): if n <= 0:

print

’

Blastoff!

’

else:

print n countdown(n-1)