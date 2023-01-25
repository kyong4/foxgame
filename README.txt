using this site to learn:
https://www.youtube.com/watch?v=GFO_txvwK_c&ab_channel=freeCodeCamp.org

typed the code from that video above.

source is freecodecamp, project#9 in the youtube video.


To run, download Live Server on Visual Studio Code. Right click index.html and click on run with live server.


RESOLVED:
/////////-fox does not jump. Watch 7:30:09 about jumping. Seems to be related to player.js
and 7:44:10 about playerState jumping class.
check: main.js, player.js, playerstate.js
descriptive: when jump is pressed, fox doesnt jump and goes straight into falling animation.
y axis does not move at all./////SOLVED! Problem was a small typo in the onGround class in player.js
-climbing and ground enemies are not appearing -> FIXED after changing enemies.js to -> this.x-=this.speedX+this.gamespeed;

-flying enemies disappearing randomly -> //  FIXED was typo here->  if(enemy.markedForDeletion) this.enemies.splice(this.enemies.indexOf(enemy),1)
-fly enemies are not flying properly. -> FIXED

BUGS:
-particles not appearing
-HP feature in UI.js doesnt work.

Feature ideas:
game ideas: after a certain amount of score, level up and evolve?
make game harder, else can abuse the roll feature. -> end roll animation after x seconds after pressing enter.
Shop implementation and "coins" to collect? or can use score as money.
button to reset game rather than F5.

changing the fox to another char.

CHANGES:
Changed enter to z(Do this by changing in UI and playerstates)
note: tried to change to "Spacebar" but that involves potentially changing e.key to e.code
which would make changing playerState not as straightforward