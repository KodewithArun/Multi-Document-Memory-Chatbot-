To see how this works, think about starting with an empty HashTable and adding a se- quence of items. We start with 2 LinearMaps, so the ﬁrst 2 adds are fast (no resizing re- quired). Let’s say that they take one unit of work each. The next add requires a resize, so we have to rehash the ﬁrst two items (let’s call that 2 more units of work) and then add the third item (one more unit). Adding the next item costs 1 unit, so the total so far is 6 units of work for 4 items.

The next add costs 5 units, but the next three are only one unit each, so the total is 14 units for the ﬁrst 8 adds.

B.4. Hashtables

Figure B.1: The cost of a hashtable add.

The next add costs 9 units, but then we can add 7 more before the next resize, so the total is 30 units for the ﬁrst 16 adds.