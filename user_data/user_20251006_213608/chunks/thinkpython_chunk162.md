def distance(x1, y1, x2, y2):

dx = x2 - x1 dy = y2 - y1 dsquared = dx**2 + dy**2 result = math.sqrt(dsquared) return result

If that works correctly, you are done. Otherwise, you might want to print the value of result before the return statement.

The ﬁnal version of the function doesn’t display anything when it runs; it only returns a value. The print statements we wrote are useful for debugging, but once you get the function working, you should remove them. Code like that is called scaffolding because it is helpful for building the program but is not part of the ﬁnal product.

When you start out, you should add only a line or two of code at a time. As you gain more experience, you might ﬁnd yourself writing and debugging bigger chunks. Either way, incremental development can save you a lot of debugging time.

The key aspects of the process are: