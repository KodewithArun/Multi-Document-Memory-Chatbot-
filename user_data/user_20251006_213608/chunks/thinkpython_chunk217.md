’

’

c return

.islower(): ’ ’

True

79

80

Chapter 8. Strings

else:

return

’

False

’

def any_lowercase3(s):

for c in s:

flag = c.islower()

return flag

def any_lowercase4(s):

flag = False for c in s:

flag = flag or c.islower()

return flag

def any_lowercase5(s):

for c in s:

if not c.islower(): return False

return True

Exercise 8.12. ROT13 is a weak form of encryption that involves “rotating” each letter in a word by 13 places. To rotate a letter means to shift it through the alphabet, wrapping around to the beginning if necessary, so ’A’ shifted by 3 is ’D’ and ’Z’ shifted by 1 is ’A’.

Write a function called rotate_word that takes a string and an integer as parameters, and that returns a new string that contains the letters from the original string “rotated” by the given amount.

For example, “cheer” rotated by 7 is “jolly” and “melon” rotated by -10 is “cubed”.