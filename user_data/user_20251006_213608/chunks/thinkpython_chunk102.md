3.9 Variables and parameters are local

When you create a variable inside a function, it is local, which means that it only exists inside the function. For example: def cat_twice(part1, part2): cat = part1 + part2 print_twice(cat)

This function takes two arguments, concatenates them, and prints the result twice. Here is an example that uses it: >>> line1 = >>> line2 = >>> cat_twice(line1, line2) Bing tiddle tiddle bang. Bing tiddle tiddle bang.

’ ’

’ ’

Bing tiddle tiddle bang.

When cat_twice terminates, the variable cat is destroyed. If we try to print it, we get an exception: >>> print cat NameError: name

’

’

cat

is not defined

3.10. Stack diagrams

line1line2’tiddle bang.’part1part2catbruce’Bing tiddle ’’Bing tiddle ’’tiddle bang.’’Bing tiddle tiddle bang.’’Bing tiddle tiddle bang.’<module>cat_twiceprint_twice

Figure 3.1: Stack diagram.

Parameters are also local. For example, outside print_twice, there is no such thing as bruce.

3.10 Stack diagrams