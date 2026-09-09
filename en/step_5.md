## Reset after a crash

Send the boat back to the start when it crashes.

Inside the `if`{:class="block3control"} block, add `movement`{:class="block3motion"} and `costume`{:class="block3looks"} blocks to reset the boat.

```blocks3
if <touching color [#663b00] ?> then
switch costume to (hit v)
say [Noooooo!] for (2) seconds
+switch costume to (normal v)
+point in direction (0)
+go to x: (-190) y: (-150)
end
```

## Now run your code

Click the green flag.

Crash into a barrier and check that the boat goes back to the start.
