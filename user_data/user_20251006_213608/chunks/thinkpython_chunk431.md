suffix_map = {} prefix = ()

Because these variables are global we can only run one analysis at a time. If we read two texts, their preﬁxes and sufﬁxes would be added to the same data structures (which makes for some interesting generated text).

To run multiple analyses, and keep them separate, we can encapsulate the state of each analysis in an object. Here’s what that looks like:

175

176

Chapter 18. Inheritance

class Markov(object):

def __init__(self):

self.suffix_map = {} self.prefix = ()

Next, we transform the functions into methods. For example, here’s process_word:

def process_word(self, word, order=2):

if len(self.prefix) < order:

self.prefix += (word,) return

try:

self.suffix_map[self.prefix].append(word)

except KeyError:

# if there is no entry for this prefix, make one self.suffix_map[self.prefix] = [word]

self.prefix = shift(self.prefix, word)