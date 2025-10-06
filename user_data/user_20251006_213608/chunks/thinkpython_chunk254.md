t.append(x) t = t + [x]

And these are wrong:

t.append([x]) t = t.append(x) t + [x] t = t + x

# WRONG! # WRONG! # WRONG! # WRONG!

Try out each of these examples in interactive mode to make sure you understand what they do. Notice that only the last one causes a runtime error; the other three are legal, but they do the wrong thing.

3. Make copies to avoid aliasing.

If you want to use a method like sort that modiﬁes the argument, but you need to keep the original list as well, you can make a copy.

orig = t[:] t.sort()

In this example you could also use the built-in function sorted, which returns a new, sorted list and leaves the original alone. But in that case you should avoid using sorted as a variable name!

10.14 Glossary

list: A sequence of values.

element: One of the values in a list (or other sequence), also called items.

index: An integer value that indicates an element in a list.

nested list: A list that is an element of another list.