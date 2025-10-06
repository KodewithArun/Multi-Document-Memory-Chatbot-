# velocity in meters/second.

Good variable names can reduce the need for comments, but long names can make com- plex expressions hard to read, so there is a tradeoff.

2.10 Debugging

At this point the syntax error you are most likely to make is an illegal variable name, like class and yield, which are keywords, or odd~job and US$, which contain illegal charac- ters.

3 is

2.11. Glossary

If you put a space in a variable name, Python thinks it is two operands without an operator:

>>> bad name = 5 SyntaxError: invalid syntax

For syntax errors, the error messages don’t help much. The most common messages are SyntaxError: invalid syntax and SyntaxError: invalid token, neither of which is very informative.

The runtime error you are most likely to make is a “use before def;” that is, trying to use a variable before you have assigned a value. This can happen if you spell a variable name wrong:

>>> principal = 327.68 >>> interest = principle * rate NameError: name

’

’

principle