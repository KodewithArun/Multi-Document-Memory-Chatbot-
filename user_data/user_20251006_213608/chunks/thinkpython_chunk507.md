The in operator for sequences uses a linear search; so do string methods like find and count.

If the elements of the sequence are in order, you can use a bisection search, which is O(logn). Bisection search is similar to the algorithm you probably use to look a word up in a dictionary (a real dictionary, not the data structure). Instead of starting at the be- ginning and checking each item in order, you start with the item in the middle and check whether the word you are looking for comes before or after. If it comes before, then you search the ﬁrst half of the sequence. Otherwise you search the second half. Either way, you cut the number of remaining items in half.

If the sequence has 1,000,000 items, it will take about 20 steps to ﬁnd the word or conclude that it’s not there. So that’s about 50,000 times faster than a linear search.

205

206

Appendix B. Analysis of Algorithms