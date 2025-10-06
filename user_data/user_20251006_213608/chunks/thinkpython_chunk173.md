def fibonacci (n): if n == 0:

return 0

elif

n == 1:

return 1

else:

return fibonacci(n-1) + fibonacci(n-2)

If you try to follow the ﬂow of execution here, even for fairly small values of n, your head explodes. But according to the leap of faith, if you assume that the two recursive calls work correctly, then it is clear that you get the right result by adding them together.

6.8 Checking types

What happens if we call factorial and give it 1.5 as an argument? >>> factorial(1.5) RuntimeError: Maximum recursion depth exceeded It looks like an inﬁnite recursion. But how can that be? There is a base case—when n == 0. But if n is not an integer, we can miss the base case and recurse forever.

In the ﬁrst recursive call, the value of n is 0.5. In the next, it is -0.5. From there, it gets smaller (more negative), but it will never be 0.