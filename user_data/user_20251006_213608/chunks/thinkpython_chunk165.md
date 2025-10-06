def circle_area(xc, yc, xp, yp):

return area(distance(xc, yc, xp, yp))

6.4 Boolean functions

Functions can return booleans, which is often convenient for hiding complicated tests in- side functions. For example:

def is_divisible(x, y): if x % y == 0:

return True

else:

return False

6.5. More recursion

It is common to give boolean functions names that sound like yes/no questions; is_divisible returns either True or False to indicate whether x is divisible by y.

Here is an example: >>> False >>> True The result of the == operator is a boolean, so we can write the function more concisely by returning it directly: def is_divisible(x, y):

is_divisible(6, 4)

is_divisible(6, 3)

return x % y == 0

Boolean functions are often used in conditional statements: if is_divisible(x, y): ’

’

print

x is divisible by y

It might be tempting to write something like: if is_divisible(x, y) == True: x is divisible by y

’

’

print