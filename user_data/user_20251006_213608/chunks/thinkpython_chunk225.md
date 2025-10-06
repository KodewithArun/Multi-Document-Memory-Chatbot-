for letter in word:

if letter not in available:

return False

return True

Instead of a list of forbidden letters, we have a list of available letters. If we ﬁnd a letter in word that is not in available, we can return False.

uses_all is similar except that we reverse the role of the word and the string of letters: def uses_all(word, required):

for letter in required:

if letter not in word:

return False

return True

Instead of traversing the letters in word, the loop traverses the required letters. If any of the required letters do not appear in the word, we can return False.

If you were really thinking like a computer scientist, you would have recognized that uses_all was an instance of a previously-solved problem, and you would have written: def uses_all(word, required):

return uses_only(required, word)