17.2 Printing objects

In Chapter 16, we deﬁned a class named Time and in Exercise 16.1, you wrote a function named print_time: class Time(object):

"""Represents the time of day."""

def print_time(time): ’

print

%.2d:%.2d:%.2d

’

% (time.hour, time.minute, time.second)

To call this function, you have to pass a Time object as an argument: >>> start = Time() >>> start.hour = 9 >>> start.minute = 45 >>> start.second = 00 >>> print_time(start) 09:45:00

To make print_time a method, all we have to do is move the function deﬁnition inside the class deﬁnition. Notice the change in indentation. class Time(object):

def print_time(time): ’

print

%.2d:%.2d:%.2d

’

% (time.hour, time.minute, time.second)

Now there are two ways to call print_time. The ﬁrst (and less common) way is to use function syntax: >>> Time.print_time(start) 09:45:00

In this use of dot notation, Time is the name of the class, and print_time is the name of the method. start is passed as a parameter.