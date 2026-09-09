## Speed the boat up

Make the boat go faster over a white arrow.

![boat sprite](images/boat_resize.png)

Click on the **Boat sprite**.

## Step 1

Inside the `forever`{:class="block3control"} loop, add an empty `if`{:class="block3control"} block.

```blocks3
+if < > then
+end
```

## Step 2

Set the condition to check if the boat is `touching`{:class="block3sensing"} white.

```blocks3
+if <touching color [#FFFFFF] ?> then
end
```

## Step 3

Inside it, add `move 3 steps`{:class="block3motion"}.

```blocks3
if <touching color [#FFFFFF] ?> then
+move (3) steps
end
```

## Now run your code

Click the green flag and drive over an arrow.

Check that the boat speeds up.
