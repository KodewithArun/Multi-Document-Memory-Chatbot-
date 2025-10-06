But if you keep those caveats in mind, algorithmic analysis is a useful tool. At least for large problems, the “better” algorithms is usually better, and sometimes it is much better. The difference between two algorithms with the same order of growth is usually a constant factor, but the difference between a good algorithm and a bad algorithm is unbounded!

203

204

Appendix B. Analysis of Algorithms

B.2 Analysis of basic Python operations

Most arithmetic operations are constant time; multiplication usually takes longer than ad- dition and subtraction, and division takes even longer, but these run times don’t depend on the magnitude of the operands. Very large integers are an exception; in that case the run time increases with the number of digits.

Indexing operations—reading or writing elements in a sequence or dictionary—are also constant time, regardless of the size of the data structure.