## Start looking normal

Make sure the boat always starts out on its `normal` costume, even after a crash.

You're still working on the `Boat`{:class="block3looks"} sprite.

Add a `switch costume to (normal v)`{:class="block3looks"} block at the very start of your code.

```blocks3
when flag clicked
+switch costume to (normal v)
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
```

## Now run your code

Crash the boat, then click the green flag again.

The boat always starts on its normal costume, ready to race.
