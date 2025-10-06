It turns out that class is one of Python’s keywords. The interpreter uses keywords to recognize the structure of the program, and they cannot be used as variable names.

Python 2 has 31 keywords:

and as assert break class continue def

del elif else except exec finally for

from global if import in is lambda

not or pass print raise return try

while with yield

In Python 3, exec is no longer a keyword, but nonlocal is.

You might want to keep this list handy. If the interpreter complains about one of your variable names and you don’t know why, see if it is on this list.

2.4 Operators and operands

Operators are special symbols that represent computations like addition and multiplica- tion. The values the operator is applied to are called operands.

The operators +, -, *, / and ** perform addition, subtraction, multiplication, division and exponentiation, as in the following examples:

20+32

hour-1

hour*60+minute

minute/60

5**2

(5+9)*(15-7)