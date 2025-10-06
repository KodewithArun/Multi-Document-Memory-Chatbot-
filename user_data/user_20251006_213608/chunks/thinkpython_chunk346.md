14.6. Databases

If an error occurs while opening, reading, writing or closing ﬁles, your program should catch the exception, print an error message, and exit. Solution: http://thinkpython.com/code/sed. py.

14.6 Databases

A database is a ﬁle that is organized for storing data. Most databases are organized like a dictionary in the sense that they map from keys to values. The biggest difference is that the database is on disk (or other permanent storage), so it persists after the program ends.

The module anydbm provides an interface for creating and updating database ﬁles. As an example, I’ll create a database that contains captions for image ﬁles.

Opening a database is similar to opening other ﬁles:

>>> import anydbm >>> db = anydbm.open( ’

’

’

’

’

c

,

captions.db

)

’