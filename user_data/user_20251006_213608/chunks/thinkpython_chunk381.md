minutes = time.hour * 60 + time.minute seconds = minutes * 60 + time.second return seconds

And here is the function that converts integers to Times (recall that divmod divides the ﬁrst argument by the second and returns the quotient and remainder as a tuple). def int_to_time(seconds):

time = Time() minutes, time.second = divmod(seconds, 60) time.hour, time.minute = divmod(minutes, 60) return time

You might have to think a bit, and run some tests, to convince yourself that these functions are correct. One way to test them is to check that time_to_int(int_to_time(x)) == x for many values of x. This is an example of a consistency check.

Once you are convinced they are correct, you can use them to rewrite add_time: def add_time(t1, t2):

seconds = time_to_int(t1) + time_to_int(t2) return int_to_time(seconds)

This version is shorter than the original, and easier to verify. Exercise 16.5. Rewrite increment using time_to_int and int_to_time.