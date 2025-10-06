All functions with the leading term n2 belong to O(n2); they are quadratic, which is a fancy word for functions with the leading term n2.

The following table shows some of the orders of growth that appear most commonly in algorithmic analysis, in increasing order of badness.

Order of growth O(1) O(logb n) O(n) O(nlogb n) O(n2) O(n3) O(cn)

Name

constant logarithmic (for any b) linear “en log en” quadratic cubic exponential (for any c)

For the logarithmic terms, the base of the logarithm doesn’t matter; changing bases is the equivalent of multiplying by a constant, which doesn’t change the order of growth. Sim- ilarly, all exponential functions belong to the same order of growth regardless of the base of the exponent. Exponential functions grow very quickly, so exponential algorithms are only useful for small problems. Exercise B.1. Read the Wikipedia page on Big-Oh notation at http://en.wikipedia.org/ wiki/Big_O_notation and answer the following questions: