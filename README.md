micro:bit Egg Catching Game
--------------------
![](EggCatcherGame.gif)   
In this assignment you will create a "catch the egg" game on your micro:bit in which an egg (represented by a single LED) "falls" from the top of the micro:bit LED display and can be caught by a moveable basket at the bottom.

By default, the first "egg" LED starts to drop from the center of the top line. The basket at the bottom will also be at the center, so the first egg will be very easy to catch. Subsequent "eggs" will then fall from random positions at the top of the display. The basket can be moved by pressing the buttons or by tilting the micro:bit


Program requirements
-----------------
* Your program must use the Python `randint()` function
* Your program will use at least 3 variables: `eggX`, `eggY`, `basketX`
* If an egg falls to the bottom of the screen without being caught, the game will display a "Game Over" message
* The position of the egg and the basket will be set with the `display.set_pixel()` function

Suggested steps to getting the egg to drop
----------
1. Write two `import` statements at the top of your program:
    * `from microbit import *`
    * `import random`
2. Declare and initialize a variable `eggX` with a value of 2
3. Declare and initialize a variable `eggY` with a value of 0
4. Underneath the variable declarations, create a `while True:` loop
   1. Inside the `while` loop call `display.clear()`
   2. On the next line, call `display.setpixel()` to display the egg at position `eggX,eggY` with a value of `9`
   3. Set `eggY` to be larger by 1
   4. `sleep` for 500 milliseconds
5. Run the program, you should see the egg drop. If the egg falls past the bottom of the screen, you should see an error message

Suggested steps to adding the basket
----------
6. Under the other two variable declarations, declare and initialize a variable `basketX` with a value of 2
7. After `display.clear()`, call `display.setpixel()` to display the basket at position `basketX,4` with a value of `4`
8. Underneath the `sleep(500), create a `if` that checks if `eggY` is equal to `5` `and` `eggX` is equal to `basketX`
   1. If so, set `eggy` to `0`
   2. Set `eggy` to a random integer from 1 to 4
9. Run the program, you should see the egg drop. When it reaches the basket, it should drop again from a random position at the top of the screen

Suggested steps to moving the basket
----------
10. After `display.clear()`, add two `if` statements
11. If `basketX` is greater than 0 `and` button a was pressed
   * Set `basketX` to be smaller by 1
12. If `basketX` is less than 4 `and` button b was pressed
   * Set `basketX` to be larger by 1
13. Run the program, you should be able to catch the egg. If you miss the egg and it falls past the bottom of the screen, you should see an error message

Suggested steps to ending the game
----------
14. TBD

Extensions
----------
You can move the basket with the accelerometer rather than the buttons. You could also keep score of the number of eggs caught and display the score along with the game over message.

Samples of Student Work
----------
*none yet!*
