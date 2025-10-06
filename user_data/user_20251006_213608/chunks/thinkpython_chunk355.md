14.10 Debugging

When you are reading and writing ﬁles, you might run into problems with whitespace. These errors can be hard to debug because spaces, tabs and newlines are normally invisible:

’

>>> s = >>> print s 1 2 3 4

1 2\t 3\n 4

’

The built-in function repr can help. It takes any object as an argument and returns a string representation of the object. For strings, it represents whitespace characters with backslash sequences:

>>> print repr(s) ’

’

1 2\t 3\n 4

14.11. Glossary

This can be helpful for debugging.

One other problem you might run into is that different systems use different characters to indicate the end of a line. Some systems use a newline, represented \n. Others use a return character, represented \r. Some use both. If you move ﬁles between different systems, these inconsistencies might cause problems.