The mathematical operators work on long integers, and the functions in the math module, too, so in general any code that works with int will also work with long.

Any time the result of a computation is too big to be represented with an integer, Python converts the result as a long integer:

>>> 1000 * 1000 1000000 >>> 100000 * 100000 10000000000L

In the ﬁrst case the result has type int; in the second case it is long. Exercise 11.8. Exponentiation of large integers is the basis of common algorithms for public-key en- cryption. Read the Wikipedia page on the RSA algorithm (http://en.wikipedia.org/wiki/ RSA_(algorithm)) and write functions to encode and decode messages.

11.8 Debugging

As you work with bigger datasets it can become unwieldy to debug by printing and check- ing data by hand. Here are some suggestions for debugging large datasets: