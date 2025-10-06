7.3 The while statement

Computers are often used to automate repetitive tasks. Repeating identical or similar tasks without making errors is something that computers do well and people do poorly.

We have seen two programs, countdown and print_n, that use recursion to perform rep- etition, which is also called iteration. Because iteration is so common, Python provides several language features to make it easier. One is the for statement we saw in Section 4.2. We’ll get back to that later.

Another is the while statement. Here is a version of countdown that uses a while statement:

def countdown(n):

while n > 0:

print n n = n-1

’

print

Blastoff!

’

You can almost read the while statement as if it were English. It means, “While n is greater than 0, display the value of n and then reduce the value of n by 1. When you get to 0, display the word Blastoff!”

More formally, here is the ﬂow of execution for a while statement:

1. Evaluate the condition, yielding True or False.