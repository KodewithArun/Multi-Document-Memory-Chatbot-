The second (and more concise) way is to use method syntax: >>> start.print_time() 09:45:00

In this use of dot notation, print_time is the name of the method (again), and start is the object the method is invoked on, which is called the subject. Just as the subject of a sentence is what the sentence is about, the subject of a method invocation is what the method is about.

Inside the method, the subject is assigned to the ﬁrst parameter, so in this case start is assigned to time.

17.3. Another example

By convention, the ﬁrst parameter of a method is called self, so it would be more common to write print_time like this:

class Time(object):

def print_time(self): ’

print

%.2d:%.2d:%.2d

’

% (self.hour, self.minute, self.second)

The reason for this convention is an implicit metaphor:

The syntax for a function call, print_time(start), suggests that the function is the active agent. It says something like, “Hey print_time! Here’s an object for you to print.”