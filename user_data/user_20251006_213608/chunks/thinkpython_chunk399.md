Unfortunately, this implementation of addition is not commutative. If the integer is the ﬁrst operand, you get

>>> print 1337 + start TypeError: unsupported operand type(s) for +:

’

int

’

and

’

instance

’

The problem is, instead of asking the Time object to add an integer, Python is asking an integer to add a Time object, and it doesn’t know how to do that. But there is a clever solution for this problem: the special method __radd__, which stands for “right-side add.” This method is invoked when a Time object appears on the right side of the + operator. Here’s the deﬁnition:

# inside class Time:

def __radd__(self, other):

return self.__add__(other)

And here’s how it’s used:

17.9. Polymorphism

>>> print 1337 + start 10:07:17 Exercise 17.5. Write an add method for Points that works with either a Point object or a tuple: