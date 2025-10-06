’

’

2

With the methods we have so far, we can create and print cards:

>>> card1 = Card(2, 11) >>> print card1 Jack of Hearts

Figure 18.1 is a diagram of the Card class object and one Card instance. Card is a class object, so it has type type. card1 has type Card. (To save space, I didn’t draw the contents of suit_names and rank_names).

18.3 Comparing cards

For built-in types, there are relational operators (<, >, ==, etc.) that compare values and de- termine when one is greater than, less than, or equal to another. For user-deﬁned types, we can override the behavior of the built-in operators by providing a method named __cmp__.

__cmp__ takes two parameters, self and other, and returns a positive number if the ﬁrst object is greater, a negative number if the second object is greater, and 0 if they are equal to each other.