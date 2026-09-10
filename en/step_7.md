## Winning

The player wins when the boat reaches the island.

## Step 1

At the bottom of the `forever`{:class="block3control"} loop, add an empty `if`{:class="block3control"} block.

```blocks3
forever
if <touching color [#663b00] ?> then
switch costume to (hit v)
say [Noooooo!] for (2) seconds
switch costume to (normal v)
point in direction (0)
go to x: (-190) y: (-150)
end
+if < > then
+end
end
```

## Step 2

Add a `touching color`{:class="block3sensing"} block and use the eyedropper tool to select the yellow colour of the island.

```blocks3
+if <touching color [#FFFF99] ?> then
end
```

## Step 3

Add a `say`{:class="block3looks"} YEAH! for when you win and `stop all`{:class="block3control"}.

```blocks3
if <touching color [#FFFF99] ?> then
+say [YEAH!] for (2) seconds
+stop [all v]
end
```

> ## Tip
>
> To test winning quickly, change the first `go to`{:class="block3motion"} block to `go to x: (150) y: (-90)`{:class="block3motion"}.
>
> Change it back to `go to x: (-190) y: (-150)`{:class="block3motion"} afterwards.

## Now run your code

Click the green flag and steer to the island.

Check that the boat says YEAH! and the game stops.
