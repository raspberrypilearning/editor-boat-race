## Winning

Make the player win when the boat reaches the island.

You're still working on the **Boat sprite**.

Inside the `forever`{:class="block3control"} loop, below the crash check, add an `if`{:class="block3control"} block.

Set it to check if the boat is `touching`{:class="block3sensing"} the yellow island.

Inside it, add `say`{:class="block3looks"} YEAH!

Then add `stop all`{:class="block3control"}.

```blocks3
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
```

## Now run your code

Click the green flag and steer to the island.

Check that the boat says YEAH! and the game stops.

## Tip

To test winning quickly, change the first `go to`{:class="block3motion"} block to `go to x: (150) y: (-90)`.

Change it back afterwards.
