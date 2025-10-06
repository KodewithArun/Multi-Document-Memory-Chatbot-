def square(t):

for i in range(4): fd(t, 100) lt(t)

square(bob)

The innermost statements, fd and lt are indented twice to show that they are inside the for loop, which is inside the function deﬁnition. The next line, square(bob), is ﬂush with the left margin, so that is the end of both the for loop and the function deﬁnition.

Inside the function, t refers to the same turtle bob refers to, so lt(t) has the same effect as lt(bob). So why not call the parameter bob? The idea is that t can be any turtle, not just bob, so you could create a second turtle and pass it as an argument to square:

ray = Turtle() square(ray)

Wrapping a piece of code up in a function is called encapsulation. One of the beneﬁts of encapsulation is that it attaches a name to the code, which serves as a kind of documenta- tion. Another advantage is that if you re-use the code, it is more concise to call a function twice than to copy and paste the body!

4.5 Generalization