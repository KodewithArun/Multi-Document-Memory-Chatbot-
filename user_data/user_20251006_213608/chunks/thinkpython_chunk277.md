if n in known:

return known[n]

res = fibonacci(n-1) + fibonacci(n-2) known[n] = res return res

known is a dictionary that keeps track of the Fibonacci numbers we already know. It starts with two items: 0 maps to 0 and 1 maps to 1.

Whenever fibonacci is called, it checks known. If the result is already there, it can return immediately. Otherwise it has to compute the new value, add it to the dictionary, and return it. Exercise 11.6. Run this version of fibonacci and the original with a range of parameters and compare their run times. Exercise 11.7. Memoize the Ackermann function from Exercise 6.5 and see if memoization makes it possible to evaluate the function with bigger arguments. Hint: no. Solution: http: //thinkpython.com/code/ackermann_memo.py.

107

108

Chapter 11. Dictionaries

11.6 Global variables