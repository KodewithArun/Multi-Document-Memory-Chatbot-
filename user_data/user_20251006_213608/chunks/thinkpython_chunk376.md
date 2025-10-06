To test this function, I’ll create two Time objects: start contains the start time of a movie, like Monty Python and the Holy Grail, and duration contains the run time of the movie, which is one hour 35 minutes.

add_time ﬁgures out when the movie will be done.

>>> start = Time() >>> start.hour = 9 >>> start.minute = 45 >>> start.second = 0

>>> duration = Time() >>> duration.hour = 1 >>> duration.minute = 35 >>> duration.second = 0

>>> done = add_time(start, duration) >>> print_time(done) 10:80:00

The result, 10:80:00 might not be what you were hoping for. The problem is that this function does not deal with cases where the number of seconds or minutes adds up to more than sixty. When that happens, we have to “carry” the extra seconds into the minute column or the extra minutes into the hour column.

Here’s an improved version:

def add_time(t1, t2): sum = Time() sum.hour = t1.hour + t2.hour sum.minute = t1.minute + t2.minute sum.second = t1.second + t2.second

16.3. Modiﬁers