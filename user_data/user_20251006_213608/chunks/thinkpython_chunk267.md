An implementation is a way of performing a computation; some implementations are better than others. For example, an advantage of the dictionary implementation is that we don’t have to know ahead of time which letters appear in the string and we only have to make room for the letters that do appear.

Here is what the code might look like: def histogram(s): d = dict() for c in s:

if c not in d:

d[c] = 1

else:

d[c] += 1

return d

The name of the function is histogram, which is a statistical term for a set of counters (or frequencies).

The ﬁrst line of the function creates an empty dictionary. The for loop traverses the string. Each time through the loop, if the character c is not in the dictionary, we create a new item with key c and the initial value 1 (since we have seen this letter once). If c is already in the dictionary we increment d[c].