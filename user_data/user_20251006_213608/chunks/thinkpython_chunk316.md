’

’

’

’

’

a

,

b

,

>>> t = [ ] >>> hist = histogram(t) >>> print hist {

a

’

’

’

’

: 1}

b

a

: 2,

your function should return ’a’ with probability 2/3 and ’b’ with probability 1/3.

13.3. Word histogram

13.3 Word histogram

You should attempt the previous exercises before you go on. You can download my so- lution from http://thinkpython.com/code/analyze_book.py. You will also need http: //thinkpython.com/code/emma.txt.

Here is a program that reads a ﬁle and builds a histogram of the words in the ﬁle:

import string

def process_file(filename):

hist = dict() fp = open(filename) for line in fp:

process_line(line, hist)

return hist

def process_line(line, hist): line = line.replace(

’

’



,

’ ’

)

for word in line.split():

word = word.strip(string.punctuation + string.whitespace) word = word.lower()

hist[word] = hist.get(word, 0) + 1

hist = process_file(

’

emma.txt

’

)

This program reads emma.txt, which contains the text of Emma by Jane Austen.