The traceback identiﬁes the function that is currently running, and then the function that invoked it, and then the function that invoked that, and so on. In other words, it traces the

A.2. Runtime errors

sequence of function invocations that got you to where you are. It also includes the line number in your ﬁle where each of these calls occurs.

The ﬁrst step is to examine the place in the program where the error occurred and see if you can ﬁgure out what happened. These are some of the most common runtime errors:

NameError: You are trying to use a variable that doesn’t exist in the current environment. Remember that local variables are local. You cannot refer to them from outside the function where they are deﬁned.

TypeError: There are several possible causes:

You are trying to use a value improperly. Example: indexing a string, list, or tuple with something other than an integer.