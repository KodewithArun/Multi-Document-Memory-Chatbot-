def factorial(n): if n == 0:

return 1

Otherwise, and this is the interesting part, we have to make a recursive call to ﬁnd the factorial of n − 1 and then multiply it by n:

def factorial(n): if n == 0:

return 1

else:

recurse = factorial(n-1) result = n * recurse return result

The ﬂow of execution for this program is similar to the ﬂow of countdown in Section 5.8. If we call factorial with the value 3:

Since 3 is not 0, we take the second branch and calculate the factorial of n-1...

Since 2 is not 0, we take the second branch and calculate the factorial of n-1...

Since 1 is not 0, we take the second branch and calculate the factorial of n-1...

Since 0 is 0, we take the ﬁrst branch and return 1 without making any more recursive calls.

The return value (1) is multiplied by n, which is 1, and the result is returned.

The return value (1) is multiplied by n, which is 2, and the result is returned.