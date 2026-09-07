## Smooth out the movement

When the boat reaches the mouse pointer, it jitters about.

Fix this so the boat only moves when it is more than 5 pixels away from the pointer.

You're still working on the `Boat`{:class="block3looks"} sprite.

Add an `if`{:class="block3control"} block that checks whether the `distance to the mouse pointer`{:class="block3sensing"} is `greater than 5`{:class="block3operators"}, and put the movement inside it.

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
+if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

## Now run your code

Move the mouse near the boat.

The boat stops jittering when the pointer is close.
