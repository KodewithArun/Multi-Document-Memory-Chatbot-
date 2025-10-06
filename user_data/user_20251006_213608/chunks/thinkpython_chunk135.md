Solution: //thinkpython.com/code/polygon.py. Exercise 4.5. Read about spirals at http://en.wikipedia.org/wiki/Spiral; then write a program that draws an Archimedian spiral (or one of the other kinds). Solution: http: //thinkpython.com/code/spiral.py.

http://thinkpython.com/code/letters.py,

also

requires

http:

Chapter 5

Conditionals and recursion

5.1 Modulus operator

The modulus operator works on integers and yields the remainder when the ﬁrst operand is divided by the second. In Python, the modulus operator is a percent sign (%). The syntax is the same as for other operators: >>> quotient = 7 / 3 >>> print quotient 2 >>> remainder = 7 % 3 >>> print remainder 1

So 7 divided by 3 is 2 with 1 left over.

The modulus operator turns out to be surprisingly useful. For example, you can check whether one number is divisible by another—if x % y is zero, then x is divisible by y.