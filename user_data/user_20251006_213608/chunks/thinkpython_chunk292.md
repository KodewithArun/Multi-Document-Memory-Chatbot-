12.3. Tuples as return values

12.3 Tuples as return values

Strictly speaking, a function can only return one value, but if the value is a tuple, the effect is the same as returning multiple values. For example, if you want to divide two integers and compute the quotient and remainder, it is inefﬁcient to compute x/y and then x%y. It is better to compute them both at the same time.

The built-in function divmod takes two arguments and returns a tuple of two values, the quotient and remainder. You can store the result as a tuple:

>>> t = divmod(7, 3) >>> print t (2, 1)

Or use tuple assignment to store the elements separately:

>>> quot, rem = divmod(7, 3) >>> print quot 2 >>> print rem 1

Here is an example of a function that returns a tuple:

def min_max(t):

return min(t), max(t)

max and min are built-in functions that ﬁnd the largest and smallest elements of a sequence. min_max computes both and returns a tuple of two values.

12.4 Variable-length argument tuples