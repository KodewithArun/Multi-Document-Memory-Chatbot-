2. Write a function that prompts the user to input three stick lengths, converts them to integers, and uses is_triangle to check whether sticks with the given lengths can form a triangle.

The following exercises use TurtleWorld from Chapter 4: Exercise 5.5. Read the following function and see if you can ﬁgure out what it does. Then run it (see the examples in Chapter 4).

49

50

Chapter 5. Conditionals and recursion

Figure 5.2: A Koch curve.

def draw(t, length, n):

if n == 0: return angle = 50 fd(t, length*n) lt(t, angle) draw(t, length, n-1) rt(t, 2*angle) draw(t, length, n-1) lt(t, angle) bk(t, length*n)

Exercise 5.6. The Koch curve is a fractal that looks something like Figure 5.2. To draw a Koch curve with length x, all you have to do is

1. Draw a Koch curve with length x/3.

2. Turn left 60 degrees.

3. Draw a Koch curve with length x/3.

4. Turn right 120 degrees.

5. Draw a Koch curve with length x/3.

6. Turn left 60 degrees.

7. Draw a Koch curve with length x/3.