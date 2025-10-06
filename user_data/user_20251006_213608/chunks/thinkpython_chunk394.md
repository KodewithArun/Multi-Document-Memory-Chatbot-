def is_after(self, other):

return self.time_to_int() > other.time_to_int()

To use this method, you have to invoke it on one object and pass the other as an argument: >>> end.is_after(start) True

One nice thing about this syntax is that it almost reads like English: “end is after start?”

17.5 The init method

The init method (short for “initialization”) is a special method that gets invoked when an object is instantiated. Its full name is __init__ (two underscore characters, followed by init, and then two more underscores). An init method for the Time class might look like this: # inside class Time:

def __init__(self, hour=0, minute=0, second=0):

self.hour = hour self.minute = minute self.second = second

It is common for the parameters of __init__ to have the same names as the attributes. The statement

self.hour = hour

stores the value of the parameter hour as an attribute of self.