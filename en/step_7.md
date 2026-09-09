## Add a timer

Add a timer so the player has to reach the island quickly.

## Step 1

Click on the **Stage**.

## Step 2

Add a new variable called `time`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

![screenshot](images/boat-variable-annotated.png)

## Step 3

Add code to the **Stage** to reset the timer and start a loop.

![stage](images/stage.png)

```blocks3
when flag clicked
set [time v] to [0]
forever
end
```

## Step 4

Inside the loop, count up in tenths of a second.

```blocks3
when flag clicked
set [time v] to [0]
forever
+wait (0.1) seconds
+change [time v] by (0.1)
end
```

## Now run your code

Click the green flag and race to the island.

Check that the timer counts up as you play.

![screenshot](images/boat-variable-test.png)
