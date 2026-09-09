## Detect a crash

Make the boat crash when it touches the wooden barrier.

## Step 1

Inside the `forever`{:class="block3control"} loop, add an `if`{:class="block3control"} block.

```blocks3
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
end
+if < > then
+end
```

## Step 2

Check if the boat is `touching`{:class="block3sensing"} the brown wood colour.

```blocks3
+if <touching color [#663b00] ?> then
end
```

Use the eyedropper tool to set the same brown as the wood.

ADD gif or screen shot.

## Step 3

If touching the wood, `switch costume`{:class="block3looks"} to hit and `say`{:class="block3looks"} "Noooooo!".

```blocks3
if <touching color [#663b00] ?> then
+switch costume to (hit v)
+say [Noooooo!] for (2) seconds
end
```

## Now run your code

Click the green flag and crash into a barrier.

Check that the boat shows its wrecked costume and says Noooooo!

![screenshot](images/boat-crash.png)
