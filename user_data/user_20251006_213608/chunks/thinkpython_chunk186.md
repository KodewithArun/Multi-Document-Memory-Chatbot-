1. Evaluate the condition, yielding True or False.

7.4. break

2. If the condition is false, exit the while statement and continue execution at the next statement.

3. If the condition is true, execute the body and then go back to step 1.

This type of ﬂow is called a loop because the third step loops back around to the top.

The body of the loop should change the value of one or more variables so that eventu- ally the condition becomes false and the loop terminates. Otherwise the loop will repeat forever, which is called an inﬁnite loop. An endless source of amusement for computer scientists is the observation that the directions on shampoo, “Lather, rinse, repeat,” are an inﬁnite loop.

In the case of countdown, we can prove that the loop terminates because we know that the value of n is ﬁnite, and we can see that the value of n gets smaller each time through the loop, so eventually we have to get to 0. In other cases, it is not so easy to tell:

def sequence(n):

while n != 1: