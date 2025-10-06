A string like cwd that identiﬁes a ﬁle is called a path. A relative path starts from the current directory; an absolute path starts from the topmost directory in the ﬁle system.

The paths we have seen so far are simple ﬁlenames, so they are relative to the current directory. To ﬁnd the absolute path to a ﬁle, you can use os.path.abspath:

’

>>> os.path.abspath( ’

memo.txt ’

/home/dinsdale/memo.txt

’

)

os.path.exists checks whether a ﬁle or directory exists:

>>> os.path.exists( True

’

memo.txt

’

)

If it exists, os.path.isdir checks whether it’s a directory:

>>> os.path.isdir( False >>> os.path.isdir( True

’

’

memo.txt

music

’

)

’

)

Similarly, os.path.isfile checks whether it’s a ﬁle.

os.listdir returns a list of the ﬁles (and other directories) in the given directory:

>>> os.listdir(cwd) , [

’

’

’

’

music

,

photos

’

memo.txt

’

]