while True: print x y = (x + a/x) / 2 if y == x:

break

x = y

For most values of a this works ﬁne, but in general it is dangerous to test float equality. Floating-point values are only approximately right: most rational numbers, like 1/3, and irrational numbers, like

√

2, can’t be represented exactly with a float.

Rather than checking whether x and y are exactly equal, it is safer to use the built-in func- tion abs to compute the absolute value, or magnitude, of the difference between them:

if abs(y-x) < epsilon:

break

Where epsilon has a value like 0.0000001 that determines how close is close enough. Exercise 7.2. Encapsulate this loop in a function called square_root that takes a as a parameter, chooses a reasonable value of x, and returns an estimate of the square root of a.

7.6 Algorithms

Newton’s method is an example of an algorithm: it is a mechanical process for solving a category of problems (in this case, computing square roots).