## Speed the boat up

Make the boat go faster when it drives over a white arrow.

![boat sprite](images/boat_resize.png)

Click on the `Boat`{:class="block3looks"} sprite.

Add more blocks to the boat's `forever`{:class="block3control"} loop so the boat moves three extra steps when it touches white.

```blocks3
if <touching color [#FFFFFF] ?> then
move (3) steps
end
```

## Now run your code

Click the green flag and drive over your booster arrows.

The boat speeds up as it crosses them.
