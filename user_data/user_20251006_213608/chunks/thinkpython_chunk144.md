The countdown that got n=2 returns.

The countdown that got n=3 returns.

And then you’re back in __main__. So, the total output looks like this:

3 2 1 Blastoff!

A function that calls itself is recursive; the process is called recursion.

As another example, we can write a function that prints a string n times.

def print_n(s, n): if n <= 0: return

print s print_n(s, n-1)

If n <= 0 the return statement exits the function. The ﬂow of execution immediately re- turns to the caller, and the remaining lines of the function are not executed.

The rest of the function is similar to countdown: if n is greater than 0, it displays s and then calls itself to display s n − 1 additional times. So the number of lines of output is 1 + (n - 1), which adds up to n.

For simple examples like this, it is probably easier to use a for loop. But we will see examples later that are hard to write with a for loop and easy to write with recursion, so it is good to start early.