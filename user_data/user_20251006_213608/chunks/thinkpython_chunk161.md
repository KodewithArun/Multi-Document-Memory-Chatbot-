At this point we have conﬁrmed that the function is syntactically correct, and we can start adding code to the body. A reasonable next step is to ﬁnd the differences x2 − x1 and y2 − y1. The next version stores those values in temporary variables and prints them. def distance(x1, y1, x2, y2):

dx = x2 - x1 dy = y2 - y1 ’ dx is print ’ print dy is return 0.0

’ ’

, dx , dy

’

’

and ’dy is 4’. If so, we know that If the function is working, it should display the function is getting the right arguments and performing the ﬁrst computation correctly. If not, there are only a few lines to check.

dx is 3

Next we compute the sum of squares of dx and dy:

def distance(x1, y1, x2, y2):

dx = x2 - x1 dy = y2 - y1 dsquared = dx**2 + dy**2 print return 0.0

’

’

dsquared is:

, dsquared

Again, you would run the program at this stage and check the output (which should be 25). Finally, you can use math.sqrt to compute and return the result:

def distance(x1, y1, x2, y2):