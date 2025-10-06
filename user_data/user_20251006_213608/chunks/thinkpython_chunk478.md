For example:

while x > 0 and y < 0 : # do something to x # do something to y

print "x: ", x print "y: ", y print "condition: ", (x > 0 and y < 0)

Now when you run the program, you will see three lines of output for each time through the loop. The last time through the loop, the condition should be false. If the loop keeps going, you will be able to see the values of x and y, and you might ﬁgure out why they are not being updated correctly.

Inﬁnite Recursion

Most of the time, an inﬁnite recursion will cause the program to run for a while and then produce a Maximum recursion depth exceeded error.

If you suspect that a function or method is causing an inﬁnite recursion, start by checking to make sure that there is a base case. In other words, there should be some condition that will cause the function or method to return without making a recursive invocation. If not, then you need to rethink the algorithm and identify a base case.