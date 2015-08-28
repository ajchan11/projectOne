# Project 1: Whack a Dictator!

![alt tag](https://github.com/ajchan11/projectOne/blob/master/readme/intro.png)

Name of the game: Whack a Mole

Objective: Whack as many dictators as quickly as possible within the 30 second time limit. Minus 10 points for hitting the Dalai Lama!

1. Began constructing the game with a simple layout of 8 x 3 squares.

![alt tag](https://github.com/ajchan11/projectOne/blob/master/readme/outline2.png)

2. Used a random number generator that cycles through the number of squares, randomly choosing one. The chosen box is given a new variable "random". 

![alt tag](https://github.com/ajchan11/projectOne/blob/master/readme/boxes.png)

3. Created a new class with a background image of my "mole".

![alt tag](https://github.com/ajchan11/projectOne/blob/master/readme/active.png)

4. Created a function that had an if/else statement. If the random box had the class "active", the box had the class "active" removed and a new global random variable was assigned to random. Else, the class "active" was given to the random box and a new global random variable was assigned. 

![alt tag](https://github.com/ajchan11/projectOne/blob/master/readme/swap.png)

4. Game keep track of time by creating a function with a setTimeout with 1000ms. The function was constantly looped and the variable "s" was redefined to represent a count down clock in which 1 was subtracted from s. If s < 1, the gameStop function was called.

![alt tag](https://github.com/ajchan11/projectOne/blob/master/readme/time.png)

5. The function gameStop cleared the timeOut number given in setTimeout as well as cleared the game interval that would be called. The body element was given the class "gameOver" which displayed the gameOver sign, and all other classes were removed. the "display" score was pushed into an array "highScore" which had a default var highScore = [0]. The timer was replaced with "Time has finished"

![alt tag](https://github.com/ajchan11/projectOne/blob/master/readme/stop.png)

6. The game begins when a player clicks a mode. Each mode begins with removing the class "gameOver" from the body, the "s" is reset to 30. the "display" score is reset to 0 and the global interval variable is definied with the function "startGame" and the time frequency in which the function is constantly called. The function "gameCount" is called and the timer begins. 

![alt tag](https://github.com/ajchan11/projectOne/blob/master/readme/easy.png)