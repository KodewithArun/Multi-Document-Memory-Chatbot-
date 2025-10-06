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

The mode means that the database should be created if it doesn’t already exist. The result is a database object that can be used (for most operations) like a dictionary. If you create a new item, anydbm updates the database ﬁle.

c

>>> db[

’

cleese.png

’

] =

’

Photo of John Cleese.

’

When you access one of the items, anydbm reads the ﬁle:

’

>>> print db[ Photo of John Cleese.

cleese.png

’

]

If you make another assignment to an existing key, anydbm replaces the old value:

’

’

’

>>> db[ >>> print db[ Photo of John Cleese doing a silly walk.

] =

cleese.png ’

Photo of John Cleese doing a silly walk. ’

cleese.png

]

’

Many dictionary methods, like keys and items, also work with database objects. So does iteration with a for statement.

for key in db:

print key

As with other ﬁles, you should close the database when you are done:

>>> db.close()

14.7 Pickling