def __str__(self):

’

return

%.2d:%.2d:%.2d

’

% (self.hour, self.minute, self.second)

When you print an object, Python invokes the str method:

>>> time = Time(9, 45) >>> print time 09:45:00

When I write a new class, I almost always start by writing __init__, which makes it easier to instantiate objects, and __str__, which is useful for debugging. Exercise 17.3. Write a str method for the Point class. Create a Point object and print it.

17.7 Operator overloading

By deﬁning other special methods, you can specify the behavior of operators on user- deﬁned types. For example, if you deﬁne a method named __add__ for the Time class, you can use the + operator on Time objects.

Here is what the deﬁnition might look like:

# inside class Time:

def __add__(self, other):

seconds = self.time_to_int() + other.time_to_int() return int_to_time(seconds)

And here is how you could use it:

>>> start = Time(9, 45) >>> duration = Time(1, 35) >>> print start + duration 11:20:00