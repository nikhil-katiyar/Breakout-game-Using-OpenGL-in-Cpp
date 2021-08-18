# Breakout-game-Using-OpenGL-in-C-
The project has been implemented in Microsoft Visual Studio Community Edition 2019 which uses C and/or C++ as the language tool. The objective of the game is to eliminate all of the BRICKS that are distributed around the top of the game screen. The bricks get broken after coming in contact with a ball that bounces around the screen. At the bottom is a paddle that in the game moves based on user input from keyboard or mouse. The player moves a PADDLE from side-to-side to hit the BALL. The user has to make sure the ball bounces off the paddle without going off the bottom of the screen. But, if the ball hits the bottom enclosure, the player loses and the game ends! To win the game, the player has to eliminate all the BRICKS in the respective levels. There is a score for a player which is the number of bricks the player was able to destroy before the ball hit the base.

## Gameplay Instructions
In order to play the game, press “S” to launch the ball. After pressing the S key to launch the ball, the ball will be moving.
The players can control the paddle movement in two different ways. It can be controlled by the keyboard as well as the mouse. The player uses the “A” and “D” keys
to move the paddle to the left and to the right respectively. 
For mouse controls the player's movement of the mouse pointer on screen determines the movement of the paddle accordingly.
During the game, if at any time the player wishes to start a new game, he could press the “Q” key.
The goal of the game is to break all of the bricks by intercepting the ball with the paddle and redirecting the ball to collide with the bricks.

## Menu
Players are allowed to change and customize game settings and difficulty using the menu. 
When the player right clicks the mouse,a menu appears which is quite self descriptive. Players can change the colour of the ball, bricks, paddle and text. There is an option to choose the difficulty level namely “Easy”, “Medium” and “Hard”. 
Level ‘Easy’ refers to normal speed and as the level increases to ‘Hard’, the speed increases. Also, the game difficulty can be increased by changing the paddle size from small, medium to large.
Default is “Easy” difficulty level and “Medium” size of paddle.
The major milestones for the project implementation were: 
● Displaying the bricks and disappearing after hitting the ball.
● Creating Small platform/paddle which moves left and right given user input from mouse or keyboard buttons ‘a’ and ‘d’. 
● The ball must deflect back after hitting brick, side walls and paddle at the bottom.
● Changing the game difficulty by changing the speed of the ball as well as the paddle size for different levels.

## Concepts Used
All the Computer Graphics concepts that are implemented are listed below:

### Translation: 
Concept of translation is used in the game while moving the paddle as well as while the ball is in motion rebounding from the different surfaces.

### Scaling: 
Concept of scaling can be seen in the game when the changing paddle size, the scaling of the paddle differs. When the paddle selected is ‘small’ we scale the paddle smaller and when it is ‘large’ we scale the paddle longer. This concept is also used when ball is created and scaled it to better view.

### Drawing Circle: 
For drawing the ball the function solidsphere present in glut library is used.

### Drawing Polygons: 
Different shapes (paddle and bricks) were drawn using the inbuilt polygon function and quads function and defining the appropriate vertices which matches the shape of
the polygon.

### Game Concept: 
Breakout is a famous retro game where we have to destroy all the bricks and the ball should not fall. If the ball falls the game will restart. The main player of the game is
paddle, we have to save the ball from going below by the paddle and at the same time try to hit as many bricks as possible.

### Difficulty Levels: 
To ensure the users interest in the game we came up with different levels and difficulties, the concepts for the level are described below:
a) Changing Size of Paddle: For this we changed the position of the vertices while defining the polygon. That way we can make the paddle smaller or bigger.
b) Changing the speed of the Ball: For this particular feature we decided to have a rate variable which on increasing gives us a high speed of the ball and vice versa. This
rate depends on the x-coordinate and the y-coordinate. The more the rate means the faster the x and y coordinates will change.

### Keyboard Inputs: 
Now for playing the game the user needs some kind of input to give. This can be done very easily by using a glut function ‘keyboard’ and then by specifying the role of
the keys in the switch case. In each switch case you need to define what that key will do.

### Hitting the Brick: 
This is the concept which comes into play when the ball hits the brick. This function defines the trajectory of the ball after hitting. We used the concept by applying the if
else conditions and accordingly changing the direction of the ball. 

### Trajectory of the Ball: 
The concept used for this particular feature of our game which handles the motion of the ball along with the rebounding from various surfaces. Here one condition is for increasing the rate after some successive collisions and another condition is to make the changes for the different directions of the ball after rebounding.

## GameScreen
![Screenshot (512)](https://user-images.githubusercontent.com/56537415/129949257-ac6ef605-cd0d-4a40-a688-69c0ac8878a3.png)

## Menu
![Screenshot (514)](https://user-images.githubusercontent.com/56537415/129949260-81520242-b89c-4bf6-9f18-7ea55e154bc0.png)

## Gameplay
![Screenshot (513)](https://user-images.githubusercontent.com/56537415/129949262-22466c32-6709-4626-a875-2eb7737fa689.png)
