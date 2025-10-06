dy = event.y - self.dragy

self.dragx = event.x self.dragy = event.y

self.move(dx, dy)

This computation is done in pixel coordinates; there is no need to convert to Canvas coor- dinates.

Finally, drop restores the original color of the item:

def drop(self, event):

self.config(fill=self.fill)

You can use the Draggable class to add drag-and-drop capability to an existing item. For example, here is a modiﬁed version of make_circle that uses circle to create an Item and Draggable to make it draggable:

def make_circle(event):

pos = ca.canvas_coords([event.x, event.y]) item = ca.circle(pos, 5, fill= item = Draggable(item)

’

’

red

)

This example demonstrates one of the beneﬁts of inheritance: you can modify the capa- bilities of a parent class without modifying its deﬁnition. This is particularly useful if you want to change behavior deﬁned in a module you did not write.

19.9 Debugging