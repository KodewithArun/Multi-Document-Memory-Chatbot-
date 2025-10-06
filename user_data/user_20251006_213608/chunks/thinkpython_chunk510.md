def get(self, k):

for key, val in self.items:

if key == k:

return val

raise KeyError

add appends a key-value tuple to the list of items, which takes constant time.

get uses a for loop to search the list: if it ﬁnds the target key it returns the corresponding value; otherwise it raises a KeyError. So get is linear.

An alternative is to keep the list sorted by key. Then get could use a bisection search, which is O(logn). But inserting a new item in the middle of a list is linear, so this might

B.4. Hashtables

not be the best option. There are other data structures (see http://en.wikipedia.org/ wiki/Red-black_tree) that can implement add and get in log time, but that’s still not as good as constant time, so let’s move on.