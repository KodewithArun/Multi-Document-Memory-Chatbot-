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

Python starts by executing the try clause. If all goes well, it skips the except clause and proceeds. If an exception occurs, it jumps out of the try clause and executes the except clause.

Handling an exception with a try statement is called catching an exception. In this exam- ple, the except clause prints an error message that is not very helpful. In general, catching an exception gives you a chance to ﬁx the problem, or try again, or at least end the program gracefully. Exercise 14.2. Write a function called sed that takes as arguments a pattern string, a replacement string, and two ﬁlenames; it should read the ﬁrst ﬁle and write the contents into the second ﬁle (creating it if necessary). If the pattern string appears anywhere in the ﬁle, it should be replaced with the replacement string.

14.6. Databases