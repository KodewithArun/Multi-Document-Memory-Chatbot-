miles = 26.2 print miles * 1.61

This behavior can be confusing at ﬁrst.

A script usually contains a sequence of statements. If there is more than one statement, the results appear one at a time as the statements execute.

For example, the script

2.7. Order of operations

print 1 x = 2 print x

produces the output

1 2

The assignment statement produces no output. Exercise 2.1. Type the following statements in the Python interpreter to see what they do:

5 x = 5 x + 1

Now put the same statements into a script and run it. What is the output? Modify the script by transforming each expression into a print statement and then run it again.

2.7 Order of operations

When more than one operator appears in an expression, the order of evaluation depends on the rules of precedence. For mathematical operators, Python follows mathematical convention. The acronym PEMDAS is a useful way to remember the rules: