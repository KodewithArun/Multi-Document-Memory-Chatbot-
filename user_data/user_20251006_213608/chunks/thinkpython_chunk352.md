You can use a pipe to run md5sum from Python and get the result: >>> filename = >>> cmd = >>> fp = os.popen(cmd) >>> res = fp.read() >>> stat = fp.close() >>> print res 1e0033f0ed0656636de0d75144ba32e0 book.tex >>> print stat None Exercise 14.4. In a large collection of MP3 ﬁles, there may be more than one copy of the same song, stored in different directories or with different ﬁle names. The goal of this exercise is to search for duplicates.

’

’

book.tex

’

’

md5sum

+ filename

1. Write a program that searches a directory and all of its subdirectories, recursively, and returns a list of complete paths for all ﬁles with a given sufﬁx (like .mp3). Hint: os.path provides several useful functions for manipulating ﬁle and path names.

2. To recognize duplicates, you can use md5sum to compute a “checksum” for each ﬁles. If two ﬁles have the same checksum, they probably have the same contents.

3. To double-check, you can use the Unix command diff.