’

bad_file

)

’

’

bad_file

If you don’t have permission to access a ﬁle: >>> fout = open( IOError: [Errno 13] Permission denied:

’

’

’

’

/etc/passwd

,

w

)

’

/etc/passwd

’

And if you try to open a directory for reading, you get ) >>> fin = open( IOError: [Errno 21] Is a directory

’

’

/home

To avoid these errors, you could use functions like os.path.exists and os.path.isfile, but it would take a lot of time and code to check all the possibilities (if “Errno 21” is any indication, there are at least 21 things that can go wrong).

It is better to go ahead and try—and deal with problems if they happen—which is exactly what the try statement does. The syntax is similar to an if statement: try:

’

fin = open( for line in fin:

bad_file

’

)

print line

fin.close()

except:

print

’

Something went wrong.

’