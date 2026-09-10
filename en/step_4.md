## Detect a crash

Make the boat crash when it touches the wooden barrier.

## Step 1

Click on the **Code tab**.

![The Code tab selected](images/tab_code.png)

## Step 2

Inside the `forever`{:class="block3control"} loop, add an `if`{:class="block3control"} block.

```blocks3
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
end
+if < > then
+end
end
```

## Step 3

Add a `touching color`{:class="block3sensing"} block to detect if the boat is touching brown wood colour.

```blocks3
+if <touching color [#663b00] ?> then
end
```

Use the eyedropper tool to set the same brown as the wood.

![The eyedropper picking the brown wood colour](images/eyedropper.png)

## Step 4

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

![The crashed boat saying Noooooo!](images/boat-crash.png)
