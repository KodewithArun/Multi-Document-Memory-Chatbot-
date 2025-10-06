If the function seems to be working, look at the function call to make sure the return value is being used correctly (or used at all!).

Adding print statements at the beginning and end of a function can help make the ﬂow of execution more visible. For example, here is a version of factorial with print statements:

def factorial(n):

’ ’

space = print space, if n == 0:

(4 * n) ’

factorial

’

, n

print space, return 1

’

returning 1

’

else:

recurse = factorial(n-1) result = n * recurse print space, return result

’

returning

’

, result

space is a string of space characters that controls the indentation of the output. Here is the result of factorial(5) :

59

60

Chapter 6. Fruitful functions

factorial 5

factorial 4

factorial 3

factorial 2

factorial 1

factorial 0 returning 1

returning 1

returning 2

returning 6

returning 24

returning 120