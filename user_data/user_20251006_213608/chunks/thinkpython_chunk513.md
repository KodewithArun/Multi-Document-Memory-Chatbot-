Here (ﬁnally) is the crucial idea that makes hashtables fast: if you can keep the maximum length of the LinearMaps bounded, LinearMap.get is constant time. All you have to do is keep track of the number of items and when the number of items per LinearMap exceeds a threshold, resize the hashtable by adding more LinearMaps.

Here is an implementation of a hashtable:

207

208

Appendix B. Analysis of Algorithms

class HashMap(object):

def __init__(self):

self.maps = BetterMap(2) self.num = 0

def get(self, k):

return self.maps.get(k)

def add(self, k, v):

if self.num == len(self.maps.maps):

self.resize()

self.maps.add(k, v) self.num += 1

def resize(self):

new_maps = BetterMap(self.num * 2)

for m in self.maps.maps: for k, v in m.items:

new_maps.add(k, v)

self.maps = new_maps

Each HashMap contains a BetterMap; __init__ starts with just 2 LinearMaps and initializes num, which keeps track of the number of items.