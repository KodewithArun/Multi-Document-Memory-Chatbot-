y =

x + a/x 2

For example, if a is 4 and x is 3:

>>> a = 4.0 >>> x = 3.0 >>> y = (x + a/x) / 2 >>> print y 2.16666666667

Which is closer to the correct answer ( estimate, it gets even closer:

√

4 = 2). If we repeat the process with the new

>>> x = y >>> y = (x + a/x) / 2 >>> print y 2.00641025641

After a few more updates, the estimate is almost exact:

7.6. Algorithms

>>> x = y >>> y = (x + a/x) / 2 >>> print y 2.00001024003 >>> x = y >>> y = (x + a/x) / 2 >>> print y 2.00000000003

In general we don’t know ahead of time how many steps it takes to get to the right answer, but we know when we get there because the estimate stops changing:

>>> x = y >>> y = (x + a/x) / 2 >>> print y 2.0 >>> x = y >>> y = (x + a/x) / 2 >>> print y 2.0

When y == x, we can stop. Here is a loop that starts with an initial estimate, x, and im- proves it until it stops changing:

while True: print x y = (x + a/x) / 2 if y == x:

break

x = y