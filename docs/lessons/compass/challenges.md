# compass challenges

Display the direction that the micro:bit is facing using the compass 

## Before we get started

Complete the following [guided tutorial](/microbit/lessons/compass/activity), your code should look like this:

```blocks
 let degrees = null;
basic.forever(() => {
    degrees = input.compassHeading();
    if (degrees < 45) {
        basic.showString("N");
    }
    else if (degrees < 135) {
        basic.showString("E");
    }
    else if (degrees < 225) {
        basic.showString("S");
    }
    else {
        basic.showString("W");
    }
});
```

### Challenge 1

Instead of displaying `N` when the BBC micro:bit is pointing North, display a star to indicate the north star.

```blocks
 let degrees = null;
basic.forever(() => {
    degrees = input.compassHeading();
    if (degrees < 45) {
        basic.showLeds(`
# . # . #
. # # # .
# # # # #
. # # # .
# . # . #`);
    }
    else if (degrees < 135) {
        basic.showString("E");
    }
    else if (degrees < 225) {
        basic.showString("S");
    }
    else {
        basic.showString("W");
    }
});
```


* Run your code to see if it works as expected

### Challenge 2

Instead of displaying just `N`, `W`, `S`, or `E`, display the full word.

```blocks
 let degrees = null;
basic.forever(() => {
    degrees = input.compassHeading();
    if (degrees < 45) {
        basic.showString("NORTH");
    }
    else if (degrees < 135) {
        basic.showString("EAST");
    }
    else if (degrees < 225) {
        basic.showString("SOUTH");
    }
    else {
        basic.showString("WEST");
    }
});
```


* Run your code to see if it works as expected

### Challenge 3

Display your own unique message for each direction.
