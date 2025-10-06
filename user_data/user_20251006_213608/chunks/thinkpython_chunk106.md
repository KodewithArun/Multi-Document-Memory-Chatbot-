Void functions might display something on the screen or have some other effect, but they don’t have a return value. If you try to assign the result to a variable, you get a special value called None.

>>> result = print_twice( Bing Bing >>> print result None

’

Bing

’

)

The value None is not the same as the string type:

’

None

’

. It is a special value that has its own

>>> print type(None) <type

’

’

NoneType

>

The functions we have written so far are all void. We will start writing fruitful functions in a few chapters.

3.12 Why functions?

It may not be clear why it is worth the trouble to divide a program into functions. There are several reasons:

Creating a new function gives you an opportunity to name a group of statements, which makes your program easier to read and debug.

Functions can make a program smaller by eliminating repetitive code. Later, if you make a change, you only have to make it in one place.

3.13. Importing with from