## Controlling the boat

Make the boat start in the corner and follow the mouse pointer.

![boat sprite](images/boat_resize.png)

Click on the `Boat`{:class="block3looks"} sprite, then add this code so it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
point towards (mouse-pointer v)
move (1) steps
```

## Now run your code

Click the green flag and move your mouse.

The boat turns and follows the pointer around the screen.

--- no-print ---

![screenshot](images/boat-pointer-test-anim.gif)

--- /no-print ---

--- print-only ---

![screenshot](images/boat-pointer-test-anim.png)

--- /print-only ---
