def __add__(self, other):

if isinstance(other, Time):

return self.add_time(other)

else:

return self.increment(other)

def add_time(self, other):

seconds = self.time_to_int() + other.time_to_int() return int_to_time(seconds)

def increment(self, seconds):

seconds += self.time_to_int() return int_to_time(seconds)

The built-in function isinstance takes a value and a class object, and returns True if the value is an instance of the class.

If other is a Time object, __add__ invokes add_time. Otherwise it assumes that the param- eter is a number and invokes increment. This operation is called a type-based dispatch because it dispatches the computation to different methods based on the type of the argu- ments.

Here are examples that use the + operator with different types: >>> start = Time(9, 45) >>> duration = Time(1, 35) >>> print start + duration 11:20:00 >>> print start + 1337 10:07:17