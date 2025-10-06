In object-oriented programming, the objects are the active agents. A method invoca- tion like start.print_time() says “Hey start! Please print yourself.”

This change in perspective might be more polite, but it is not obvious that it is useful. In the examples we have seen so far, it may not be. But sometimes shifting responsibility from the functions onto the objects makes it possible to write more versatile functions, and makes it easier to maintain and reuse code. Exercise 17.1. Rewrite time_to_int (from Section 16.4) as a method. It is probably not appro- priate to rewrite int_to_time as a method; what object you would invoke it on?

17.3 Another example

Here’s a version of increment (from Section 16.3) rewritten as a method:

# inside class Time:

def increment(self, seconds):

seconds += self.time_to_int() return int_to_time(seconds)

This version assumes that time_to_int is written as a method, as in Exercise 17.1. Also, note that it is a pure function, not a modiﬁer.