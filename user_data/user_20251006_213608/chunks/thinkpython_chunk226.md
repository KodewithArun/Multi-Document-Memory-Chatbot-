return uses_only(required, word)

This is an example of a program development method called problem recognition, which means that you recognize the problem you are working on as an instance of a previously- solved problem, and apply a previously-developed solution.

9.4 Looping with indices

I wrote the functions in the previous section with for loops because I only needed the characters in the strings; I didn’t have to do anything with the indices.

83

84

Chapter 9. Case study: word play

For is_abecedarian we have to compare adjacent letters, which is a little tricky with a for loop: def is_abecedarian(word): previous = word[0] for c in word:

if c < previous: return False

previous = c

return True

An alternative is to use recursion: def is_abecedarian(word): if len(word) <= 1: return True

if word[0] > word[1]: return False

return is_abecedarian(word[1:])

Another option is to use a while loop: def is_abecedarian(word):

i = 0 while i < len(word)-1:

if word[i+1] < word[i]: