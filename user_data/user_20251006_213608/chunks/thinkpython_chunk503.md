Multiplying by k doesn’t change the order of growth, but neither does dividing. So if the body of a loop is in O(na) and it runs n/k times, the loop is in O(na+1), even for large k.

Most string and tuple operations are linear, except indexing and len, which are constant time. The built-in functions min and max are linear. The run-time of a slice operation is proportional to the length of the output, but independent of the size of the input.

All string methods are linear, but if the lengths of the strings are bounded by a constant— for example, operations on single characters—they are considered constant time.

Most list methods are linear, but there are some exceptions:

Adding an element to the end of a list is constant time on average; when it runs out of room it occasionally gets copied to a bigger location, but the total time for n operations is O(n), so we say that the “amortized” time for one operation is O(1).

Removing an element from the end of a list is constant time.