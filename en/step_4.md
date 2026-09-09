## Detect a crash

Make the boat crash when it touches a wooden barrier.

You're still working on the **Boat sprite**.

## Step 1

Inside the `forever`{:class="block3control"} loop, add an `if`{:class="block3control"} block.

Set it to check if the boat is `touching`{:class="block3sensing"} the brown wood.

Inside the `if`{:class="block3control"} block, add `switch costume to`{:class="block3looks"} hit.

Then add `say`{:class="block3looks"} something.

[[[scratch3-set-block-input-colour-with-eyedropper]]]

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
end
+if <touching color [#663b00] ?> then
+switch costume to (hit v)
+say [Noooooo!] for (2) seconds
+end
```

## Step 2

Still inside the `if`{:class="block3control"} block, add blocks to send the boat back to the start.

```blocks3
if <touching color [#663b00] ?> then
switch costume to (hit v)
say [Noooooo!] for (2) seconds
+switch costume to (normal v)
+point in direction (0)
+go to x: (-190) y: (-150)
end
```

## Now run your code

Click the green flag and crash into a barrier.

Check that the boat crashes and jumps back to the start.

![screenshot](images/boat-crash.png)
