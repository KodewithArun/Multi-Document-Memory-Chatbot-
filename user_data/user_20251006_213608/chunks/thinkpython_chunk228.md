’

flossy

’

Here is a version of is_palindrome (see Exercise 6.6) that uses two indices; one starts at the beginning and goes up; the other starts at the end and goes down. def is_palindrome(word):

i = 0 j = len(word)-1

while i<j:

if word[i] != word[j]:

return False

i = i+1 j = j-1

return True

9.5. Debugging

Or, if you noticed that this is an instance of a previously-solved problem, you might have written:

def is_palindrome(word):

return is_reverse(word, word)

Assuming you did Exercise 8.9.

9.5 Debugging

Testing programs is hard. The functions in this chapter are relatively easy to test because you can check the results by hand. Even so, it is somewhere between difﬁcult and impos- sible to choose a set of words that test for all possible errors.

Taking has_no_e as an example, there are two obvious cases to check: words that have an ’e’ should return False; words that don’t should return True. You should have no trouble coming up with one of each.