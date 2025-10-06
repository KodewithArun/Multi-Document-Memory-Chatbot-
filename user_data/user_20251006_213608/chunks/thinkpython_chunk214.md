’

’

pots

If I ﬁx that error and run the program again, I get: ’

’

’

’

pots

>>> is_reverse( 0 3 1 2 2 1 True

,

stop

)

This time we get the right answer, but it looks like the loop only ran three times, which is suspicious. To get a better idea of what is happening, it is useful to draw a state diagram. During the ﬁrst iteration, the frame for is_reverse is shows in Figure 8.2.

I took a little license by arranging the variables in the frame and adding dotted lines to show that the values of i and j indicate characters in word1 and word2. Exercise 8.9. Starting with this diagram, execute the program on paper, changing the values of i and j during each iteration. Find and ﬁx the second error in this function.

8.12 Glossary

object: Something a variable can refer to. For now, you can use “object” and “value”

interchangeably.

8.13. Exercises

sequence: An ordered set; that is, a set of values where each value is identiﬁed by an

integer index.