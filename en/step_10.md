## Speed the boat up

Make the boat go faster over a white arrow.

## Step 1

![boat sprite](images/boat_resize.png)

Click on the **Boat sprite**.

Inside the `forever`{:class="block3control"} loop, add an empty `if`{:class="block3control"} and `touching`{:class="block3sensing"} block.

```blocks3
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
end
if <touching color [#663b00] ?> then
switch costume to (hit v)
say [Noooooo!] for (2) seconds
switch costume to (normal v)
point in direction (0)
go to x: (-190) y: (-150)
end
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
+if <touching color [#FFFFFF] ?> then
+end
```
Use the eyedropper tool to set the colour to the white arrows.

## Step 2

Inside it, add `move 3 steps`{:class="block3motion"}.

```blocks3
if <touching color [#FFFFFF] ?> then
+move (3) steps
end
```

## Now run your code

Click the green flag and drive over an arrow.

Check that the boat speeds up.
