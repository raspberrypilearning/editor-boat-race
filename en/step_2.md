## Smooth out the movement

The boat jitters when it reaches the pointer, you can smooth it out. 

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
Check that the `distance to`{:class="block3sensing"} the mouse pointer is `more than 5`{:class="block3operators"}.

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

Click the green flag and move your mouse near the boat.

Check that the boat stops jittering.
