In general, we expect an algorithm with a smaller leading term to be a better algorithm for large problems, but for smaller problems, there may be a crossover point where another algorithm is better. The location of the crossover point depends on the details of the algo- rithms, the inputs, and the hardware, so it is usually ignored for purposes of algorithmic analysis. But that doesn’t mean you can forget about it.

If two algorithms have the same leading order term, it is hard to say which is better; again, the answer depends on the details. So for algorithmic analysis, functions with the same leading term are considered equivalent, even if they have different coefﬁcients.

B.1. Order of growth

An order of growth is a set of functions whose asymptotic growth behavior is considered equivalent. For example, 2n, 100n and n + 1 belong to the same order of growth, which is written O(n) in Big-Oh notation and often called linear because every function in the set grows linearly with n.