I use Python to demonstrate these implementations, but in real life you wouldn’t write code like this in Python; you would just use a dictionary! So for the rest of this chapter, you have to imagine that dictionaries don’t exist and you want to implement a data structure that maps from keys to values. The operations you have to implement are:

add(k, v): Add a new item that maps from key k to value v. With a Python dictionary, d,

this operation is written d[k] = v.

get(target): Look up and return the value that corresponds to key target. With a Python

dictionary, d, this operation is written d[target] or d.get(target).

For now, I assume that each key only appears once. The simplest implementation of this interface uses a list of tuples, where each tuple is a key-value pair.

class LinearMap(object):

def __init__(self): self.items = []

def add(self, k, v):

self.items.append((k, v))

def get(self, k):

for key, val in self.items:

if key == k:

return val

raise KeyError