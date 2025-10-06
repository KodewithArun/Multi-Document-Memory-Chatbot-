>>> start = Time(9, 45) >>> duration = Time(1, 35) >>> print start + duration 11:20:00

When you apply the + operator to Time objects, Python invokes __add__. When you print the result, Python invokes __str__. So there is quite a lot happening behind the scenes!

Changing the behavior of an operator so that it works with user-deﬁned types is called op- erator overloading. For every operator in Python there is a corresponding special method, like __add__. For more details, see http://docs.python.org/2/reference/datamodel. html#specialnames. Exercise 17.4. Write an add method for the Point class.

161

162

Chapter 17. Classes and methods

17.8 Type-based dispatch

In the previous section we added two Time objects, but you also might want to add an integer to a Time object. The following is a version of __add__ that checks the type of other and invokes either add_time or increment: # inside class Time:

def __add__(self, other):

if isinstance(other, Time):

return self.add_time(other)