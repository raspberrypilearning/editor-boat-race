## Speed the boat up

Make the boat go faster over a white arrow.

![boat sprite](images/boat_resize.png)

Click on the **Boat sprite**.

Inside the `forever`{:class="block3control"} loop, add an `if`{:class="block3control"} block.

Set it to check if the boat is `touching`{:class="block3sensing"} white.

Inside it, add `move 3 steps`{:class="block3motion"}.

```blocks3
if <touching color [#FFFFFF] ?> then
move (3) steps
end
```

## Now run your code

Click the green flag and drive over an arrow.

Check that the boat speeds up.
