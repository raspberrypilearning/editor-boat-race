## Winning

The player wins when the boat reaches the island.

## Step 1

Below the crash check, add an empty `if`{:class="block3control"} block.

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
+if < > then
+end
```

## Step 2

Check if the boat is `touching`{:class="block3sensing"} the yellow island.

```blocks3
+if <touching color [#FFFF99] ?> then
end
```

Use the eyedropper took to select the yellow colour.

add image here

## Step 3

Add a `say`{:class="block3looks"} YEAH! for when you win and `stop all`{:class="block3control"}.

```blocks3
if <touching color [#FFFF99] ?> then
+say [YEAH!] for (2) seconds
+stop [all v]
end
```

## Now run your code

Click the green flag and steer to the island.

Check that the boat says YEAH! and the game stops.

> ## Tip
>
> To test winning quickly, change the first `go to`{:class="block3motion"} block to `go to x: (150) y: (-90)`.
>
> Change it back afterwards.
