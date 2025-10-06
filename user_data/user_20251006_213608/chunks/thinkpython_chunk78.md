In Python 3, the result of this division is a float. The new operator // performs ﬂoor division.

If either of the operands is a ﬂoating-point number, Python performs ﬂoating-point divi- sion, and the result is a float: >>> minute/60.0 0.98333333333333328

2.5 Expressions and statements

An expression is a combination of values, variables, and operators. A value all by itself is considered an expression, and so is a variable, so the following are all legal expressions (assuming that the variable x has been assigned a value): 17 x x + 17

A statement is a unit of code that the Python interpreter can execute. We have seen two kinds of statement: print and assignment.

Technically an expression is also a statement, but it is probably simpler to think of them as different things. The important difference is that an expression has a value; a statement does not.

2.6 Interactive mode and script mode