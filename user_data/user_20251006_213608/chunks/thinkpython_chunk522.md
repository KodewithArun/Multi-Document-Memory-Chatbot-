def countdown(n): if n <= 0:

’

’

print Blastoff! lumpy.object_diagram()

else:

print n countdown(n-1)

lumpy = Lumpy() lumpy.make_reference() countdown(3)

Figure C.2 shows the result. Each frame is represented with a box that has the function’s name outside and variables inside. Since this function is recursive, there is one frame for each level of recursion.

Remember that a stack diagram shows the state of the program at a particular point in its execution. To get the diagram you want, sometimes you have to think about where to invoke object_diagram.

In this case I invoke object_diagram after executing the base case of the recursion; that way the stack diagram shows each level of the recursion. You can call object_diagram more than once to get a series of snapshots of the program’s execution.

C.3 Object diagrams