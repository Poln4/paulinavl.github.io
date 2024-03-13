# Family UNO
#### Video Demo:  <URL https://youtu.be/4Ym6EKDC_C8>
#### Description:
This project has two parts.
1. A C file to play at the terminal.
2. A dinamic web app with a database run with Flask.

Motivation
My motivation for this project is my family. They like to play UNO and they have their own rules to play.
The cards get some values and whoever reaches or overpass 200 set the end of the game. Players need to count their points and keep track of them.
That is why I made this. I want to help my family by facilitating the recollection of points. So, they will stop using random papers. And we can keep a record of the best players.

Projects
The firt parts was made with C.
I piloted the idea with my family during my summer vacations.
The program is functional and it helped us to play. I followed some suggestions of my family to improve it, but it has some limitations.
I coundn't keep a track of the rounds before nor check the historical winners.
Then, I decided to make a more dinamic wep app with the use of database to keep records.

Common ground:
In both parts, the starting point is to add the names of the players. Later on, round by round, the user needs to input the points of each player and the system count them and detect if someone has reached or overpassed 200 points.
When that happens, both system will stop the game and determine the winner.

Difference:
In the web app, there is an additional feature: top winners (records).
People can examine who has been the winner in previous sessions, regarless of the day of consult.
If people don't know how to play, they can check the rules of the UNO game, and if they don't know how to use the web app, there are instructions too.

Limitations
There are some features that I would like to improve in the future.
For example, I set 10 rounds at the maximum. But I cound set to add rounds to the data base in case it is needed.
Now, if players run out of rounds, they will be kick out.
Also, I could show the number of rounds they have been playing.
Anyway, I am happy with what I have done so far.

Web App pages:
Main page. Here we can add players by clicking in the button, or we can access to it by the navigation bar.
Add players. Here, the user can add the name of players and check there name in a list after inputing them in.
New game. It reset the points of the players to 0.  It can be clicked whenever a player finds it fit, like in the middle of a game or after a game is finished.
Top winners. Here users can see the top winners over privious games. This list never changes.
Rules. User can check the general rules of the game and also the instructions to use the web app.

Inside the code:
In the app.py there are more functions than html templates, but they are all connected.



