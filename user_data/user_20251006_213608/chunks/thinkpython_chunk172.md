The same is true of recursive programs. When you get to the recursive call, instead of following the ﬂow of execution, you should assume that the recursive call works (yields the correct result) and then ask yourself, “Assuming that I can ﬁnd the factorial of n − 1, can I compute the factorial of n?” In this case, it is clear that you can, by multiplying by n.

Of course, it’s a bit strange to assume that the function works correctly when you haven’t ﬁnished writing it, but that’s why it’s called a leap of faith!

6.7 One more example

After factorial, the most common example of a recursively deﬁned mathematical func- tion is fibonacci, which has the following deﬁnition (see http://en.wikipedia.org/ wiki/Fibonacci_number):

ﬁbonacci(0) = 0 ﬁbonacci(1) = 1 ﬁbonacci(n) = ﬁbonacci(n − 1) + ﬁbonacci(n − 2)

Translated into Python, it looks like this:

57

58

Chapter 6. Fruitful functions

def fibonacci (n): if n == 0:

return 0

elif

n == 1:

return 1

else: