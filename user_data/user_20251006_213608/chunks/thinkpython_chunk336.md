log f = logc − slogr

So if you plot log f versus log r, you should get a straight line with slope −s and intercept log c.

Write a program that reads a text from a ﬁle, counts word frequencies, and prints one line for each word, in descending order of frequency, with log f and log r. Use the graphing program of your choice to plot the results and check whether they form a straight line. Can you estimate the value of s?

Solution: http://thinkpython.com/code/zipf.py. To make the plots, you might have to install matplotlib (see http://matplotlib.sourceforge.net/).

Chapter 14

Files

14.1 Persistence

Most of the programs we have seen so far are transient in the sense that they run for a short time and produce some output, but when they end, their data disappears. If you run the program again, it starts with a clean slate.