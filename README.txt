using this site to learn:
https://www.youtube.com/watch?v=GFO_txvwK_c&ab_channel=freeCodeCamp.org

typed the code from that video above.

source is freecodecamp, project#9 in the youtube video.


To run, download Live Server on Visual Studio Code. Right click index.html and click on run with live server.

Game Description:
Uses Delta time and Uses different states for the sprites

Game Rules:
Avoid the enemies.
-5 score if touch enemy, -1 live
-10 score if touch enemy while rolling. <- should change this to positive and instead just limit roll time.
(live is not lost when rolling and touch enemy)


RESOLVED:
/////////-fox does not jump. Watch 7:30:09 about jumping. Seems to be related to player.js
and 7:44:10 about playerState jumping class.
check: main.js, player.js, playerstate.js
descriptive: when jump is pressed, fox doesnt jump and goes straight into falling animation.
y axis does not move at all./////FIXED Problem was a small typo in the onGround class in player.js
-climbing and ground enemies are not appearing -> FIXED after changing enemies.js to -> this.x-=this.speedX+this.gamespeed;
-flying enemies disappearing randomly -> //  FIXED was typo here->  if(enemy.markedForDeletion) this.enemies.splice(this.enemies.indexOf(enemy),1)
-fly enemies are not flying properly. -> FIXED
- button 'd' wasn't working, FIXED by adding game to input.js constructor and   this.game=game;
-HP feature in UI.js doesnt work. FIXED.
-particles not appearing. FIXED - added particles code in main.js for draw()


Feature ideas:
game ideas: after a certain amount of score, level up and evolve?
make game harder, else can abuse the roll feature. -> end roll animation after x seconds after pressing enter.
Shop implementation and "coins" to collect? or can use score as money.
button to reset game rather than F5.
pause feature.
changing the fox to another char.
making it two player local game.
score system by time rather than enemy system? makes it harder and better for two player.
keeping track of scores and high score.
limit times can roll?

-> use x axis if player reaches certain distance they win.
as time goes on, make game harder by increasing enemy frequency.


CHANGES:
Changed enter to z(Do this by changing in UI and playerstates)
note: tried to change to "Spacebar" but that involves potentially changing e.key to e.code
which would make changing playerState not as straightforward

changed player.js 's weight and playerstate to adjust falling speed. note that when rolling can still jump high.
-> should adjust horizontal speed to become slower.