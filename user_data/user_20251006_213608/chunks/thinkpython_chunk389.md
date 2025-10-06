This observation is the motivation for methods; a method is a function that is associated with a particular class. We have seen methods for strings, lists, dictionaries and tuples. In this chapter, we will deﬁne methods for user-deﬁned types.

Methods are semantically the same as functions, but there are two syntactic differences:

158

Chapter 17. Classes and methods

Methods are deﬁned inside a class deﬁnition in order to make the relationship be- tween the class and the method explicit.

The syntax for invoking a method is different from the syntax for calling a function.

In the next few sections, we will take the functions from the previous two chapters and transform them into methods. This transformation is purely mechanical; you can do it simply by following a sequence of steps. If you are comfortable converting from one form to another, you will be able to choose the best form for whatever you are doing.

17.2 Printing objects