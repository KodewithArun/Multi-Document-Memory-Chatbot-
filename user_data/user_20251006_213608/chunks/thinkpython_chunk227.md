i = 0 while i < len(word)-1:

if word[i+1] < word[i]:

return False

i = i+1 return True

The loop starts at i=0 and ends when i=len(word)-1. Each time through the loop, it com- pares the ith character (which you can think of as the current character) to the i + 1th character (which you can think of as the next).

If the next character is less than (alphabetically before) the current one, then we have dis- covered a break in the abecedarian trend, and we return False.

If we get to the end of the loop without ﬁnding a fault, then the word passes the test. To convince yourself that the loop ends correctly, consider an example like . The length of the word is 6, so the last time the loop runs is when i is 4, which is the index of the second-to-last character. On the last iteration, it compares the second-to-last character to the last, which is what we want.

’

flossy

’