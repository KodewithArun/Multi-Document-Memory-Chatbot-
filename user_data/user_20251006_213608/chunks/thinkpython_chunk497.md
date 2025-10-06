The following table shows the run time of these algorithms for different problem sizes:

Input

Run time of size Algorithm A Algorithm B 111 1 001 10 101 10 001 1 001 001 100 001 > 1010 1 000 001

Run time of

10 100 1 000 10 000

At n = 10, Algorithm A looks pretty bad; it takes almost 10 times longer than Algorithm B. But for n = 100 they are about the same, and for larger values A is much better.

The fundamental reason is that for large values of n, any function that contains an n2 term will grow faster than a function whose leading term is n. The leading term is the term with the highest exponent.

For Algorithm A, the leading term has a large coefﬁcient, 100, which is why B does better than A for small n. But regardless of the coefﬁcients, there will always be some value of n where an2 > bn.

The same argument applies to the non-leading terms. Even if the run time of Algorithm A were n + 1000000, it would still be better than Algorithm B for sufﬁciently large n.