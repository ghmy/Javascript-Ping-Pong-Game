# Javascript-Ping-Pong-Game
Based on the Udemy Course "Code Your First Game: Arcade Classic in JavaScript on Canvas", I developed the ping pong game further.

game_simple.html is the very slightly updated (calculation of paddle-ball and paddle-wall collisions) project of the mentioned Udemy course. 
The other files are different as to how the calculation is done to move the paddle.

The crucial part is the calculateHitPoint() method. 

For the left paddle, the hit point is (PADDLE_THICKESS, y); for the right paddle, the hit point is (canvas.width - PADDLE_THICKNESS, y)
and that y coordinate is calculated by calculateHitPoint function. This method runs once the game starts/resets and once the opponent 
hits the ball. After the calculation, the paddle goes to that y coordinate and waits for the ball. 
