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

To demonstrate these functions, the following example “walks” through a directory, prints the names of all the ﬁles, and calls itself recursively on all the directories.

def walk(dirname):

for name in os.listdir(dirname):

path = os.path.join(dirname, name)

135

136

Chapter 14. Files

if os.path.isfile(path):

print path

else:

walk(path)

os.path.join takes a directory and a ﬁle name and joins them into a complete path. Exercise 14.1. The os module provides a function called walk that is similar to this one but more versatile. Read the documentation and use it to print the names of the ﬁles in a given directory and its subdirectories.

Solution: http://thinkpython.com/code/walk.py.

14.5 Catching exceptions

A lot of things can go wrong when you try to read and write ﬁles. If you try to open a ﬁle that doesn’t exist, you get an IOError: ’ >>> fin = open( IOError: [Errno 2] No such file or directory:

’