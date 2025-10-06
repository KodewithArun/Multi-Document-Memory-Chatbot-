If we test this function with the words “pots” and “stop”, we expect the return value True, but we get an IndexError: ’

’

’

’

pots

>>> is_reverse( ...

,

stop

)

77

78

Chapter 8. Strings

i0j3word1’pots’word2’stop’

Figure 8.2: State diagram.

File "reverse.py", line 15, in is_reverse

if word1[i] != word2[j]:

IndexError: string index out of range

For debugging this kind of error, my ﬁrst move is to print the values of the indices imme- diately before the line where the error appears.

while j > 0:

print i, j

# print here

if word1[i] != word2[j]:

return False

i = i+1 j = j-1

Now when I run the program again, I get more information:

’

’

’

’

pots

>>> is_reverse( 0 4 ... IndexError: string index out of range

,

stop

)

The ﬁrst time through the loop, the value of j is 4, which is out of range for the . The index of the last character is 3, so the initial value for j should be string len(word2)-1.

’

’

pots