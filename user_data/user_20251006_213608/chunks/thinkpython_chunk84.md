For this reason, it is a good idea to add notes to your programs to explain in natural lan- guage what the program is doing. These notes are called comments, and they start with the # symbol: # compute the percentage of the hour that has elapsed percentage = (minute * 100) / 60

In this case, the comment appears on a line by itself. You can also put comments at the end of a line: percentage = (minute * 100) / 60 Everything from the # to the end of the line is ignored—it has no effect on the program.

# percentage of an hour

Comments are most useful when they document non-obvious features of the code. It is reasonable to assume that the reader can ﬁgure out what the code does; it is much more useful to explain why.

This comment is redundant with the code and useless: v = 5

# assign 5 to v

This comment contains useful information that is not in the code: v = 5

# velocity in meters/second.