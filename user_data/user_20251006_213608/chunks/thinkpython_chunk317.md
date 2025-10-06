’

emma.txt

’

)

This program reads emma.txt, which contains the text of Emma by Jane Austen.

process_file loops through the lines of the ﬁle, passing them one at a time to process_line. The histogram hist is being used as an accumulator.

process_line uses the string method replace to replace hyphens with spaces before using split to break the line into a list of strings. It traverses the list of words and uses strip and lower to remove punctuation and convert to lower case. (It is a shorthand to say that strings are “converted;” remember that string are immutable, so methods like strip and lower return new strings.)

Finally, process_line updates the histogram by creating a new item or incrementing an existing one.

To count the total number of words in the ﬁle, we can add up the frequencies in the his- togram:

def total_words(hist):

return sum(hist.values())

The number of different words is just the number of items in the dictionary:

def different_words(hist):