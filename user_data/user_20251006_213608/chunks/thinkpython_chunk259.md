Because the words are in alphabetical order, we can speed things up with a bisection search (also known as binary search), which is similar to what you do when you look a word up in the dictionary.

10.15. Exercises

You start in the middle and check to see whether the word you are looking for comes before the word in the middle of the list. If so, then you search the ﬁrst half of the list the same way. Otherwise you search the second half.

Either way, you cut the remaining search space in half. If the word list has 113,809 words, it will take about 17 steps to ﬁnd the word or conclude that it’s not there.

Write a function called bisect that takes a sorted list and a target value and returns the index of the value in the list, if it’s there, or None if it’s not.