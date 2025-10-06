The is operator indicates that p1 and p2 are not the same object, which is what we expected. But you might have expected == to yield True because these points contain the same data. In that case, you will be disappointed to learn that for instances, the default behavior of the == operator is the same as the is operator; it checks object identity, not object equivalence. This behavior can be changed—we’ll see how later.

If you use copy.copy to duplicate a Rectangle, you will ﬁnd that it copies the Rectangle object but not the embedded Point.

147

148

Chapter 15. Classes and objects

y0.0x0.0widthheight100.0corner200.0box100.0200.0widthheightcornerbox2

Figure 15.3: Object diagram.

>>> box2 = copy.copy(box) >>> box2 is box False >>> box2.corner is box.corner True

Figure 15.3 shows what the object diagram looks like. This operation is called a shallow copy because it copies the object and any references it contains, but not the embedded objects.