Also, you can extract the right-most digit or digits from a number. For example, x % 10 yields the right-most digit of x (in base 10). Similarly x % 100 yields the last two digits.

5.2 Boolean expressions

A boolean expression is an expression that is either true or false. The following examples use the operator ==, which compares two operands and produces True if they are equal and False otherwise: >>> 5 == 5 True >>> 5 == 6 False True and False are special values that belong to the type bool; they are not strings: >>> type(True) ’ <type >>> type(False) <type

’

>

bool

’

’

bool

>

42

Chapter 5. Conditionals and recursion

The == operator is one of the relational operators; the others are:

x != y x > y x < y x >= y x <= y

# x is not equal to y # x is greater than y # x is less than y # x is greater than or equal to y # x is less than or equal to y