## Detect a crash

Make the boat crash and reset when it touches a wooden barrier.

You're still working on the `Boat`{:class="block3looks"} sprite.

## Step 1

Add blocks inside your `forever`{:class="block3control"} loop that keep checking whether the boat is touching the brown wood.

If it is, switch to the `hit` costume, say something, then reset the boat's position.

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
switch costume to (hit v)
say [Noooooo!] for (2) seconds
switch costume to (normal v)
point in direction (0)
go to x: (-190) y: (-150)
end
```

## Step 2

Make sure the boat always starts out looking `normal`.

```blocks3
when flag clicked
+switch costume to (normal v)
point in direction (0)
go to x: (-190) y: (-150)
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
```

## Now run your code

Sail the boat into a wooden barrier.

The boat crashes and then moves back to its starting position.

![screenshot](images/boat-crash.png)
