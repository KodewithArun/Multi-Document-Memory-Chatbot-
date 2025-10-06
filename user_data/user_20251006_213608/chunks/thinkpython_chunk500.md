1. What is the order of growth of n3 + n2? What about 1000000n3 + n2? What about n3 + 1000000n2?

2. What is the order of growth of (n2 + n) · (n + 1)? Before you start multiplying, remember that you only need the leading term.

3. If f is in O(g), for some unspeciﬁed function g, what can we say about af + b?

4. If f1 and f2 are in O(g), what can we say about f1 + f2?

5. If f1 is in O(g) and f2 is in O(h), what can we say about f1 + f2?

6. If f1 is in O(g) and f2 is O(h), what can we say about f1 · f2?

Programmers who care about performance often ﬁnd this kind of analysis hard to swal- low. They have a point: sometimes the coefﬁcients and the non-leading terms make a real difference. Sometimes the details of the hardware, the programming language, and the characteristics of the input make a big difference. And for small problems asymptotic behavior is irrelevant.