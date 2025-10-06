Here’s how you would invoke increment:

>>> start.print_time() 09:45:00 >>> end = start.increment(1337) >>> end.print_time() 10:07:17

The subject, start, gets assigned to the ﬁrst parameter, self. The argument, 1337, gets assigned to the second parameter, seconds.

This mechanism can be confusing, especially if you make an error. For example, if you invoke increment with two arguments, you get:

>>> end = start.increment(1337, 460) TypeError: increment() takes exactly 2 arguments (3 given)

The error message is initially confusing, because there are only two arguments in paren- theses. But the subject is also considered an argument, so all together that’s three.

159

160

Chapter 17. Classes and methods

17.4 A more complicated example

is_after (from Exercise 16.2) is slightly more complicated because it takes two Time ob- jects as parameters. In this case it is conventional to name the ﬁrst parameter self and the second parameter other: # inside class Time: