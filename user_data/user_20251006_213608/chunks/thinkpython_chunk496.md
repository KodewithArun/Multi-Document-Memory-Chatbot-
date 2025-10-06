Relative performance also depends on the size of the problem. A sorting algorithm that is fast for small lists might be slow for long lists. The usual solution to this problem is to express run time (or number of operations) as a function of problem size, and to compare the functions asymptotically as the problem size increases.

The good thing about this kind of comparison that it lends itself to simple classiﬁcation of algorithms. For example, if I know that the run time of Algorithm A tends to be propor- tional to the size of the input, n, and Algorithm B tends to be proportional to n2, then I expect A to be faster than B for large values of n.

This kind of analysis comes with some caveats, but we’ll get to that later.

B.1 Order of growth

Suppose you have analyzed two algorithms and expressed their run times in terms of the size of the input: Algorithm A takes 100n + 1 steps to solve a problem with size n; Algo- rithm B takes n2 + n + 1 steps.