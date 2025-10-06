return word[-1]

def middle(word):

return word[1:-1]

We’ll see how they work in Chapter 8.

1. Type these functions into a ﬁle named palindrome.py and test them out. What happens if you call middle with a string with two letters? One letter? What about the empty string, which is written ’’

2. Write a function called is_palindrome that takes a string argument and returns True if it is a palindrome and False otherwise. Remember that you can use the built-in function len to check the length of a string.

Solution: http://thinkpython.com/code/palindrome_soln.py. Exercise 6.7. A number, a, is a power of b if it is divisible by b and a/b is a power of b. Write a function called is_power that takes parameters a and b and returns True if a is a power of b. Note: you will have to think about the base case. Exercise 6.8. The greatest common divisor (GCD) of a and b is the largest number that divides both of them with no remainder.