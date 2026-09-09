## Smooth out the movement

Make the boat stop moving when it touches the pointer.

## Step 1
Wrap the movement in an `if`{:class="block3control"} block.

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
+if < > then
point towards (mouse-pointer v)
move (1) steps
```

## Step 2
Add a `more than`{:class="block3operators"} block and change the number to `5`. Drag a `distance to mouse-pointer`{:class="block3sensing"} block into the other slot.

```blocks3
forever
+if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

## Now run your code

Click the green flag and move your mouse near the boat.

Check that the boat stops jittering.
