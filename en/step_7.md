## Add a timer

Add a timer so the player has to reach the island as quickly as possible.

## Step 1

Click on the **Stage**.

## Step 2

Add a new variable called `time`{:class="block3variables"}.

[[[generic-scratch3-add-variable]]]

![screenshot](images/boat-variable-annotated.png)

## Step 3

Add code to the **Stage** so the timer counts up in tenths (0.1) of a second.

![stage](images/stage.png)

```blocks3
when flag clicked
set [time v] to [0]
forever
wait (0.1) seconds
change [time v] by (0.1)
end
```

## Now run your code

Play the game and watch the timer.

See how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)
