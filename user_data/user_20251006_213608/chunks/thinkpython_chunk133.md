docstring: A string that appears in a function deﬁnition to document the function’s inter-

face.

precondition: A requirement that should be satisﬁed by the caller before a function starts.

postcondition: A requirement that should be satisﬁed by the function before it ends.

4.12 Exercises

Exercise 4.1. Download the code in this chapter from http://thinkpython.com/code/ polygon.py.

1. Write appropriate docstrings for polygon, arc and circle.

2. Draw a stack diagram that shows the state of the program while executing circle(bob, radius). You can do the arithmetic by hand or add print statements to the code.

3. The version of arc in Section 4.7 is not very accurate because the linear approximation of the circle is always outside the true circle. As a result, the turtle ends up a few units away from the correct destination. My solution shows a way to reduce the effect of this error. Read the code and see if it makes sense to you. If you draw a diagram, you might see how it works.