# Ping-Pong-Game

ball: A constant that stores a reference to the HTML div element with the id attribute ball. This element represents the ball in the game.
rod1: A constant that stores a reference to the HTML div element with the id attribute BluRaptor. This element represents the left player's rod in the game.
rod2: A constant that stores a reference to the HTML div element with the id attribute YellooRaptor. This element represents the right player's rod in the game.
\_name: A constant that stores the string "\_name", which is used as the key for storing the name of the rod with the highest score in local storage.
\_score: A constant that stores the string "\_score", which is used as the key for storing the maximum score in local storage.
bluRaptor: A constant that stores the string "Blu-Raptor", which is the name of the left player's rod.
yellooRaptor: A constant that stores the string "Yelloo-Raptor", which is the name of the right player's rod.
score: A variable that stores the current score of the game.
maxScore: A variable that stores the maximum score achieved in previous games.
movement: A variable that stores the interval ID for the game loop.
rod: A variable that stores the name of the rod with the highest score.
ballSpeedX: A variable that stores the speed of the ball in the x direction.
ballSpeedY: A variable that stores the speed of the ball in the y direction.
rod1X: A variable that stores the x position of the left player's rod.
rod2X: A variable that stores the x position of the right player's rod.
gameOn: A boolean variable that indicates whether the game is currently in progress.
windowWidth: A variable that stores the width of the window.
windowHeight: A variable that stores the height of the window.
The code also defines the following functions:

resetBoard(): This function sets the initial positions of the ball and rods, and sets the gameOn variable to false. It also clears the local storage. It takes one argument, rodName, which is the name of the rod that lost the previous game (if any).
storeWin(): This function is called when a player wins the game. It stores the name of the winning rod and the score in local storage if the score is greater than the current maximum score. It then clears the interval, calls the resetBoard() function with the rod name as an argument, and displays an alert message with the final score and the maximum score.
The anonymous function passed to the addEventListener() method for the keydown event: This function moves the rods left or right based on the key press, and starts the game if the Enter or Space key is pressed. The game consists of a loop that updates the ball's position, checks for collisions with the rods or walls, and ends the game if a player scores. It also updates the score and displays it on the screen.
