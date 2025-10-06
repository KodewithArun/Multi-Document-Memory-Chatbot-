A for loop that traverses a sequence or dictionary is usually linear, as long as all of the operations in the body of the loop are constant time. For example, adding up the elements of a list is linear:

total = 0 for x in t:

total += x

The built-in function sum is also linear because it does the same thing, but it tends to be faster because it is a more efﬁcient implementation; in the language of algorithmic analysis, it has a smaller leading coefﬁcient.

If you use the same loop to “add” a list of strings, the run time is quadratic because string concatenation is linear.

The string method join is usually faster because it is linear in the total length of the strings.

As a rule of thumb, if the body of a loop is in O(na) then the whole loop is in O(na+1). The exception is if you can show that the loop exits after a constant number of iterations. If a loop runs k times regardless of n, then the loop is in O(na), even for large k.