’

>>> type( <type >>> type( <type

’

str ’

’

str

’

17 ’ > 3.2 ’ >

)

’

)

They’re strings.

When you type a large integer, you might be tempted to use commas between groups of three digits, as in 1,000,000. This is not a legal integer in Python, but it is legal:

12

Chapter 2. Variables, expressions and statements

messagenpi17’And now for something completely different’3.1415926535897932

Figure 2.1: State diagram.

>>> 1,000,000 (1, 0, 0)

Well, that’s not what we expected at all! Python interprets 1,000,000 as a comma- separated sequence of integers. This is the ﬁrst example we have seen of a semantic error: the code runs without producing an error message, but it doesn’t do the “right” thing.

2.2 Variables

One of the most powerful features of a programming language is the ability to manipulate variables. A variable is a name that refers to a value.

An assignment statement creates new variables and gives them values:

’