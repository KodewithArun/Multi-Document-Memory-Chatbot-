4.8. A development plan

Finally, we can rewrite circle to use arc:

def circle(t, r):

arc(t, r, 360)

This process—rearranging a program to improve function interfaces and facilitate code re- use—is called refactoring. In this case, we noticed that there was similar code in arc and polygon, so we “factored it out” into polyline.

If we had planned ahead, we might have written polyline ﬁrst and avoided refactoring, but often you don’t know enough at the beginning of a project to design all the interfaces. Once you start coding, you understand the problem better. Sometimes refactoring is a sign that you have learned something.

4.8 A development plan

A development plan is a process for writing programs. The process we used in this case study is “encapsulation and generalization.” The steps of this process are:

1. Start by writing a small program with no function deﬁnitions.

2. Once you get the program working, encapsulate it in a function and give it a name.