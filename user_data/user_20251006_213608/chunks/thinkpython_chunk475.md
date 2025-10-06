Something in your development environment is conﬁgured incorrectly.

A.2. Runtime errors

If you are writing a module and using import, make sure you don’t give your module the same name as one of the standard Python modules.

If you are using import to read a module, remember that you have to restart the interpreter or use reload to read a modiﬁed ﬁle. If you import the module again, it doesn’t do anything.

If you get stuck and you can’t ﬁgure out what is going on, one approach is to start again with a new program like “Hello, World!,” and make sure you can get a known program to run. Then gradually add the pieces of the original program to the new one.

A.2 Runtime errors

Once your program is syntactically correct, Python can compile it and at least start running it. What could possibly go wrong?

A.2.1 My program does absolutely nothing.