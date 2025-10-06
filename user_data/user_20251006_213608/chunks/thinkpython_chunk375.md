’

’

%.2d

16.2 Pure functions

In the next few sections, we’ll write two functions that add time values. They demonstrate two kinds of functions: pure functions and modiﬁers. They also demonstrate a develop- ment plan I’ll call prototype and patch, which is a way of tackling a complex problem by starting with a simple prototype and incrementally dealing with the complications.

152

Chapter 16. Classes and functions

5930hourminutesecond11Timetime

Figure 16.1: Object diagram.

Here is a simple prototype of add_time:

def add_time(t1, t2): sum = Time() sum.hour = t1.hour + t2.hour sum.minute = t1.minute + t2.minute sum.second = t1.second + t2.second return sum

The function creates a new Time object, initializes its attributes, and returns a reference to the new object. This is called a pure function because it does not modify any of the objects passed to it as arguments and it has no effect, like displaying a value or getting user input, other than returning a value.