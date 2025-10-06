One way to improve LinearMap is to break the list of key-value pairs into smaller lists. Here’s an implementation called BetterMap, which is a list of 100 LinearMaps. As we’ll see in a second, the order of growth for get is still linear, but BetterMap is a step on the path toward hashtables: class BetterMap(object):

def __init__(self, n=100):

self.maps = [] for i in range(n):

self.maps.append(LinearMap())

def find_map(self, k):

index = hash(k) % len(self.maps) return self.maps[index]

def add(self, k, v):

m = self.find_map(k) m.add(k, v)

def get(self, k):

m = self.find_map(k) return m.get(k) __init__ makes a list of n LinearMaps.

find_map is used by add and get to ﬁgure out which map to put the new item in, or which map to search.

find_map uses the built-in function hash, which takes almost any Python object and returns an integer. A limitation of this implementation is that it only works with hashable keys. Mutable types like lists and dictionaries are unhashable.