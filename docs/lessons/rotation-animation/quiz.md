# rotation animation quiz

Learn how to create a rotating image with a while loop. #image #loop  #while #docs

## Name

## Directions

Use this activity document to guide your work in the [rotation animation tutorial](/microbit/lessons/rotation-animation/tutorial).

Answer the questions while completing the tutorial. Pay attention to the dialogues!

## 1. What is a " variable"?

<br />

## 2. Write the code to create a variable called foo that stores a boolean and initialize it to false.

<br/>

## 3. Explain why you use a while loop with a variable

```blocks
let rotating = true;
while (rotating) {
    basic.showLeds(`
        . . . . .
        . . . . .
        . . # . .
        . . . . .
        . . . . .
        `)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        `)
}

```

<br/>

## 4. Draw the areas on the micro:bits to illustrate the code below. Explain why you chose to draw in those areas.

```blocks
basic.showAnimation(`
# . . . . . . # . . . . . . # . . . . .
. # . . . . . # . . . . . # . . . . . .
. . # . . . . # . . . . # . . # # # # #
. . . # . . . # . . . # . . . . . . . .
. . . . # . . # . . # . . . . . . . . .
`, 400)
```

![](/static/mb/lessons/looper-2.png)

<br/>
