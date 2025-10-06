For most applications, invoking grow_rectangle on one of the Rectangles would not affect the other, but invoking move_rectangle on either would affect both! This behavior is confusing and error-prone.

this is not what you want.

In this example,

Fortunately, the copy module contains a method named deepcopy that copies not only the object but also the objects it refers to, and the objects they refer to, and so on. You will not be surprised to learn that this operation is called a deep copy. >>> box3 = copy.deepcopy(box) >>> box3 is box False >>> box3.corner is box.corner False box3 and box are completely separate objects. Exercise 15.3. Write a version of move_rectangle that creates and returns a new Rectangle instead of modifying the old one.

15.7 Debugging