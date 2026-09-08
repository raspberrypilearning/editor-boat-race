## Winning!

Let the player win when the boat reaches the island.

You're still working on the `Boat`{:class="block3looks"} sprite.

Add more blocks inside your `forever`{:class="block3control"} loop that check whether the boat is touching the island.

If it is, say `YEAH!` and then stop the game.

```blocks3
when flag clicked
switch costume to (normal v)
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
+if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
```

## Now run your code

Click the green flag and steer all the way to the island.

The boat says `YEAH!` and the game stops.

## Tip

To reach the island quickly while testing, temporarily change the first `go to`{:class="block3motion"} block to `go to x: (150) y: (-90)`, then change it back when you're done.
