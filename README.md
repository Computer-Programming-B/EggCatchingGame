micro:bit Egg Catching Game
--------------------
[](EggCatcherGame.gif)   
In this assignment you will create a "catch the egg" game on your micro:bit in which an egg (represented by a single LED) "falls" from the top of the micro:bit LED display and can be caught by a moveable basket at the bottom.

By default, the first "egg" LED starts to drop from the center of the top line. The basket at the bottom will also be at the center, so the first egg will be very easy to catch. Subsequent "eggs" will then fall from random positions at the top of the display. The basket can be moved by pressing the buttons or by tilting the micro:bit


Program requirements
-----------------
* Your program must use the Python `randint()` function
* Your program will use at least 3 variables: `eggX`, `eggY`, `basketX`
* If an egg falls to the bottom of the screen without being caught, the game will display a "Game Over" message
* The position of the egg and the basket will be set with the `display.set_pixel()` function

Suggested steps to completing this assignment
----------
1. Write two `import` statements at the top of your program:
    * `from microbit import *`
    * `import random`
2. Declare and initialize a variable `eggX` with a value of 2
3. Declare and initialize a variable `eggY` with a value of 2
4. Underneath the variable declarations, create a `while True:` loop
5. TBD

Extensions
----------
You can move the basket with the accelerometer rather than the buttons. You could also keep score of the number of eggs caught and display the score along with the game over message.

Samples of Student Work
----------
*none yet!*
