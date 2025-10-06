3. To double-check, you can use the Unix command diff.

Solution: http://thinkpython.com/code/find_duplicates.py.

14.9 Writing modules

Any ﬁle that contains Python code can be imported as a module. For example, suppose you have a ﬁle named wc.py with the following code: def linecount(filename):

count = 0 for line in open(filename):

count += 1

return count

print linecount(

’

wc.py

’

)

139

140

Chapter 14. Files

If you run this program, it reads itself and prints the number of lines in the ﬁle, which is 7. You can also import it like this:

>>> import wc 7

Now you have a module object wc:

>>> print wc ’ <module

’

wc

from

’

wc.py

’

>

That provides a function called linecount: ’

’

>>> wc.linecount( 7

wc.py

)

So that’s how you write modules in Python.

The only problem with this example is that when you import the module it executes the test code at the bottom. Normally when you import a module, it deﬁnes new functions but it doesn’t execute them.