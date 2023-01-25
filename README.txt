using this site to learn:
https://www.youtube.com/watch?v=GFO_txvwK_c&ab_channel=freeCodeCamp.org

typed the code from that video above.

source is freecodecamp, project9 in the youtube video.


To run, download Live Server on Visual Studio Code. Right click index.html and click on run with live server.




Current bugs:

/////////-fox does not jump. Watch 7:30:09 about jumping. Seems to be related to player.js
and 7:44:10 about playerState jumping class.
check: main.js, player.js, playerstate.js/////SOLVED! Problem was a small typo in the onGround method

descriptive: when jump is pressed, fox doesnt jump and goes straight into falling animation.
y axis does not move at all.

-fly enemies are not transitioning properly.
-climbing and ground enemies are not appearing
check enemies.js

Unlikely to have mistake:
playerstate.js