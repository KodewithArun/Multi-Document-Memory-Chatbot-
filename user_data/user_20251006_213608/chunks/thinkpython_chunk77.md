20+32

hour-1

hour*60+minute

minute/60

5**2

(5+9)*(15-7)

In some other languages, ^ is used for exponentiation, but in Python it is a bitwise operator called XOR. I won’t cover bitwise operators in this book, but you can read about them at http://wiki.python.org/moin/BitwiseOperators.

In Python 2, the division operator might not do what you expect:

>>> minute = 59 >>> minute/60 0

The value of minute is 59, and in conventional arithmetic 59 divided by 60 is 0.98333, not 0. The reason for the discrepancy is that Python is performing ﬂoor division. When both of the operands are integers, the result is also an integer; ﬂoor division chops off the fraction part, so in this example it rounds down to zero.

13

14

Chapter 2. Variables, expressions and statements

In Python 3, the result of this division is a float. The new operator // performs ﬂoor division.