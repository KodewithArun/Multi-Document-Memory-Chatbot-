The empty parentheses after the name indicate that this function doesn’t take any argu- ments.

The ﬁrst line of the function deﬁnition is called the header; the rest is called the body. The header has to end with a colon and the body has to be indented. By convention, the indentation is always four spaces (see Section 3.14). The body can contain any number of statements.

The strings in the print statements are enclosed in double quotes. Single quotes and double quotes do the same thing; most people use single quotes except in cases like this where a single quote (which is also an apostrophe) appears in the string.

If you type a function deﬁnition in interactive mode, the interpreter prints ellipses (...) to let you know that the deﬁnition isn’t complete:

21

22

Chapter 3. Functions

>>> def print_lyrics(): print "I ... ... print "I sleep all night and I work all day." ...

’

’

m a lumberjack, and I

m okay."