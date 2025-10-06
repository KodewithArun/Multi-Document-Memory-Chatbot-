33

34

Chapter 4. Case study: interface design

Hint: ﬁgure out the circumference of the circle and make sure that length * n = circumference.

if bob is too slow for you, you can speed him up by changing Another hint: bob.delay, which is the time between moves, in seconds. bob.delay = 0.01 ought to get him moving.

5. Make a more general version of circle called arc that takes an additional parameter angle, which determines what fraction of a circle to draw. angle is in units of degrees, so when angle=360, arc should draw a complete circle.

4.4 Encapsulation

The ﬁrst exercise asks you to put your square-drawing code into a function deﬁnition and then call the function, passing the turtle as a parameter. Here is a solution:

def square(t):

for i in range(4): fd(t, 100) lt(t)

square(bob)