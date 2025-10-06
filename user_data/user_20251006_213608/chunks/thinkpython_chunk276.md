To understand why, consider Figure 11.2, which shows the call graph for fibonacci with n=4:

A call graph shows a set of function frames, with lines connecting each frame to the frames of the functions it calls. At the top of the graph, fibonacci with n=4 calls fibonacci with n=3 and n=2. In turn, fibonacci with n=3 calls fibonacci with n=2 and n=1. And so on.

Count how many times fibonacci(0) and fibonacci(1) are called. This is an inefﬁcient solution to the problem, and it gets worse as the argument gets bigger.

One solution is to keep track of values that have already been computed by storing them in a dictionary. A previously computed value that is stored for later use is called a memo. Here is a “memoized” version of fibonacci:

known = {0:0, 1:1}

def fibonacci(n):

if n in known:

return known[n]

res = fibonacci(n-1) + fibonacci(n-2) known[n] = res return res