9.3 Search

All of the exercises in the previous section have something in common; they can be solved with the search pattern we saw in Section 8.6. The simplest example is:

9.4. Looping with indices

def has_no_e(word):

for letter in word: e if letter ==

’

’

:

return False

return True

The for loop traverses the characters in word. If we ﬁnd the letter “e”, we can immediately return False; otherwise we have to go to the next letter. If we exit the loop normally, that means we didn’t ﬁnd an “e”, so we return True.

avoids is a more general version of has_no_e but it has the same structure: def avoids(word, forbidden): for letter in word:

if letter in forbidden:

return False

return True

We can return False as soon as we ﬁnd a forbidden letter; if we get to the end of the loop, we return True.

uses_only is similar except that the sense of the condition is reversed: def uses_only(word, available):

for letter in word:

if letter not in available:

return False

return True