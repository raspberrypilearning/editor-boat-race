## Speed the boat up

Make the boat go faster over a white arrow.

## Step 1

![The boat sprite](images/boat_resize.png)

On the **Boat sprite** add an `if`{:class="block3control"} and `touching`{:class="block3sensing"} block. Use the eyedropper tool to set the colour to the white arrows.

```blocks3
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
+if <touching color [#FFFFFF] ?> then
+end
```

## Step 2

Move the boat faster by adding a `move`{:class="block3motion"} block and changing it to `3`.

```blocks3
if <touching color [#FFFFFF] ?> then
+move (3) steps
end
```

## Now run your code

Click the green flag and drive over an arrow.

Check that the boat speeds up.
