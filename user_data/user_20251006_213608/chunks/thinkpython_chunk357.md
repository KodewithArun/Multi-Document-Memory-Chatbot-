relative path: A path that starts from the current directory.

absolute path: A path that starts from the topmost directory in the ﬁle system.

catch: To prevent an exception from terminating a program using the try and except state-

ments.

database: A ﬁle whose contents are organized like a dictionary with keys that correspond

to values.

14.12 Exercises

Exercise 14.6. The urllib module provides methods for manipulating URLs and downloading information from the web. The following example downloads and prints a secret message from thinkpython.com: import urllib

conn = urllib.urlopen( for line in conn:

’

http://thinkpython.com/secret.html

’

)

print line.strip()

Run this code and follow the instructions you see there. Solution: http://thinkpython.com/ code/zip_code.py.

141

142

Chapter 14. Files

Chapter 15

Classes and objects